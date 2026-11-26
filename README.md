# Schede Palestra (versione statica)

Sito statico: `index.html` + `esercizi.json`. Nessun server, nessun login.

- **Archivio esercizi**: `esercizi.json`, comune a tutti. Per aggiornarlo modifica il file (anche dal sito GitHub) oppure, dall'app, Esercizi → Esporta JSON e incolla il risultato nel file.
- **Storico e modifiche personali**: salvati nel browser di ciascun dispositivo.
- Campi esercizio: `id`, `name`, `pattern` (squat, hinge, lunge, push_h, push_v, pull_h, pull_v, core, carry, cardio, arms; `warmup` = riscaldamento a corpo libero, `mobility` = stretching/mobilità), `equipment` (lista), `places` (palestra, casa, outdoor), `notes`, `desc` (descrizione), `reps` (ripetizioni AMRAP, es. `10`, `6+6`, `30"`), `img` (URL immagine https), `ref` (link ad altre immagini), `active`.
- Struttura scheda: riscaldamento (5-15 min: macchina cardio tra quelle selezionate, esercizi `warmup` da 50s+10s, o metà e metà) → parte centrale → stretching e mobilità (5-15 min, intervalli 30s + 10s di cambio; usa esercizi `mobility` se presenti, altrimenti solo timer).
- Parte centrale: stazioni (N stazioni × esercizi per stazione × ripetizioni della stazione, modificabili per singola stazione nella scheda), AMRAP (blocchi di N minuti, più giri possibili, contatore giri), oppure entrambi.
- Immagini: dataset pubblico [free-exercise-db](https://github.com/yuhonas/free-exercise-db) (Unlicense); dove manca, link a una ricerca immagini.

Pubblicazione: GitHub → Settings → Pages → Deploy from branch `main` / root. A ogni modifica di `index.html` aggiorna `APP_VERSION`: le pagine già aperte o in cache la confrontano con quella pubblicata e si ricaricano da sole.
