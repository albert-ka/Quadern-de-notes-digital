# Quadern de Notes

Eina per calcular i exportar notes de classe per trimestre. Funciona íntegrament
al navegador — no hi ha cap servidor ni base de dades: cada persona que hi entra
té les seves pròpies classes, desades al seu propi ordinador.

## Allotjar-ho a GitHub Pages

1. Crea un repositori nou a GitHub (pot ser públic; amb GitHub Pages gratuït cal
   que ho sigui, tret que tinguis un pla de pagament).
2. Puja tots els fitxers d'aquesta carpeta (`index.html`, `manifest.json`,
   `sw.js`, `icon-192.png`, `icon-512.png`, `apple-touch-icon.png`,
   `favicon-32.png`) a l'arrel del repositori.
3. Ves a **Settings → Pages**.
4. A "Build and deployment", tria **Source: Deploy from a branch**, branca
   `main`, carpeta `/ (root)`. Desa.
5. Espera un minut i visita `https://<el-teu-usuari>.github.io/<nom-del-repo>/`.

## Instal·lar-la com a aplicació (Chrome)

**A l'ordinador:** amb la pàgina oberta a Chrome, cerca la icona d'instal·lar a
la barra d'adreces (una pantalla amb una fletxa cap avall, a la dreta de la
URL), o al menú de tres punts → **"Instal·la Quadern de Notes..."**. Un cop
instal·lada, s'obre en una finestra pròpia, amb icona a l'escriptori/menú
d'aplicacions, com si fos un programa normal.

**Al mòbil (Android/Chrome):** menú de tres punts → **"Afegir a la pantalla
d'inici"**.

## Actualitzar-la

Cada cop que vulguis publicar canvis, puja els fitxers actualitzats al mateix
repositori (`git add`, `git commit`, `git push`, o directament des de la web de
GitHub). GitHub Pages es actualitza sol al cap d'uns segons/minuts. La gent que
ja la tingui instal·lada rebrà la versió nova la següent vegada que l'obri amb
connexió a internet.

## Una cosa important: les dades no es comparteixen

Publicar el codi a una URL pública **no vol dir que les dades es comparteixin**
entre persones ni entre ordinadors. Cada persona que obre l'enllaç (o l'app
instal·lada) treballa amb les seves pròpies classes, desades localment al seu
navegador i als fitxers `.json` que ella mateixa triï. Si vols fer servir la
mateixa classe en dos ordinadors diferents, continua fent servir "Desa la
classe" / "Obrir una classe" (o la carpeta compartida, per exemple via Google
Drive/Dropbox sincronitzats) per moure-la d'un lloc a l'altre — exactament
igual que ja funciona ara.
