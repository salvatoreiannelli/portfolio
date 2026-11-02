# Sito di Salvatore Iannelli

Portfolio video. Pagina singola, nessun programma da installare, nessun database.

## Come pubblicarlo su GitHub Pages

1. Su GitHub crea un repository nuovo chiamato `portfolio`, **pubblico**, vuoto
   (niente README, niente .gitignore).
2. Apri il repository, clicca **Add file → Upload files**.
3. Trascina dentro **il contenuto** di questa cartella: `index.html`, `404.html`,
   `.nojekyll` e la cartella `img`. Non trascinare la cartella che li contiene.
4. Clicca **Commit changes**.
5. Vai su **Settings → Pages**. Alla voce *Source* scegli *Deploy from a branch*,
   ramo `main`, cartella `/ (root)`. Salva.
6. Dopo qualche minuto il sito è online su `https://TUOUTENTE.github.io/portfolio/`.

## Una cosa da cambiare appena il sito è online

Apri `index.html` e cerca `INDIRIZZO-DEL-SITO` (compare due volte, in cima al file).
Sostituiscilo con l'indirizzo vero, per esempio `tuoutente.github.io/portfolio`.
Serve solo per l'anteprima che appare quando mandi il link su WhatsApp o LinkedIn.

## Come aggiungere un video più avanti

Tutti i video stanno in un unico elenco dentro `index.html`, nel blocco che comincia
con `<script type="application/json" id="data">`. Ogni video è una riga con titolo,
anno, cliente, categoria, durata, link e nome della copertina.

Per aggiungerne uno servono due cose: copiare una riga esistente e modificarla,
e mettere la nuova copertina nella cartella `img` con lo stesso schema di nomi
(`cover-12-640.jpg` e `cover-12-1280.jpg`).

## Dominio personalizzato

Quando compri un dominio, si collega da **Settings → Pages → Custom domain**.
Da quel momento il sito risponde all'indirizzo del dominio e il nome `portfolio`
sparisce dall'URL: chi apre il vecchio indirizzo viene rimandato al dominio.
L'unica cosa da aggiornare è `INDIRIZZO-DEL-SITO` qui sopra.
