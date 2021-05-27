
# Installation

## 1 - Commandes
`npm init -y `<br>
`npm install -D tailwindcss postcss-cli autoprefixer`<br>
`npx tailwind init`<br>
`npx tailwindcss init -p`


## 2 - Dans le package.json 
``"build": "postcss css/tailwind.css -o public/tailwind.css"``


## 3 - Purge
Dans tailwind.config : './public/index.html',
Run : $env:NODE_ENV="production",
Run : npm run build

## 4 - Textension
Tailwind CSS IntelliSense

Pour ajouter @tilwind rule pour éviter le bug
https://stackoverflow.com/questions/47607602/how-to-add-a-tailwind-css-rule-to-css-checker