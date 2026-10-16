# Calculadora Assignació de Diputats - Província de València (Llei d'Hondt)

Aquesta aplicació web interactiva permet simular i calcular el repartiment de diputats de la província de València utilitzant el **sistema d'Hondt** (Llei d'Hondt), tant per a les **Eleccions Generals** (16 diputats al Congrés) com per a les **Eleccions Autonòmiques** (40 diputats a les Corts Valencianes).

## 🚀 Característiques i Funcionalitats

- **Totalment Editable:** Modifica el nom de qualsevol partit o el seu nombre de vots en temps real.
- **Gestió Dinàmica:** Afegeix nous partits o elimina'ls fàcilment.
- **Paràmetres Configurables:** Ajusta el nombre de diputats totals a repartir i la barrera electoral (ex. 3% per a la LOREG / Generals, 5% per a Corts Valencianes).
- **Preset de Dades Reals:** Botons per a carregar instantàniament els resultats reals de la província de València (Generals 2023 i Corts Valencianes 2023).
- **Visualització Pas a Pas:** Taula detallada de matriu de quocients ($Vots / 1, Vots / 2, dots$) marcant clarament quins quocients han obtingut escó.
- **Hemicicle Parlamentari Visual:** Representació gràfica semiactiva en format d'arc parlamentari dels escons assignats.
- **Interfície Moderna:** Disseny clean, responsive i adaptable en valencià utilitzant Tailwind CSS.

---

## 🛠️ Com publicar aquesta web a GitHub Pages pas a pas

Si vols publicar aquesta mateixa aplicació al teu compte de GitHub Pages (com l'exemple `https://el-teu-usuari.github.io/hont-valencia/`), segueix aquests senzills passos:

### Pas 1: Crear un compte i un nou repositori
1. Accedeix a [GitHub.com](https://github.com) i inicia sessió (o crea un compte gratuït).
2. Fes clic al botó **"New"** (o en el signe **+** a dalt a la dreta -> **New repository**).
3. Nom del repositori: **`hont-valencia`** (o el nom que penses adequat).
4. Assegura't que estiga marcat com a **Public**.
5. Fes clic en **"Create repository"**.

### Pas 2: Creació dels fitxers del projecte
1. Dintre del teu repositori, fes clic en **"uploading an existing file"** o crea un fitxer prement **"creating a new file"**.
2. Anomena el fitxer principal com **`index.html`** i enganxa-hi el codi font HTML d'aquesta aplicació.
3. Crea un segon fitxer anomenat **`README.md`** i enganxa-hi aquest text explicatiu.
4. Fes clic en el botó verd **"Commit changes"** a la part inferior per desar els canvis.

### Pas 3: Activar GitHub Pages
1. Dins del repositori, ves a la pestanya **Settings** (Configuració) de la barra superior.
2. Al menú lateral esquerre, selecciona la secció **Pages**.
3. En la secció **"Build and deployment"** -> **Source**, tria **"Deploy from a branch"**.
4. Sota **Branch**, selecciona **`main`** (o `master`) i la carpeta **`/(root)`**.
5. Fes clic en **Save** (Guardar).

### Pas 4: Veure la teua aplicació en línia
En un parell de minuts, GitHub processarà el fitxer i t'oferirà una URL pública amb aquest format:
👉 `https://el-teu-usuari.github.io/hont-valencia/`

---

## 📐 Com funciona el Sistema D'Hondt?

1. **Filtre / Barrera Electoral:** S'eliminen aquelles candidatures que no superen el percentatge mínim establit (per exemple el 3% o 5% sobre el total de vots vàlids a candidatures).
2. **Càlcul de Quocients:** Els vots de cada candidatura restant es dividesixen successivament per $1, 2, 3, 4, dots$ fins al nombre total d'escons a repartir.
3. **Assignació:** Els escons s'atribueixen a les candidatures que obtinguen els quocients més grans en ordre decreixent.

---
*Projecte desenvolupat per a la simulació de resultats electorals a la Província de València.*
