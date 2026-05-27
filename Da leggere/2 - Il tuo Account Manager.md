# Il tuo Account Manager

Lezione 1 - Parte B. Qui costruisci il secondo collaboratore: l'account manager, quello che si ricorda di ogni cliente - cosa vi siete detti, cosa avete deciso, a che punto siete. Non più "dove eravamo rimasti?".

## Il problema che risolviamo

Fai una call con un cliente o un collaboratore. Vi dite cose, prendete decisioni, vi date dei compiti. Poi la settimana dopo: cosa avevamo deciso sul prezzo? Chi doveva mandare quel documento?

E quando riprendi un cliente dopo settimane, parti da zero: rileggi le email, cerchi gli appunti, ricostruisci tutto a memoria. Ogni volta.

Il tuo account manager risolve questo: ogni cliente diventa una **cartella che ricorda tutto**.

## L'archivio cliente

L'idea è semplice: **una cartella per ogni cliente**. Lì dentro vive tutto quello che riguarda quel cliente - le call, le decisioni, i documenti.

Quando lavori su quel cliente, apri quella cartella e Claude ha sotto mano tutta la sua storia. Non gli devi rispiegare niente.

## Le memorie del tuo collaboratore

Il tuo collaboratore ha due tipi di memoria: quella che vale **sempre** e quella che vale **per un cliente solo**.

**Memoria globale** (vale ovunque, con qualsiasi cliente):

- **CLAUDE.md** globale - **chi sei**: il tuo lavoro, con chi lavori. (Fatto nella Lezione 0.)
- **STYLE.md** - **come scrivi**: la tua voce. (Costruito nella Parte A, vedi il file "Crea il tuo stile di scrittura".)

Questi si caricano da soli a ogni sessione, qualunque cosa tu stia facendo.

**Memoria del cliente** (vale solo per quel cliente, dentro la sua cartella):

- **CLAUDE.md** locale - **le regole di questo cliente**: cosa fa, come va trattato, le sue particolarità. Si accende quando lavori nella sua cartella.
- **MEMORY.md** - **cosa avete deciso**: la memoria storica del cliente. Qui c'è la differenza tra "ricordare le call" e "ricordare le decisioni". Tre sezioni che non invecchiano:
  - **Decisioni** (con data e perché) - cosa avete scelto e per quale motivo.
  - **Insight** - cosa hai capito di questo cliente nel tempo.
  - **Numeri** - budget, prezzi, dati concordati.

Una cosa importante da capire: la memoria globale e quella del cliente **si sommano**. Quando lavori su un cliente, Claude ha in testa tutto insieme: chi sei, come scrivi, le regole di quel cliente e le sue decisioni. Non scegli quale usare, le ha tutte.

## La skill `/recap-call`

È la gemella della `/recap-discovery` che hai costruito nella Parte A, ma per uno scopo diverso:

- `/recap-discovery` = call **commerciale con un potenziale cliente** → serve a fare la **proposta**.
- `/recap-call` = call **operativa con un cliente o un collaboratore già acquisito** → serve a sintetizzare cosa vi siete detti.

Prende la trascrizione della call e ne tira fuori un recap ordinato, sempre con la stessa struttura. **Sei parti:**

1. **Di cosa avete parlato** - il riassunto della call in un colpo d'occhio.
2. **I temi, uno per uno** - i punti affrontati, le decisioni prese e le cose lette tra le righe.
3. **Chi fa cosa** - i compiti, divisi per persona, con la scadenza. È il cuore: è quello che dopo una call ti dimentichi sempre.
4. **Le domande aperte** - cosa è rimasto in sospeso, da chiarire.
5. **I prossimi passi** - le tre cose che contano di più.
6. **Il punto per te** - in due righe, ciò che conta davvero di quella call.

E un passo in più: dai compiti del punto 3 ti tira fuori la **lista delle cose da fare**, e mette da parte le **decisioni importanti** perché non si perdano. Non è un riassunto che leggi e chiudi: ti lascia il lavoro già organizzato.

Il recap si salva dentro la cartella del cliente (in `call/`): così non è un'email che si perde, ma entra nella memoria di quel cliente.

## Come la costruisci (esercitazione)

`/recap-call` la costruisci tu, perché il metodo l'hai già visto con `/recap-discovery`. Hai più strade, scegli quella al tuo livello:

1. **Da solo col Plan Mode** - descrivi a Claude cosa vuoi, lui ti mostra il piano, tu approvi.
2. **Partendo da una call vera** - dai a Claude una trascrizione di una tua call passata e parti da lì.
3. **Col metodo della Parte A** - fai il recap a mano una volta, poi dici "trasformalo in una skill".
4. **Con una guida passo-passo** - un file che ti conduce, come hai fatto per lo STYLE.md.

## Cosa ti porti a casa oggi

- Ogni cliente è una cartella che ricorda tutto: call, decisioni, documenti.
- Il collaboratore ha memoria globale (chi sei, come scrivi - sempre) e memoria del cliente (le sue regole, le sue decisioni - solo nella sua cartella), e le usa insieme.
- `MEMORY.md` non è il diario delle call: è il registro delle **decisioni, insight e numeri** del cliente.
- `/recap-call` trasforma una call con un cliente in un recap ordinato a 6 parti, e ti lascia già pronti i compiti da fare e le decisioni da ricordare.
