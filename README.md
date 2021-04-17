L'application produits est passé en quasar 2.

Ceci a entrainé des modifications de configuration, comme décrit dans la page de migration
de quasar pour passer de 1 à 2.

electron est resté en 9 : au delà de cette version "remote" est deprecated ce qui impose de revoir :
- config.js

ce qui pour l'instant n'est pas indispensable.

Le builder est désormais electron-builder et non plus packager.
Ceci a changé dans quasar.conf.js la section corresponde pour gérer une production AppImage.

Sous windows la cible est 'portable'.
Sous linux la cible est 'AppImage' ou 'deb' - Faire le build SOUS LA MEME VERSION de Linux (18.04 ou 20.04) que l'exploitation.

Test : quasar dev -m electron
Build : quasar build -m electron
