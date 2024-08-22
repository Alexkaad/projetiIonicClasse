# projetiIonicClasse
Mini Projet Guidé
Par groupe de 2-3 personnes, ou en solo au choix (mais si solo, je conseil de vous mettre quand même dans une chat vocal avec d'autres gens pour vous entraider), créer une appli permettant de poster des messages géolocalisés consultables par tous les membres de la communautés.
 
Scénario d'utilisation 1 : Je lance l'application mobile, je vais sur la page de la carte qui se centre sur ma position actuelle, et sur la carte je peux voir des points autour de moi qui représentent les messages des personnes. Je clique sur un point et je peux voir le message. Si je le souhaite, à l'aide d'un dropdown ou autre, je peux sélectionner une catégorie de message pour n'afficher que ceux qui concernent par exemple des points d'intérêt lié au street art.
 
Scénario d'utilisation 2 : Je lance l'application mobile, je clique sur le bouton poster qui me permet d'entrer mon message, indiquer mon nom (ou laisser anonyme), choisir une catégorie parmis celles existantes, éventuellement prendre une photo, lorsque je valide, mon message est géolocalisé par mon appareil et il apparaîtra maintenant sur la carte là où j'ai fait le post.
 
Entités
On part sur une ou deux entités selon si vous êtes en groupe ou non : L'entité principale qui est le Post et l'entité secondaire Category
Dans la Post, on peut mettre l'image même si on ne s'en sert pas au final, juste bien la mettre nullable partout aussi bien dans le SQL, dans le PHP et dans le TS
 
Organisation
Faire 2 applications, une appli Symfony sous forme d'API REST et une appli Ionic Angular (avec un template ou non, selon s'il y en a un qui correspond à ce que vous voulez faire comme navigation)
 
Vous pouvez utiliser un ORM ou pas selon ce que vous souhaiter travailler, je ferai personnellement la "correction" sans ORM. Si pas d'ORM commencez par créer le fichier SQL avec les create tables et les insert into pour avoir des données de tests.
 
Je conseil de commencer par créer les entités pour avoir au moins cette base là, et ensuite travailler soit par couche  (repository -> controllers -> front end) soit par tranche/fonctionnalités (peut être plus intéressant pour être sûr de travailler un peu tout). Par fonctionnalité en gros on choisis une fonctionnalité à développer, et on commence par la partie qu'on veut, par exemple je commence à faire l'interface graphique jusqu'au point où j'ai besoin de faire un appel serveur, là je fais la route associée dans le contrôleur et la méthode du repository correspondante, et allez soyons fou, je fais aussi un test fonctionnel pour la route. Je m'en sers dans mon front et je continue comme ça jusqu'à ce que la fonctionnalité soit terminée puis je passe à une autre.
dam-grenoble-ionic-usecase.png
dam-grenoble-ionic-class.png
 

