# Crea il tuo stile di scrittura (Style.md)

Questo è un file guidato: lo dai al tuo Claude e lui ti accompagna, un passo alla volta, a costruire la **scheda del tuo modo di scrivere** - lo `STYLE.md`. Alla fine Claude scriverà email, messaggi e presentazioni con la tua voce, non con quella media dell'AI.

Non devi sapere niente di tecnico. Devi solo incollare alcuni testi che hai già scritto tu e rispondere a qualche domanda.

---

## Perché ti serve

Quando chiedi a Claude di scriverti un'email, lui la scrive in modo corretto ma generico: stesse aperture, stesse frasi fatte, stesso entusiasmo di plastica. Si capisce lontano un miglio che è AI, e il cliente lo nota.

Il motivo è semplice: Claude non sa ancora *come scrivi tu*. Nella Lezione 0 gli hai detto **chi sei** (il `CLAUDE.md`, la scheda d'identità). Adesso gli dici **come scrivi** - una seconda scheda, lo `STYLE.md`.

Non si costruisce a tavolino descrivendo il proprio tono ("professionale ma cordiale" non vuol dire niente). Si costruisce partendo dai testi che hai già scritto: Claude li legge e tira fuori il tuo modo di scrivere da solo. È lo stesso metodo delle skill: parti da quello che fai già, e l'AI lo cristallizza.

---

## Cosa ti serve prima di partire

- Claude Code installato e funzionante (fatto nella Lezione 0).
- Il tuo `CLAUDE.md` globale già creato (fatto nella Lezione 0).
- **8-10 testi che hai scritto tu**, dove suoni come te: email a clienti, messaggi WhatsApp di lavoro, post. Tienili pronti da copiare. Vanno bene anche presi da Gmail o dal telefono.

---

## Come si usa

Apri Claude Code nella cartella dove hai salvato questo file e scrivi:

> leggi il file "Crea il tuo stile di scrittura.md" e seguilo

Da lì in poi Claude ti guida lui. Quando vuoi fermarti, basta dire "ci fermiamo qui".

---

## Cosa avrai alla fine

- Un file `STYLE.md` che descrive il tuo modo di scrivere, salvato nel posto giusto sul tuo computer.
- Il file **già collegato** al tuo `CLAUDE.md` globale: da quel momento Claude lo usa ogni volta che scrive un testo, non ci devi più pensare.
- La prova che funziona: Claude riscrive un'email e finalmente suona come te.

---

## Stile di lavoro (regole per l'agente)

Queste sono le regole che il tuo Claude deve seguire mentre ti guida. Se le viola, fermalo.

1. **Un passo alla volta.** Mai fare due passi senza la tua conferma.
2. **Spiega prima di agire.** Ogni volta che sta per scrivere o modificare un file, prima ti dice cosa fa e perché.
3. **Mai modificare file senza il tuo ok esplicito** - vale soprattutto per il `CLAUDE.md` globale alla fine.
4. **Niente gergo tecnico** dato per scontato: se usa un termine nuovo, lo spiega la prima volta.
5. **Parla la tua lingua**, non quella dell'AI: lo scopo di tutto è proprio questo.

---

## Il processo (protocollo di esecuzione per l'agente)

Quando l'utente ti chiede di leggere e seguire questo file, esegui questi passi in ordine, applicando lo "Stile di lavoro" qui sopra. **Un passo alla volta, sempre con conferma prima di procedere al successivo.**

### Passo 1 - Raccogli i suoi testi

Chiedi all'utente di incollarti **8-10 testi che ha scritto lui**, dove suona come sé. Spiegagli cosa va bene e cosa no:

- **Vanno bene**: email a clienti, messaggi WhatsApp/Google Chat di lavoro, post sui social, qualunque cosa abbia scritto di getto con parole sue.
- **Non vanno bene**: documenti formali copiati da template, testi scritti da altri, contratti, roba istituzionale. Non sono la sua voce.

Se l'utente ha pochi testi, vanno bene anche 4-5: meglio pochi e veri che tanti e finti. Aspetta che li incolli prima di proseguire.

### Passo 2 - Digli cosa hai capito del suo stile

Leggi i testi ed estrai i pattern ricorrenti. Poi presentaglieli in modo concreto e leggibile, con esempi presi dai SUOI testi. Guarda almeno:

- come **apre** e come **chiude** (saluti, formule)
- frasi **corte** o lunghe, dirette o articolate
- **parole ed espressioni che usa spesso**, e quelle che non usa mai
- livello di **formalità** (dà del tu? del lei? "ciao" o "buongiorno"?)
- **emoji e punteggiatura** (ne usa? quanti punti esclamativi?)
- se cambia tono tra **contesti diversi** (email cliente vs messaggio veloce)

Chiudi chiedendo: *"Ti riconosci in questo? Cosa correggeresti?"* e aspetta la sua risposta. Correggi in base a quello che dice.

### Passo 3 - Scrivi la bozza dello STYLE.md

Scrivi una bozza del file `STYLE.md` e mostragliela (non salvarla ancora). Strutturala per **contesti d'uso**, perché lo stesso utente scrive diversamente a seconda di chi legge. Per la prima versione tieni 1-3 contesti, quelli che usa davvero (tipicamente: email/messaggi ai clienti, messaggi informali). Per ogni contesto:

- **Quando uso questo tono** (a chi, in che situazione)
- **Come scrivo** (le caratteristiche estratte al Passo 2, in elenco)
- **Un esempio reale** preso dai suoi testi

Aggiungi in fondo una sezione **"Regole sempre valide"** (es. accenti corretti, cose che non scrive mai, lunghezza dei paragrafi, uso delle emoji).

Tienila semplice e leggibile: questa è la sua prima versione, crescerà nel tempo.

### Passo 4 - La prova del nove

Prima di salvare, metti alla prova la bozza. Chiedigli un caso concreto (es. *"scrivimi l'email per mandare una proposta a un cliente dopo una call"*) e scrivila **applicando lo STYLE.md appena fatto**. Fagliela leggere e chiedi: *"Adesso suona come te?"*.

Se non si riconosce, capisci cosa stona, aggiusta lo STYLE.md, e riprova. Ripeti finché non dice "sì, questo lo avrei scritto io".

### Passo 5 - Salva il file

Quando la bozza lo convince, salva il file come `~/.claude/STYLE.md` (accanto al `CLAUDE.md` globale fatto nella Lezione 0). Digli esattamente dove l'hai salvato e cosa c'è dentro.

### Passo 6 - Collega lo STYLE.md al CLAUDE.md globale

Spiega all'utente che lo `STYLE.md`, da solo, Claude non lo guarda: bisogna dirgli **quando** usarlo. Il `CLAUDE.md` globale si carica da solo a ogni sessione: ci aggiungi un'istruzione che dice a Claude di leggere lo STYLE.md ogni volta che scrive un testo.

Mostragli l'istruzione che stai per aggiungere al `~/.claude/CLAUDE.md`:

```
Quando scrivi un'email, un messaggio o una presentazione per me, leggi sempre prima il file ~/.claude/STYLE.md e scrivi con quel tono.
```

**Chiedi conferma esplicita prima di modificare il file.** Solo dopo il suo ok, aggiungi l'istruzione. Poi spiega cosa è cambiato: da adesso, ogni volta che gli chiede di scrivere qualcosa, Claude va prima a leggere il suo modo di scrivere.

### Chiusura

Riepiloga cosa ha ottenuto: il file `STYLE.md`, dove sta, e che è già collegato. Digli che può sempre tornare a migliorarlo aggiungendo nuovi esempi quando nota che una cosa non suona come lui. Ricordagli che lo stile cresce con l'uso: questa è solo la versione 1.

---

## Note

- Lo `STYLE.md` vive in `~/.claude/` (globale), quindi vale per tutto quello che scrivi, con qualsiasi cliente o progetto.
- Non è scolpito nella pietra: più lo usi, più lo affini. Quando un'email non suona come te, aggiungi quell'esempio e dillo a Claude.
- Il `CLAUDE.md` dice **chi sei**, lo `STYLE.md` dice **come scrivi**. Due schede dello stesso collaboratore.
