# Quadern de Notes

Aplicació web senzilla per calcular i exportar notes de classe per trimestre.
Pensada per a professorat de secundària: dones d'alta els alumnes, defineixes
les categories i pesos de cada trimestre (exàmens, treballs, actituds...), i
l'aplicació calcula automàticament la nota ponderada i el nivell (AE/AN/AS/NA)
de cadascú.

Funciona íntegrament al navegador — **no hi ha cap servidor ni base de
dades**. Cada persona que hi entra treballa amb les seves pròpies classes,
desades localment al seu ordinador.

## Funcionalitats

- Alumnes i categories il·limitats, configurables trimestre a trimestre (noms
  i pesos lliures).
- Categories que **no computen** a la nota (per exemple "Apunts": es demanen i
  es puntuen, però no compten per a la mitjana).
- Gestió de "NP" (no presenta): compta com un 0 en el càlcul.
- Nota final de curs amb pesos configurables per trimestre.
- Exportació a **PDF** (per trimestre, nota final, o un resum complet amb tots
  els trimestres en una sola taula) i a **Excel** (.xlsx amb un full per
  trimestre).
- Desar/obrir classes com a fitxers `.json`, amb sobreescriptura directa (sense
  duplicats) i un desplegable de "classes recents" si obres una carpeta
  sencera.
- Instal·lable com a aplicació (PWA): un cop allotjada, Chrome permet
  "instal·lar-la" com si fos un programa normal, amb icona pròpia.
- Tot en català, sense necessitat de compte ni de connexió (excepte per
  carregar la tipografia i la llibreria d'Excel la primera vegada).

## Com fer-la servir

1. **Classe**: posa el nom, el curs, el professor/a i el centre.
2. **Alumnes**: dona'ls d'alta un per un.
3. **1r / 2n / 3r Trimestre**: per a cada trimestre, defineix les categories i
   el seu pes. Per exemple:

   | Categoria      | Pes  |
   |----------------|------|
   | Examen 1       | 60%  |
   | Treball        | 20%  |
   | Fitxa de classe| 12%  |
   | Apunts         | *no computa* |

   Introdueix les notes de cada alumne a la taula; la nota i el nivell
   (AE/AN/AS/NA) es calculen sols. Marca "NP" si un alumne no ha presentat
   una activitat concreta.
4. **Nota final**: defineix el pes de cada trimestre (per exemple 30% / 30% /
   40%) i obtens la nota final de curs de cada alumne. Si un trimestre encara
   no té notes, compta com un 0 (com en un full de càlcul normal) — la nota
   final pot variar quan l'acabis d'omplir.
5. **Exportar**: des de cada trimestre pots treure un PDF; des de "Nota
   final" pots exportar el PDF de notes finals, un **resum complet** (tots
   els trimestres en una taula), o tota la informació en un **Excel**.

### Exemple

A la carpeta [`examples/`](examples/) hi ha tres classes de mostra, amb noms i
notes inventades, llestes per obrir directament amb "📂 Obrir una classe":

- **`socials-3r-a-notes.json`** — classe completa amb els 3 trimestres
  omplerts, un cas de NP i una categoria marcada com a "no computa".
- **`matematiques-1r-b-notes.json`** — només el 1r trimestre té notes; útil
  per veure com es comporta la nota final quan encara falten trimestres.
- **`naturals-2n-c-notes.json`** — alumnes donats d'alta però sense cap
  categoria ni nota; per començar a provar-ho des de zero.

## Instal·lar-la com a aplicació (Chrome)

**Ordinador**: amb la pàgina oberta, cerca la icona d'instal·lar a la barra
d'adreces, o menú de tres punts → "Instal·la Quadern de Notes...".

## Important: les dades no es comparteixen

Publicar el codi a una URL pública no vol dir que les dades es comparteixin
entre persones ni entre ordinadors. Cada usuari treballa amb les seves pròpies
classes, desades al seu navegador i als fitxers `.json` que triï. Per fer
servir la mateixa classe en dos ordinadors, fes servir "Desa la classe" /
"Obrir una classe" (o una carpeta sincronitzada amb Google Drive/Dropbox) per
moure-la d'un lloc a l'altre.

## Avís

Aquesta aplicació es proporciona "tal com és", sense cap garantia. Pot
contenir errors de càlcul o de programació — revisa sempre les notes abans de
publicar-les oficialment.

## Llicència

Distribuïda sota la llicència MIT — lliure d'ús, còpia, modificació i
distribució. Vegeu [LICENSE](LICENSE).
