
# Installation

## 1 - Commandes
**Run** : `npm init -y `<br>
**Run** : `npm install -D tailwindcss postcss-cli autoprefixer`<br>
**Run** : `npx tailwindcss init -p`

## 2 - Créer dossier et fichiers
public => index.html<br>
src => tailwind.css

## 3 - Dans tailwind.css
**Ajouter** 
```
@tailwind base;
@tailwind components;
@tailwind utilities;

@layer base {

}

@layer components {

}
```

## 3 - Build
**Ajouter** dans le package.json : script => ``"build": "postcss -w src/tailwind.css -o public/style.css"``<br>
**Run** : ``npm run build``

## 4 - Extension
**Installer** : *Tailwind CSS IntelliSense*<br>

## 5 - Purge
**Ajouter** dans tailwind.config.js : purge => `./public/index.html`<br>
**Run** : `$env:NODE_ENV="production"`<br>
**Run** : `npm run build`


Ajouter @tilwind rule pour éviter le bug
https://stackoverflow.com/questions/47607602/how-to-add-a-tailwind-css-rule-to-css-checker