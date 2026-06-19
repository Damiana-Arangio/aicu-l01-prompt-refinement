
## Diagnosi senza AI

## Contesto
**Quale informazione l'AI non può conoscere da sola?**
- L'AI non sa in quale linguaggio deve essere scritto il messaggio.
- L'AI non sa de deve modificare solo il messaggio o anche l'UI per mostrarlo
- L'AI non sa quali file deve analizzare, quindi potrebbe impiegare molto tempo ad esaminarli tutti prima di individuare quelli realmente coinvolti nella modifica.
- L'AI non sa come vengono gestiti e visualizzati i ticket aperti, quindi dovrebbe capire autonomamente dove intervenire.
- Non è definito quale comportamento ci si aspetta quando non sono presenti ticket aperti.

## Ambiguità
**Quale parola o richiesta può essere interpretata in più modi?**
- La richiesta di "aggiungere un messaggio più carino" è troppo ambigua perché il termine "carino" è soggettivo e lascia spazio a numerose interpretazioni.

## Fuori scope
**Quale modifica laterale va vietata prima di iniziare?**
- L'AI non deve modificare file che non sono coinvolti nella visualizzazione dei ticket;
- L'AI non deve intervenire sulla logica di gestione dei ticket;
- L'AI non deve apportare modifiche all'UI, se non richieste esplicitamente.


## Fine
**Quale prova dice che il prompt è abbastanza controllabile?**

Il prompt non è controllabile perché:
- Non fornisce abbastanza contesto;
- Non specifica né i vincoli da rispettare e né le azioni che che l'AI non deve eseguire;
- Non definisce né il formato dell'output atteso;
- Non indica quale messaggio ci si aspetta di visualizzare.