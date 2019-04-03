Aller à l'URL "about:profiles"

OU

Clic sur : Menu > Aide > Informations de dépannage.
Dans le 1er tableau "Paramètres de base de l’application" :
Dernière ligne "Profils" : Clic sur "about:profiles".

Dans le "répertoire racine" (par exemple : /home/plaxton/.mozilla/firefox/67ter0vq.default ) :
Créer le répertoire `chrome`;
Dans ce répertoire :
Ajouter un fichier CSS :

`userChrome.css`
```
#titlebar {
   position: fixed !important;
   top: 1000000000px !important;
}
```

Redémarrer Firefox

Pour trouver les styles : 
Activer le débuggage de l'interface de firefox :
`Ctrl` + `Shift` + `i`
Clic sur `...` puis `Paramètres`
Dans la section "Paramètres avancés" (en bas à droite):
Cocher les 2 dernières cases "Activer le débogage du chrome du navigateur et des modules" et "Activer le débogage distant".

Puis clic sur : Menu > Développement web > Boîte à outils du navigateur (répondre "OK")
Et là vous avez la même console JS que pour le contenu des pages, mais ça regarde la fenêtre de firefox.
