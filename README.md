# Schede Palestra (versione statica)

Sito statico: `index.html` + `esercizi.json`. Nessun server, nessun login.

- **Archivio esercizi**: `esercizi.json`, comune a tutti. Per aggiornarlo modifica il file (anche dal sito GitHub) oppure, dall'app, Esercizi → Esporta JSON e incolla il risultato nel file.
- **Storico e modifiche personali**: salvati nel browser di ciascun dispositivo.
- Campi esercizio: `id`, `name`, `pattern` (squat, hinge, lunge, push_h, push_v, pull_h, pull_v, core, carry, cardio, arms), `equipment` (lista), `places` (palestra, casa, outdoor), `notes`, `desc` (descrizione), `reps` (ripetizioni AMRAP, es. `10`, `6+6`, `30"`), `img` (URL immagine https), `ref` (link ad altre immagini), `active`.
- Formati: intervalli (lavoro/recupero × stazioni × giri), AMRAP (blocchi di N minuti, più giri possibili, contatore giri), oppure entrambi.
- Immagini: dataset pubblico [free-exercise-db](https://github.com/yuhonas/free-exercise-db) (Unlicense); dove manca, link a una ricerca immagini.

Pubblicazione: GitHub → Settings → Pages → Deploy from branch `main` / root.
