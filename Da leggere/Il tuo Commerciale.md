# Il tuo Commerciale

Lezione 1 - Parte A. Qui costruisci il primo collaboratore del tuo team AI: il commerciale, quello che dalla registrazione di una call tira fuori una proposta pronta da inviare, scritta come la scriveresti tu.

## Il problema che risolviamo

Fai una call commerciale andata bene: il cliente è interessato, c'è feeling, vi siete detti "ci sentiamo per una proposta".

Poi la proposta te la scrivi tu. La sera, quando sei già stanco. Ti rimetti davanti allo schermo e trasformi un'ora di chiacchiere in un documento scritto.

È un lavoro lento e sempre uguale. E ha un costo nascosto: più tardi arriva la proposta, più il cliente si è raffreddato. Il momento giusto per mandargliela era quando era ancora caldo.

Questo lavoro, da oggi, lo fa il tuo commerciale.

## Cosa ti serve: la trascrizione della call

Una cosa sola: il **testo** della call. Quello che vi siete detti, scritto.

Per averlo senza trascrivere a mano, usi uno strumento che sta in sottofondo durante la call (su Zoom, Meet o Teams), la registra e te la trascrive da solo:

- **Fathom** - quello che usiamo nel corso.
- **Granola** - alternativa equivalente.

Funzionano allo stesso modo: apri uno dei due, lo colleghi al tuo calendario, e da lì in poi ogni call diventa testo senza che tu faccia niente. A fine call trovi la trascrizione pronta.

## Il flusso, in pratica

1. Registri la call con Fathom (o Granola).
2. Copi la trascrizione in una cartella che chiami **inbox** (la tua "casella in entrata").
3. Lanci la skill.
4. Da qui non tocchi più niente: è la **skill** a creare la cartella di quel cliente, metterci dentro la trascrizione e scriverti la proposta.

Tu hai solo incollato un testo e dato un comando. Tutto il resto lo fa il sistema.

## Cos'è una skill

Fin qui hai usato l'AI con i **prompt**: scrivi una richiesta, l'AI risponde, e finisce lì. La volta dopo riscrivi tutto da capo.

Una **skill** è un'altra cosa. È un'istruzione che scrivi (o meglio, che fai scrivere a Claude) **una volta sola** e che resta lì, pronta. La richiami con un comando - per esempio `/crea-proposta` - e Claude esegue quel lavoro sempre allo stesso modo, con lo stesso metodo.

Il modo più semplice per capire la differenza:

- Un **prompt** è chiedere un favore a qualcuno che passa di lì. Lo fa una volta, poi se ne va.
- Una **skill** è **assumere e formare un collaboratore**. Gli spieghi come si fa una cosa una volta, e da quel momento la sa fare da solo, ogni volta che glielo chiedi.

C'è un'analogia che rende l'idea. Immagina di dover pagare le tasse: preferisci un genio della matematica che non ha mai visto una dichiarazione dei redditi, o un commercialista esperto che ne ha fatte mille? Il genio è bravissimo, ma parte da zero ogni volta. Il commercialista sa già esattamente cosa fare. L'AI da sola è il genio. La skill è quello che la trasforma nel commercialista esperto del tuo lavoro.

Due cose importanti da tenere a mente:

- **La skill non la scrivi tu riga per riga.** La chiedi a Claude: gli spieghi a parole cosa vuoi che faccia, e te la costruisce lui. Il tuo lavoro è sapere *cosa* chiedergli.
- **Una skill nasce dal lavoro che fai già a mano.** Le skill migliori non si inventano a tavolino: si costruiscono prendendo un lavoro che fai sempre uguale e cristallizzandolo. Se il modo in cui lo fai a mano è chiaro, la skill sarà ottima. Se è confuso, anche la skill lo sarà.

Regola pratica: **se fai una cosa a mano due volte, la terza falla diventare una skill.**

## Cosa può fare una skill

Una skill non scrive solo testo. Può:

- **Leggere** file e documenti che le dai (una trascrizione, un PDF, un foglio di calcolo).
- **Scrivere col tuo tono**, sempre allo stesso modo.
- **Seguire un formato fisso** ogni volta (es. una proposta con sempre le stesse sezioni).
- **Estrarre informazioni** da un testo lungo (date, numeri, decisioni, prossimi passi).
- **Riassumere e sintetizzare** ore di materiale in poche righe.
- **Creare cartelle e organizzare i file** al posto tuo.
- **Ricordarsi cosa ha già fatto** e non rifarlo due volte.
- **Partire con un comando solo**: digiti `/nome-skill` e parte.

## Come nasce la tua prima skill

Il metodo è sempre lo stesso, e lo vedrai dal vivo:

1. **Fai il lavoro a mano una volta, bene.** Prendi una trascrizione e chiedi a Claude di elaborarla: un riassunto pulito di cosa serve al cliente.
2. **Cristallizzalo.** Quando il risultato ti piace, dici a Claude: *"trasforma questo lavoro in una skill"*.
3. **Ora hai un comando.** Da lì in poi quel lavoro lo richiami con una parola, e viene sempre uguale.

La prima skill che costruiamo così è **`/recap-discovery`**: prende la trascrizione di una call commerciale e ne tira fuori un recap ordinato di cosa vuole il cliente.

Da lì, con lo stesso metodo, costruiremo la seconda - **`/crea-proposta-progetto`** - che dal recap genera la proposta vera e propria. Questa seconda la costruiamo col **Plan Mode** (Claude ti mostra il piano prima di scrivere, così correggi prima e non dopo): i dettagli sui modi di costruire una skill sono nel documento "Anatomia di una skill".

## La proposta: le 6 sezioni, sempre le stesse

La proposta che mandi al cliente ha sempre la stessa struttura. Sei sezioni: una volta che le sai, ogni proposta è solo un riempimento.

1. **Il problema** - i suoi dolori concreti, ripresi uno per uno dal recap. Gli dimostri che hai ascoltato: parli dei suoi problemi, non dei tuoi servizi.
2. **La proposta** - la tua soluzione al suo problema: l'idea di fondo e come la realizzi. Ogni dolore di prima trova qui la sua risposta.
3. **Il perimetro** - cosa fai concretamente e, soprattutto, cosa **non** fai. È la sezione che ti salva dai malintesi: senza, il cliente dà per scontato che tu faccia anche cose mai previste.
4. **Deliverable** - cosa riceve concretamente, nero su bianco.
5. **Prezzo** - una cifra chiara, niente range. Più la scadenza dell'offerta.
6. **Termini** - tempi, modalità di pagamento, prossimo passo.

Due sezioni fanno la differenza tra una proposta che chiude e una che resta nel cassetto: il **perimetro** (ti protegge) e il **prezzo** (una cifra sola - il range "tra i 2 e i 4 mila" fa sembrare che tu non sappia quanto vale il tuo lavoro).

## Scrivere col tuo tono: perché l'email AI si riconosce

Intorno alla proposta c'è tutto il resto: email, messaggi, presentazioni. Se chiedi a Claude "scrivimi l'email per Marco", esce un testo corretto ma generico, e il cliente capisce lontano un miglio che non l'hai scritto tu.

I segnali che tradiscono un'email scritta dall'AI:

- **Sempre lo stesso ordine**: richiamo alla call, "trovi in allegato", "rimango a disposizione", proposta di call, firma.
- **Frasi-fatte da manuale**: "prenderla in rassegna con calma", "rimango a disposizione per qualsiasi dubbio", "definire i prossimi passi". Suonano bene e non dicono niente.
- **Va bene per chiunque**: zero riferimento a cosa vi siete detti davvero. Se la mandi a cento clienti diversi funziona uguale, e quando un'email va bene per tutti non parla a nessuno.

Attenzione: se vedi dei buchi tipo `[Nome]` o `[recapiti]`, quelli non sono il difetto - sono solo dati che non hai dato all'AI. **Il difetto resta anche dopo averli riempiti: è il tono.** Generico, medio, da manuale. Perché l'AI non sa ancora come scrivi tu.

## Le due schede: chi sei e come scrivi

Nella Lezione 0 hai riempito il **CLAUDE.md**, la scheda d'identità: dice a Claude **chi sei** (il tuo lavoro, con chi lavori). Si carica da sola a ogni sessione.

Quello che gli manca è una seconda scheda: **come scrivi** - la tua voce, le parole che usi e quelle che eviti, quanto vai dritto al punto. Questa scheda si chiama **STYLE.md**.

Due schede dello stesso collaboratore: una sa chi sei, l'altra come suoni.

Lo STYLE.md, da solo, Claude non lo guarda: devi dirgli **quando** usarlo. Nel CLAUDE.md globale aggiungi un'istruzione:

```
Quando scrivi un'email, un messaggio o una presentazione per me, leggi sempre prima il file ~/.claude/STYLE.md e scrivi con quel tono.
```

Da quel momento, ogni volta che gli chiedi di scrivere qualcosa, Claude va prima a prendersi il tuo modo di scrivere. Non ci pensi più.

Per costruire il tuo STYLE.md passo dopo passo segui il file "Crea il tuo stile di scrittura" (nella cartella "Da usare con Claude"): lo dai a Claude e lui ti guida.
