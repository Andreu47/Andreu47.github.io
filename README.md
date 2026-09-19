# DAM 1 · Digitalització aplicada

Web estàtica creada amb HTML, CSS i JavaScript, preparada per publicar-se amb GitHub Pages.

## Estructura del projecte

- `index.html`: portada, presentació de l'equip i índex dels workshops.
- `workshops/`: una pàgina independent per a cada workshop.
- `assets/css/base.css`: colors, tipografia i estils generals.
- `assets/css/navigation.css`: capçalera, menú i peu de pàgina.
- `assets/css/home.css`: portada, equip i índex de workshops.
- `assets/css/workshops.css`: estructura, taules i galeries dels workshops.
- `assets/css/responsive.css`: adaptació per a tauletes i mòbils.
- `assets/js/main.js`: menú per a mòbils i desplegable de workshops.
- `assets/img/`: fotografies i captures del projecte.

## Estructura de cada workshop

Cada pàgina està pensada com a suport per a una presentació oral:

1. **Resum:** tema i continguts treballats.
2. **Què hem après:** coneixements principals.
3. **Activitats:** preguntes i respostes.
4. **Captures:** contingut gràfic i evidències del treball.

El resum i els aprenentatges comparteixen la part superior de la pàgina. Les activitats apareixen a sota en una taula compacta.

## Com afegir preguntes

Dins de la taula d'activitats, duplica una fila `<tr>` i modifica les dues cel·les `<td>`:

- Primera cel·la: pregunta o activitat.
- Segona cel·la: resposta.

## Com afegir captures

1. Copia la imatge a la carpeta `assets/img/`.
2. Busca la secció `GALERIA` dins del workshop.
3. Substitueix un `capture-placeholder` per una imatge:

```html
<img src="../assets/img/nom-captura.png" alt="Descripció de la captura">
```

4. Modifica el text del `figcaption` per explicar què mostra.

## Visualització local

Obre `index.html` en un navegador o utilitza l'extensió Live Server de Visual Studio Code.

## Publicació a GitHub Pages

1. Puja aquesta carpeta a un repositori de GitHub.
2. Obre **Settings → Pages**.
3. A **Build and deployment**, selecciona **Deploy from a branch**.
4. Tria la branca `main`, la carpeta `/ (root)` i prem **Save**.
