## Prompt Migliorato

## Contesto
* Stiamo lavorando su una piccola applicazione React didattica per la gestione dei ticket. La lista dei ticket viene visualizzata nel componente `TicketsList.jsx`. In alcuni casi la lista può risultare vuota e l'interfaccia deve informare correttamente l'utente.

## Confini e permessi
- È possibile analizzare esclusivamente il caso in cui la lista dei ticket risulta vuota.
- È possibile definire un messaggio informativo quando non sono presenti ticket aperti.
- L'analisi deve essere limitata a questo specifico scenario.

## Output richiesto
- Quando non sono presenti ticket con stato `"open"`, mostrare un messaggio in lingua italiana che informi chiaramente l'utente che non sono presenti ticket aperti.

## Prova di controllo
* Se è presente almeno un ticket con stato `"open"`, il messaggio non deve essere visualizzato.
* Se non sono presenti ticket con stato `"open"`, il messaggio deve essere visualizzato.

## Non-azione
- Non scrivere codice.
- Non proporre modifiche ai file del progetto.
- Non aggiungere nuove funzionalità.


## Zero-shot / Few-shot
- Zero-shot: le istruzioni fornite sono sufficienti e non sono necessari esempi.
