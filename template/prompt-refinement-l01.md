# Prompt Refinement L01

## Prompt Di Partenza
```txt
Aggiungi un messaggio carino quando non ci sono ticket aperti.
```

## Diagnosi Operativa
- Informazioni mancanti: non sono specificati il contesto dell'applicazione, i file coinvolti, le caratteristiche del messaggio da mostrare e il linguaggio utilizzato nel progetto.
- Ambiguita': il termine "carino" è soggettivo e può essere interpretato in modi diversi.
- Rischio di scope troppo largo: l'AI potrebbe modificare componenti, logica o interfaccia non coinvolti nel problema.
- Output non verificabile: non è definito quale messaggio debba essere mostrato all'utente.
- Strategia iniziale: zero-shot, ma poco controllabile.
- Servono esempi? No, perché il problema può essere descritto in modo sufficientemente chiaro aggiungendo contesto, vincoli e criteri di verifica.

## Prompt Usato Per Migliorare

```text
Aiutami a migliorare questo prompt. 
Non risolvere il task. 
Dimmi prima quali informazioni mancano. 
Non mostrare chain-of-thought.
Poi proponi una versione migliore.
```


## Strategia Del Prompt Finale

- Zero-shot o few-shot: Zero-shot
- Motivo della scelta: il problema può essere descritto in modo sufficientemente chiaro aggiungendo contesto, vincoli, output atteso e criteri di verifica.
- Evidenze richieste all'AI: assunzioni, criterio utilizzato e verifica proposta.

## Prompt Migliorato

```txt
Contesto:
- Stiamo lavorando su una piccola applicazione React didattica per la gestione dei ticket. La lista dei ticket viene visualizzata nel componente `TicketsList.jsx`. In alcuni casi la lista può risultare vuota e l'interfaccia deve informare correttamente l'utente.

Confini e permessi:
- È possibile analizzare esclusivamente il caso in cui la lista dei ticket risulta vuota.
- È possibile definire un messaggio informativo quando non sono presenti ticket aperti.
- L'analisi deve essere limitata a questo specifico scenario.

Output richiesto
- Quando non sono presenti ticket con stato `"open"`, mostrare un messaggio in lingua italiana che informi chiaramente l'utente che non sono presenti ticket aperti.

Prova di controllo
- Se è presente almeno un ticket con stato `"open"`, il messaggio non deve essere visualizzato.
- Se non sono presenti ticket con stato `"open"`, il messaggio deve essere visualizzato.

Non-azione
- Non scrivere codice.
- Non proporre modifiche ai file del progetto.
- Non aggiungere nuove funzionalità.


Zero-shot / Few-shot
* Zero-shot: le istruzioni fornite sono sufficienti e non sono necessari esempi.
```

## Controllo Qualita'

- Contesto presente: si
- Confini espliciti: si
- Output atteso: si
- Prova di controllo: si
- Cosa chiede all'AI di non fare: non scrivere codice, non proporre modifiche ai file del progetto e non aggiungere nuove funzionalità.
- Esempi necessari e proporzionati: No
- Evita chain-of-thought estesa: si
- E' piu' specifico perche': definisce contesto, vincoli, output e criteri di verifica.
- Limita meglio il lavoro perche': restringe l'analisi al solo caso in cui non sono presenti ticket aperti.
- Produce un output piu' verificabile perche': definisce chiaramente quando il messaggio deve/non deve essere visualizzato.
- Lo classificherei come: Controllabile
