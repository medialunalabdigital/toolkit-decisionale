# 🧠 Toolkit Decisionale — by Medialuna Lab

10 comandi per **pensare meglio** dentro Claude Code: ti aiutano a decidere, smontare le idee deboli, difendere i piani, validare coi numeri e scrivere senza fuffa.

## I comandi

| Comando | Cosa fa |
|---|---|
| `/brutal` | Feedback brutalmente onesto, zero compiacenza. Smonta l'idea e dice la verità. |
| `/steelman` | Costruisce la versione più forte possibile di una tesi, anche scomoda. |
| `/devil` | Avvocato del diavolo: argomenta contro la tua posizione per testare quanto regge. |
| `/whatamimissing` | Trova i punti ciechi: assunzioni nascoste, rischi fuori dal radar, effetti di secondo ordine. |
| `/premortem` | Immagina il progetto già fallito e ricostruisce il perché, per evitarlo ora. |
| `/red-team` | Attacca il piano come farebbe un concorrente o un cliente scettico, poi ti dà la difesa. |
| `/decidi` | Confronto onesto tra opzioni e raccomandazione netta. Niente "dipende". |
| `/numeri` | Valida un'idea coi conti: break-even, quanti clienti servono, margini, scenari. |
| `/scrivi-cattivo` | Copy diretto e senza fronzoli: vende senza cliché né aziendalese. |
| `/elis` | Spiega un concetto come a un bambino: semplice, chiaro, comprensibile a chiunque. |

Tutti accettano un argomento opzionale (es. `/decidi pacchetto unico vs abbonamento mensile`) oppure lavorano sull'ultima cosa discussa nella chat.

---

## 📦 Installazione (per il cliente)

> Richiede **Claude Code** (app desktop o CLI). Questi comandi **non** funzionano sul sito web claude.ai.

### Opzione 1 — Via marketplace (consigliata, si aggiorna da sola)

Dentro Claude Code digita:

```
/plugin marketplace add medialunalabdigital/toolkit-decisionale
/plugin install toolkit-decisionale
```

> Se il repo è privato, il cliente deve avere accesso (essere invitato come collaboratore) e `gh`/git autenticato.

Quando esci e rientri, digita `/` e vedrai i 10 comandi. Quando Medialuna aggiorna il toolkit, basta `/plugin update toolkit-decisionale`.

### Opzione 2 — Copia manuale (senza GitHub)

1. Scarica la cartella `plugins/toolkit-decisionale/commands/`.
2. Copia i 10 file `.md` in:
   - **Windows:** `C:\Users\<nome>\.claude\commands\`
   - **Mac/Linux:** `~/.claude/commands/`
3. Riavvia Claude Code → digita `/` → ci sono.

---

## 🌐 Usarlo su claude.ai (web / app)

Su claude.ai gli slash command non esistono. Ci sono due modi per avere lo stesso comportamento:

### Modo 1 — Skills (cross-platform, consigliato su piani Pro/Max/Team/Enterprise)

Le stesse capacità sono impacchettate come **Skills** in `plugins/toolkit-decisionale/skills/`. Le Skills funzionano sia su Claude Code sia su claude.ai e si attivano quando l'utente scrive il comando (es. `/brutal`) **o** una frase corrispondente (es. "dimmi la verità su questa offerta").

Per caricarle su claude.ai: **Impostazioni → Capabilities/Skills → carica** la skill (zip della cartella). In `dist/` trovi uno zip pronto per ognuna.

### Modo 2 — Progetto con istruzioni (funziona su tutti i piani)

1. Su claude.ai crea un **Progetto** "Toolkit Decisionale".
2. Apri le **Istruzioni del progetto** e incolla il contenuto di [`claude-ai/ISTRUZIONI-PROGETTO-claude-ai.md`](claude-ai/ISTRUZIONI-PROGETTO-claude-ai.md) (la parte dopo "ISTRUZIONI").
3. Salva. In ogni chat di quel Progetto scrivi `/brutal ...`, `/decidi ...`, ecc.

> Differenza: i comandi (Claude Code) sono globali e si digitano `/nome`; le Skills si attivano da sole quando "calzano" e valgono ovunque; il Progetto vale solo dentro quel Progetto.

---

## 🛠️ Per chi pubblica il plugin (Medialuna)

1. Crea un repo GitHub (anche privato) e carica **tutto il contenuto di questa cartella** mantenendo la struttura:
   ```
   .claude-plugin/marketplace.json
   plugins/toolkit-decisionale/.claude-plugin/plugin.json
   plugins/toolkit-decisionale/commands/*.md
   README.md
   ```
2. Comunica ai clienti il percorso `utente/repository` da usare in `/plugin marketplace add`.
3. Per aggiornare un comando: modifica il `.md`, aumenta `version` in `plugin.json`, fai `git push`. I clienti aggiornano con `/plugin update`.

---

*Toolkit Decisionale v1.0.0 — Medialuna Lab*
