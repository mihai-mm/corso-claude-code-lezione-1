# Anatomia di una skill

Una skill non è una formula magica: è fatta di pezzi, e ogni pezzo ha un mestiere. Qui te li spiego tutti.

Non li costruisci tutti oggi. Oggi (Lezione 1) ti servono i primi tre. Gli altri sono il cuore della Lezione 4: te li lascio qui così sai già dove stai andando, ma non devi padroneggiarli adesso.

Una cosa da tenere a mente per tutto: **una skill, in pratica, è una cartella con dentro un file di testo** (si chiama `SKILL.md`). Niente di esoterico. Un foglio di istruzioni, scritto bene.

## Quello che ti serve oggi

### Il nome / comando

Come richiami la skill. Una parola che inizia con `/`: per esempio `/recap-discovery` o `/crea-proposta`.

La digiti nella chat e la skill parte.

### Il corpo - le istruzioni

È il cuore: cosa deve fare la skill e come deve comportarsi. Il "manuale" che il tuo collaboratore legge per fare il lavoro.

Una regola d'oro: **tienilo corto**. Più istruzioni ammucchi, peggio lavora. Un manuale snello e chiaro batte sempre un papiro di mille righe.

### Distillata dal lavoro che fai già a mano

Non è una parte del file, è il principio che decide se la tua skill sarà buona o scadente.

Le skill migliori non si inventano a tavolino: nascono prendendo un lavoro che fai sempre uguale, a mano, e cristallizzandolo. Se il modo in cui lo fai a mano è chiaro, la skill sarà ottima. Se è confuso, lo sarà anche lei.

Regola pratica: se fai una cosa a mano due volte, la terza falla diventare una skill.

## Quello che aggiungerai in Lezione 4

Questi non ti servono per partire. Sono il salto di qualità: trasformano una skill singola in un sistema che lavora da solo.

### La descrizione - il motore

Due o tre righe in cima al file che dicono a Claude due cose: *cosa fa* la skill e *quando* usarla.

È la riga che Claude legge per decidere se attivare la tua skill o ignorarla. Se è scritta male, il manuale sotto non viene mai letto. In Lezione 4 vedrai come scriverla perché si attivi quasi sempre.

### File di supporto (caricati quando servono)

Il file principale resta corto. Gli esempi lunghi, i casi particolari, i template li metti in **file separati** nella stessa cartella, e Claude li apre solo quando servono davvero.

Esempio: la skill che crea proposte ha il file principale snello. L'esempio completo di una proposta corporate, quello di una proposta per una piccola azienda, la lista dei termini di pagamento, stanno in file a parte. Claude li va a prendere solo se quel caso si presenta.

Come un dipendente con un manuale snello in mano e i faldoni di approfondimento nello schedario, che tira fuori solo quando gli serve quel caso.

### Script esterni (lavoro meccanico)

Certi pezzi di un lavoro sono pura esecuzione, sempre identica: non serve ragionare, serve solo fare. Quelli si scrivono come un piccolo programma che la skill lancia, invece di farli rifare all'AI ogni volta.

Esempio: "prendi questo Excel, somma la colonna fatturato, salva un PDF". È un calcolo sempre uguale: un programmino lo fa preciso e veloce, mentre l'AI potrebbe sbagliare i conti o farli diversi ogni volta.

Come la calcolatrice: per sommare non chiami un genio della matematica ogni volta, usi lo strumento che dà sempre lo stesso risultato esatto.

### Tiene il segno (non si ripete)

La skill tiene un piccolo registro di quello che ha già fatto. Quando la rilanci, salta il già fatto e lavora solo le cose nuove.

Esempio: una skill che archivia le call segna quali ha già sistemato; la volta dopo salta quelle e processa solo le nuove. Senza questo, rifarebbe tutto da capo: riprocessa cose già fatte, manda tre volte la stessa email, fa casino.

(Da non confondere con il `MEMORY.md` che vedi nel Blocco B: quello è la memoria delle *decisioni* del cliente. Questo è solo il promemoria interno della skill su cosa ha già lavorato.)

### Orchestrazione (una skill ne chiama altre)

Una skill "madre" che fa partire altre skill in sequenza. Da "ho qualche comando utile" a "ho un sistema che parte da solo".

Esempio classico: un comando della mattina che lancia in automatico cinque skill diverse mentre tu ti fai il caffè.

## Come te ne crei una, in pratica

Non c'è un solo modo. Ne hai tre, e portano tutti allo stesso punto: un comando `/nome` che riusi all'infinito. Una cosa è comune a tutti e tre: **non la scrivi tu riga per riga - la chiedi a Claude**.

### 1. La distilli dal lavoro che fai a mano

Fai il lavoro come lo faresti comunque, a mano, dentro la chat. Quando il risultato ti piace, dici a Claude: "fanne una skill". Lui prende il processo che hai appena fatto e lo cristallizza in un comando.

È il modo più naturale: la skill nasce da qualcosa che hai già visto funzionare. È quello che hai visto oggi con `/recap-discovery`.

### 2. La costruisci col Plan Mode

Descrivi a Claude cosa vuoi ottenere. Prima di scrivere qualsiasi cosa, lui ti mostra **il piano**: come ha intenzione di costruirla. Tu lo leggi, lo approvi (o lo correggi), e solo dopo Claude la scrive.

Utile quando la skill è più articolata e vuoi controllare la direzione prima che parta. È il modo che useremo per `/crea-proposta`.

### 3. La prendi già pronta

Molte skill utili le ha già scritte qualcun altro. Le cerchi su GitHub o nella community, le installi nella tua cartella, e sono subito tue. Zero lavoro di scrittura.

È così che è stata presa la skill che genera i diagrammi di queste slide.

### Due regole che valgono per tutte e tre

**Se non ti convince, la sistemi parlando.** Non è scolpita nella pietra: provi, dici a Claude cosa cambiare, lui la corregge, riprovi. Finché non ti piace. La aggiusti a parole, non riscrivendo codice.

**Quando NON farne una.** Per cose che fai una volta sola, o che cambiano ogni volta. La skill ha senso solo quando il lavoro si ripete uguale.

## Il principio che vale per tutto

Quando chiedi a Claude di costruire una skill (perché **non la scrivi tu riga per riga** - gliela fai scrivere), vale una sola regola:

**Descrivi il risultato che vuoi, non i passi tecnici per arrivarci.**

Il tuo lavoro è sapere *cosa* vuoi ottenere. Il *come* è il suo mestiere.

## Cosa ti porti a casa oggi

- Una skill è una cartella con un file di istruzioni.
- Oggi ti bastano: nome/comando, corpo corto e chiaro, e il principio "distillala dal lavoro che fai già a mano".
- Il resto (descrizione-motore, file di supporto, script, registro, orchestrazione) è il salto della Lezione 4.
- La regola d'oro per chiederla a Claude: descrivi il risultato, non i passi.
