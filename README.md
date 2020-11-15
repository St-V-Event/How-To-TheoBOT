# Use ThéoBOT Verheagen

* ThéoBOT a été réfléchi pour offrir un maximum de possibilitées en changeant plusieurs paramètres pour le mieux convenir à vos situations lors du live. Il y a 3 status/role sur le serveur qui permettent certains privilèges : 
	* <kbd>admin CERCLE</kbd> : Cette personne aura le contrôle sur toutes les commandes cité ci-dessous. Le premier admin du cercle doit être ajouté manuellement par la "Team Orga", ensuite le rôle peut-être attribué à d'autres via une commande. ATTENTION ! Ne donnez pas ce privilège à n'importe qui ! Il aura tout pouvoir sur votre section Discord !
	* <kbd>streameur CERCLE</kbd> : Cette personne a le droit à 2 commandes supplémentaires par rapport aux autres (admin l'a aussi) et peu également rejoindre certaines conversations privées pour pouvoir s'isoler lors de la diffusion de votre programme (et évitez les intrusions de troll)
	* <kbd>CERCLE</kbd> : Le rôle peu être (et doit être fait pour tout le monde ! Pas ajoutable avec une commande.) auto-attribuer grâce à un autre BOT présent sur le serveur. Dans la conversation "🔺-your-circle-🔵" vous pourrez sélectionner celui que vous représentez !

* À aucun moment il ne vous est dit de mentionner votre cercle. C'est normal car le robot détecte automatiquement dans quelle "section Discord" (un rassemblement de conversations écrites et vocales) vous avez les droits. À savoir celle portant le nom de votre cercle bien-sûr. TOUT ce que vous ferez via ces commandes ne s'appliquera que dans votre section, peu importe où vous l'écrivez (je vous recommande cependant de le faire dans le channel 🤖-bot-command pour minimiser les chances de conflits de permissions) !

* Dû à ces status, plusieurs "catégories/sections" de conversations privées sont possible. Il faut comprendre que sur Discord on peu créer autant de conversation qu'on veut sur le même serveur et en accorder le droit seulement à certaines personnes/certains rôles ! Pour vous faciliter la tâche à privatiser ces conversations plusieurs commandes sont possible, mais il faut bien choisir quel type de channel vous voulez créer ! Si vous vous ratez, pas très grâve.. supprimez et recommencez ! 

## Table des matières

* -help
* -create-text-chan [SECTION] [NAME_CHANNEL] [if commune : CERCLES]
* -delete-text-chan [#NAME_CHANNEL]
* -create-vocal-chan [SECTION] [NAME_CHANNEL] [if commune : CERCLES]
* -delete-vocal-chan [NAME_CHANNEL]
* -add-member [NAME_CHANNEL] [Members]
* -delete-member [NAME_CHANNEL] [Members]
* -add-role [ROLE] [Members]
* -delete-role [ROLE] [Members]
* -add-vieux [Member]
* -delete-vieux [Member]

<img title="" src=".\ress4how-to\Diagramme de volonté.PNG" alt="" width="750">

### -help [COMMANDE]
* Non ce n'est pas pour appeler de l'aide malheureusement.. Si vous tapez cette commande, le robot vous répondra en vous listant toutes les commandes (et peut-être d'autres cachées ?) cité dans ce document, mais direct sur Discord !

* COMMANDE
	* Si vous voulez en savoir plus sur une commande particulière, il faut copier/coller à côté de "-help" la commande voulu.

## Manage channels

### -create-text-chan [SECTION] [NAME_CHANNEL] [if commune : CERCLES]

* SECTION
	* <kbd>main</kbd> : accesible par tout le monde sur le serveur !
	* <kbd>private</kbd> : accesible par les membres du cercle (qui l'ont choisi dans la conv 🔺-your-circle-🔵 du serveur, donc en soi tout le monde peu lire en se donnant le role ! Rappelez-vous s'en !)
	* <kbd>commune</kbd> : accesible par les membres du cercle, et de membres des cercles mentionné à la place de [CERCLES]
	* <kbd>stream</kbd> : accesible par les pocesseur du rôle "streameur CERCLE"
	* <kbd>stream-commune</kbd> : accesible par les pocesseur du rôle "streameur CERCLE" et les streameurs des autres cercles mentionné à l'emplacement [CERCLES]
	* <kbd>sondage</kbd> : accesible par tout le monde, mais personne ne peu écrire à part les admin ! Vous devez également ajouter les réactions voulu pour votre sondage, les autres personnes ne le peuvent pas (pour pas que ça parte en zbeul). Vous pouvez l'utiliser comme channel "d'annonces" aussi par exemple.
	* <kbd>vieux</kbd> : accesible pour personne de base. Pas même les admin. Il faudra entrer la commande "add-vieux" pour les y ajouter.

* NAME_CHANNEL
	* Le nom que vous souhaitez donner à cette nouvelle conversation. Le robot ajoutera un smiley correspondant à la section. ATTENTION ! Le robot n'aime pas les espaces ! Il faut remplacer ceux-ci par un tiret : "-" !!

* CERCLES
	* Identifiez le.s cercle.s que vous souhaitez ajouter à la conversation en commençant par un "@" il vous suggèrera des cercles au fur et à mesure que vous écrivez.

* EXEMPLE
<img title="" src=".\ress4how-to\-create-text-chan.png" alt="" width="500">

### -delete-text-chan [NAME_CHANNEL]

* NAME_CHANNEL
	* Vous devez réécrire le nom de la conversation SCRUPULEUSEMENT ! Il faut respecter les majuscules et minuscules et les espaces en tiret. Par contre ne tenez pas compte du Smiley ajouté au début, le robot l'ajoutera tout seul dans sa recherche.

* EXEMPLE
<img title="" src=".\ress4how-to\-delete-text-chan.png" alt="" width="400">

### -create-vocal-chan [SECTION] [NAME_CHANNEL] [if commune : CERCLES]

* SECTION
	* <kbd>main</kbd> : accesible par tout le monde sur le serveur !
	* <kbd>private</kbd> : accesible par les membres du cercle (qui l'ont choisi dans la conv 🔺-your-circle-🔵 du serveur, donc en soi tout le monde peu lire en se donnant le role ! Rappelez-vous s'en !)
	* <kbd>commune</kbd> : accesible par les membres du cercle, et de membres des cercles mentionné à la place de [CERCLES]
	* <kbd>stream</kbd> : accesible par les pocesseur du rôle "streameur CERCLE"
	* <kbd>stream-commune</kbd> : accesible par les pocesseur du rôle "streameur CERCLE" et les streameurs des autres cercles mentionné à l'emplacement [CERCLES]
	* <kbd>vieux</kbd> : accesible pour personne de base. Pas même les admin. Il faudra entrer la commande "add-vieux" pour les y ajouter.

* NAME_CHANNEL
	* Le nom que vous souhaitez donner à cette nouvelle conversation. Le robot ajoutera un smiley correspondant à la section. ATTENTION ! Le robot n'aime pas les espaces ! Il faut remplacer ceux-ci par un tiret : "-" !!

* CERCLES
	* Identifiez le.s cercle.s que vous souhaitez ajouter à la conversation en commençant par un "@" il vous suggèrera des cercles au fur et à mesure que vous écrivez.

* EXEMPLE
<img title="" src=".\ress4how-to\-create-vocal-chan.png" alt="" width="500">

### -delete-vocal-chan [NAME_CHANNEL]

* NAME_CHANNEL
	* Vous devez réécrire le nom de la conversation SCRUPULEUSEMENT ! Il faut respecter les majuscules et minuscules et les espaces en tiret. Par contre ne tenez pas compte du Smiley ajouté au début, le robot l'ajoutera tout seul dans sa recherche.
* EXEMPLE
<img title="" src=".\ress4how-to\-delete-vocal-chan.png" alt="" width="400">

## Manage People

### -add-member [NAME_CHANNEL] [Members]

* Cette commande permet d'ajouter une ou des personnes à une conversation privée. Pour éviter trop de commandes, celle-ci est combinée. Il faudra d'office une conversation écrite portant un nom X, cette personne y sera ajoutée. et si le robot trouve une conversation vocale portant également le nom X, elle y sera ajoutée également.
* Cette commande, ainsi que son delete, sont les 2 seules qu'une personne aillant le rôle "streameur" peut exécuter.

* NAME_CHANNEL
	* Réécrivez SCRUPULEUSEMENT le nom de la conversation écrite (et vocale du même nom, si elle existe) en évitant les espaces.

* Members
	* Il faut "identifier" (comme quand on identifie une personne sur les réseaux), les personnes que vous souhaitez ajouter. Grâce au "@" suivit du pseudo de la personne.

* EXEMPLE
<img title="" src=".\ress4how-to\-add-member1.png" alt="" width="400">
<img title="" src=".\ress4how-to\-add-member2.png" alt="" width="500">

### -delete-member [NAME_CHANNEL] [Members]

* Cette commande permet de supprimer une ou des personnes à une conversation privée. Pour éviter trop de commandes, celle-ci est combinée. Il faudra d'office une conversation écrite portant un nom X, cette personne y sera ajoutée. et si le robot trouve une conversation vocale portant également le nom X, elle y sera ajoutée également.
* Cette commande, ainsi que son add, sont les 2 seules qu'une personne aillant le rôle "streameur" peut exécuter.

* NAME_CHANNEL
	* Réécrivez SCRUPULEUSEMENT le nom de la conversation écrite (et vocale du même nom, si elle existe) en évitant les espaces.

* Members
	* Il faut "identifier" (comme quand on identifie une personne sur les réseaux), les personnes que vous souhaitez ajouter. Grâce au "@" suivit du pseudo de la personne.

* EXEMPLE
<img title="" src=".\ress4how-to\-delete-member1.png" alt="" width="400">
<img title="" src=".\ress4how-to\-delete-member2.png" alt="" width="500">

### -add-role [ROLE] [Members]

* Cette commande permet d'attribuer un rôle aux personnes identifiées.
	
* ROLE
	* <kbd>admin</kbd> : permet d'éxécuter toutes les commandes cité dans ce document, ne confiez pas ce rôle à n'importe qui !
	* <kbd>stream</kbd> : permet l'accès aux conversations réservé aux streameurs.

* Members
	* Il faut "identifier" (comme quand on identifie une personne sur les réseaux), les personnes à qui vous souhaitez attribuer le rôle. Grâce au "@" suivit du pseudo de la personne.

* EXEMPLE
<img title="" src=".\ress4how-to\-add-role.png" alt="" width="400">

### -delete-role [ROLE] [Members]

* Cette commande permet d'enlever un rôle aux personnes identifiées.

* ROLE 
	* <kbd>admin</kbd> : permet d'éxécuter toutes les commandes cité dans ce document.
	* <kbd>stream</kbd> : permet l'accès aux conversations réservé aux streameurs.

* Members
	* Il faut "identifier" (comme quand on identifie une personne sur les réseaux), les personnes à qui vous souhaitez attribuer le rôle. Grâce au "@" suivit du pseudo de la personne.

* EXEMPLE
<img title="" src=".\ress4how-to\-delete-role.png" alt="" width="500">

## Vieux Cons

* ATTENTION : Vous vous rendrez compte lorsque vous irez sur ces conversation "vieux-cons", que la "Team Orga" a également accès à cette conversation. C'est indépendant de notre volonté pour tout dire.. C'est le cas pour TOUTES les conversations peu importe comment vous la créez ! C'est tout simplement parce-que nous avons les droits "Administrateur" du serveur, ce qui implique que, qu'on le veille ou non, nous aillons accès à TOUT. Cependant nous vous promettons de ne pas espionner ! Discutez l'esprit tranquille, pour tout vous dire on aura "mieux/plus important" à faire que de mater toutes les conversations hihihi. 

### -add-vieux [Member]

* Cette commande permet d'autoriser, UNE personne à la fois, l'accès aux channels vieux. Ces channels sont de base, bloquer pour tout le monde. Même un admin doit s'auto-ajouter à la conversation ! Cependant, elle ne reconnaitra que les conversations déjà présente sur le serveur. Si vous souhaitez créer d'autres conversations vieux il faudra utiliser la commande "add-member" pour les y ajouter.

* Member
	* Il faut "identifier" (comme quand on identifie une personne sur les réseaux), la personne à qui vous souhaitez autoriser l'accès. Grâce au "@" suivit du pseudo de la personne.

* EXEMPLES
<img title="" src=".\ress4how-to\-add-vieux1.png" alt="" width="400">
<img title="" src=".\ress4how-to\-add-vieux2.png" alt="" width="500">

### -delete-vieux [Member]

* Cette commande permet de supprimer, UNE personne à la fois, l'accès aux channels vieux. Elle ne pourra plus se connecter au channel textuel & vocal.
Cependant, elle ne reconnaitra que les conversations déjà présente sur le serveur. Si vous souhaitez créer d'autres conversations vieux il faudra utiliser la commande "delete-member" pour les en supprimer.

* Member
	* Il faut "identifier" (comme quand on identifie une personne sur les réseaux), la personne à qui vous souhaitez autoriser l'accès. Grâce au "@" suivit du pseudo de la personne.

* EXEMPLE
<img title="" src=".\ress4how-to\-delete-vieux1.png" alt="" width="400">
<img title="" src=".\ress4how-to\-delete-vieux2.png" alt="" width="500">
