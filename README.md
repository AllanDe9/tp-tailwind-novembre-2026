# TP Tailwind CSS

## Prérequis

- [Node.js](https://nodejs.org/) (avec `npm`)

## Installation

Depuis la racine du projet :

```bash
npm install
```

## Lancer et voir le projet

Il faut deux terminaux ouverts à la racine du projet.

**1. Compiler le CSS avec Tailwind (terminal 1)**

```bash
npm run tailwind
```

Cette commande génère `dist/style.css` à partir de `assets/styles/main.css`, puis surveille les fichiers : le CSS est
recompilé à chaque modification de `index.html` ou de `main.css`. Laissez ce terminal ouvert.

**2. Lancer le serveur local (terminal 2)**

```bash
npm run serve
```

Ouvrez ensuite l'adresse affichée dans le terminal (en général <http://localhost:3000>).

> Pour un simple aperçu sans serveur, vous pouvez aussi ouvrir `index.html` directement dans le navigateur, à
> condition que `dist/style.css` ait déjà été généré.

## Structure

- `index.html` : la page portfolio
- `assets/styles/main.css` : source Tailwind, avec les composants réutilisés (`btn`, `tag`, `project-card`…)
- `dist/style.css` : CSS généré par Tailwind (ne pas modifier à la main)

## En cas de problème

Si la page s'affiche sans style, vérifiez que `npm run tailwind` tourne bien dans un terminal et que
`dist/style.css` existe.
