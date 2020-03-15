git init 
git config credential.helper store

// Mettre les sources changés en stages
git commit -m "init"

git remote add origin https://github.com/coquelicoop/produits.git
git push -u origin master


Le package odoo doit être cité avec son path absolu dans package.json
  "dependencies": {
    "@quasar/extras": "^1.0.0",
    "csv-parser": "^2.3.2",
    "csv-writer": "^1.6.0",
    "electron-rebuild": "^1.0.0",
    "jimp": "^0.9.3",
    "odoo": "file:c:/git/odoo-0.4.1.tgz",
    "quasar": "^1.8.5"
  },
sinon on ne build pas.

Donc problème : rectifier package.json selon le host où on build
