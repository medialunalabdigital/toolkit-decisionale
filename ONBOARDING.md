# 🧠 Toolkit Decisionale — Guida rapida

*by Medialuna Lab*

Benvenuto/a. Questo toolkit aggiunge a Claude **10 "modalità di pensiero"** che ti aiutano a decidere meglio, smontare le idee deboli, difendere i tuoi piani e scrivere senza fuffa. Si usano scrivendo un comando (es. `/brutal`) seguito da ciò di cui vuoi parlare.

Installarlo richiede **2 minuti**. Segui il percorso giusto in base a come usi Claude.

---

## 🧭 Quale Claude usi?

| Se usi… | Vai al… |
|---|---|
| **App desktop Claude Code** (terminale / "/plugin") | **Percorso A** |
| **claude.ai** (sito web o app mobile) | **Percorso B** |

---

## 🅰️ Percorso A — Claude Code (1 minuto)

1. Apri Claude Code.
2. Scrivi questo e premi invio:
   ```
   /plugin marketplace add medialunalabdigital/toolkit-decisionale
   ```
3. Poi:
   ```
   /plugin install toolkit-decisionale@medialuna-marketplace
   ```
   *(usa il nome completo `@medialuna-marketplace`: quello "liscio" può non essere trovato.)*
4. Esci e rientra. Digita `/` → vedrai i 10 comandi. **Fatto.**

> 🔄 **Aggiornamenti:** quando rilasciamo migliorie, scrivi `/plugin update toolkit-decisionale@medialuna-marketplace`.

---

## 🅱️ Percorso B — claude.ai (web / app)

Su claude.ai i comandi `/` non si installano come plugin. Hai due modi (te ne consegniamo i file).

### Modo 1 — Skills *(piani Pro / Max / Team / Enterprise)*
1. Vai su **Impostazioni → Capabilities / Skills**.
2. **Carica** gli zip che ti abbiamo inviato (uno per comando, cartella `dist/`).
3. Pronto: i comandi si attivano scrivendo `/brutal …` **oppure** con una frase naturale (es. *"dimmi la verità su questa offerta"*).

### Modo 2 — Progetto *(funziona su tutti i piani, anche gratuito)*
1. Su claude.ai crea un **Progetto** e chiamalo *Toolkit Decisionale*.
2. Apri le **Istruzioni del progetto** e incolla il testo che ti abbiamo inviato (file `ISTRUZIONI-PROGETTO-claude-ai`).
3. Salva. In **ogni chat dentro quel Progetto** scrivi `/brutal …`, `/decidi …`, ecc.

---

## 🛠️ I 10 comandi

| Comando | Cosa fa |
|---|---|
| `/brutal` | Feedback senza filtri: ti dice la verità, niente complimenti di facciata. |
| `/steelman` | Costruisce l'argomento **più forte possibile** a favore di una tesi. |
| `/devil` | Avvocato del diavolo: attacca la tua idea per vedere se regge. |
| `/whatamimissing` | Trova i **punti ciechi**: rischi e assunzioni che non vedi. |
| `/premortem` | Immagina il progetto **già fallito** e dice perché, per evitarlo ora. |
| `/red-team` | Attacca offerta/piano come farebbe un **concorrente o cliente scettico**. |
| `/decidi` | Confronta le opzioni e **sceglie**, niente "dipende". |
| `/numeri` | Fa i **conti**: break-even, quanti clienti servono, margini. |
| `/scrivi-cattivo` | Copy **diretto e senza fuffa**, niente cliché né aziendalese. |
| `/elis` | Spiega un concetto **semplice come a un bambino**. |

---

## ▶️ Come si usano

Scrivi il comando seguito da ciò di cui vuoi parlare. Oppure scrivi solo il comando: lavorerà sull'ultima cosa di cui stavate parlando.

**Esempi:**
```
/brutal la mia offerta "gestione social a 800€/mese"
/decidi pacchetto unico a 1500€ oppure abbonamento a 300€/mese
/numeri voglio arrivare a 5.000€/mese di fatturato
/scrivi-cattivo una caption Instagram per lanciare il nuovo servizio
/elis cos'è il retargeting
```

💡 **Consiglio:** più dettagli dai, più la risposta è utile. Questi strumenti sono onesti per scelta — `/brutal` e `/red-team` ti diranno cose scomode. È voluto: servono a farti arrivare prima al punto.

---

*Problemi nell'installazione? Scrivici a medialuna.lab@gmail.com — ti aiutiamo noi.*
