
# Installation

## 1 - Commandes
`npm init -y `<br>
`npm install -D tailwindcss postcss-cli autoprefixer`<br>
`npx tailwind init`<br>

## 2 - Créer 
`postcss.config.js`

## 3 - Y ajouter  
```
module.exports = {
    plugins: [
        require('tailwindcss'),
        require('autoprefixer'),
    ]
}
```

## 4 - Dans le package.json 
    ``"build": "postcss css/tailwind.css -o public/tailwind.css"``



Pour ajouter @tilwind rule pour éviter le bug
https://stackoverflow.com/questions/47607602/how-to-add-a-tailwind-css-rule-to-css-checker