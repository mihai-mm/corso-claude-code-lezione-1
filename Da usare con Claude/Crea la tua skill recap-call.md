# Crea la tua skill recap-call

Questo è un file guidato: lo dai al tuo Claude e lui ti accompagna, un passo alla volta, a costruire la skill `/recap-call` - quella che dalla registrazione di una call con un cliente o un collaboratore tira fuori un recap ordinato, sempre con la stessa struttura.

È una delle strade per fare l'esercitazione. Scegli questa se preferisci essere condotto passo dopo passo. Se invece te la senti, puoi costruirla da solo col Plan Mode o partendo da una tua call - il metodo è quello che hai già visto stamattina con `/recap-discovery`.

Non devi sapere niente di tecnico. Devi solo avere una trascrizione di call da usare.

## Cosa otterrai

- La skill `/recap-call`: la richiami con un comando e ti trasforma qualsiasi trascrizione di call in un recap ordinato a sei parti.
- In più, dal recap ti tira fuori già pronti i compiti da fare (chi fa cosa) e mette da parte le decisioni importanti.

## Cosa ti serve prima di partire

- Claude Code installato e funzionante (Lezione 0).
- **Una trascrizione di una call** con un cliente o un collaboratore: una tua vera, oppure quella di esempio dei materiali del corso. Tienila pronta da incollare.

> Nota: `/recap-call` è per le call **operative** con clienti/collaboratori già acquisiti (cosa avete deciso, chi fa cosa). È diversa dalla `/recap-discovery`, che è per la call commerciale con un potenziale cliente e serve a fare la proposta.

## Come si usa

Apri Claude Code nella cartella dove hai salvato questo file e scrivi:

> leggi il file "Crea la tua skill recap-call.md" e seguilo

Da lì in poi Claude ti guida. Quando vuoi fermarti, basta dire "ci fermiamo qui".

## Stile di lavoro (regole per l'agente)

Queste sono le regole che il tuo Claude deve seguire mentre ti guida. Se le viola, fermalo.

1. **Un passo alla volta.** Mai fare due passi senza la tua conferma.
2. **Spiega prima di agire.** Prima di creare o modificare un file, ti dice cosa fa e perché.
3. **Niente gergo tecnico** dato per scontato: se usa un termine nuovo, lo spiega.
4. **Mostra prima, automatizza dopo**: prima ti fa vedere il recap a mano, poi lo trasforma in skill.

## Il processo (protocollo di esecuzione per l'agente)

Quando l'utente ti chiede di leggere e seguire questo file, esegui questi passi in ordine, applicando lo "Stile di lavoro". **Un passo alla volta, sempre con conferma.**

### Passo 1 - Fatti dare la trascrizione

Chiedi all'utente di incollarti la trascrizione di una call con un cliente o un collaboratore (una sua vera, o quella di esempio del corso). Aspetta che la incolli prima di proseguire.

### Passo 2 - Fai il recap a mano, una volta

Leggi la trascrizione e produci un recap ordinato in **sei parti**, senza che l'utente ti dia la struttura (gliela mostri tu):

1. **Di cosa avete parlato** - il riassunto della call.
2. **I temi, uno per uno** - i punti affrontati, le decisioni prese, le cose lette tra le righe.
3. **Chi fa cosa** - i compiti, divisi per persona, con la scadenza.
4. **Le domande aperte** - cosa è rimasto in sospeso.
5. **I prossimi passi** - le tre cose che contano di più.
6. **Il punto** - in due righe, ciò che conta davvero.

Poi, dal punto 3, estrai una **lista pulita dei compiti da fare** e segnala le **decisioni importanti** da non dimenticare.

Mostragli tutto e chiedi: *"Ti torna? Cosa cambieresti?"*. Aggiusta in base alla sua risposta. Questo è il modello da cui nascerà la skill: se il recap fatto a mano è buono, la skill sarà buona.

### Passo 3 - Trasformalo in una skill

Quando il recap lo convince, digli che adesso quel lavoro lo trasformate in un comando, così non dovrà rifarlo ogni volta. Crea la skill `/recap-call` a partire dal recap appena fatto. La skill deve:

- prendere una trascrizione e produrre il recap nelle sei parti di sopra;
- in più, estrarre la lista dei compiti da fare e mettere da parte le decisioni importanti;
- scrivere col tono dell'utente (se ha già il suo `STYLE.md`, lo rispetta).

Spiega che non la state scrivendo riga per riga: la state facendo costruire a Claude descrivendo il risultato voluto.

### Passo 4 - La prova che si ripete

Chiedi all'utente una **seconda** trascrizione (o usa di nuovo quella di esempio). Invece di rifare il lavoro a mano, lancia `/recap-call`. Fagli vedere che esce lo stesso recap a sei parti, con lo stesso metodo, in un comando solo.

### Chiusura

Riepiloga: ora ha la skill `/recap-call`, la richiama quando vuole, e gli dà sempre il recap a sei parti più la lista dei compiti e le decisioni da ricordare. Ricordagli che il recap va salvato nella cartella del cliente, così entra nella sua memoria storica (vedi il documento "Il tuo Account Manager").

## Note

- Se la skill non ti convince, la sistemi parlando: dici a Claude cosa cambiare e lui la corregge. Non si riscrive il codice a mano.
- Più la userai, più la affinerai. È normale che la prima versione non sia perfetta.
