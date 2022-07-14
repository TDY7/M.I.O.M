# *M.I.O.M*

## Description:

Le Mangeur Intelligent d'Ordures Ménagères soit M.I.O.M est une poubelle intelligente qui va s'ouvrir dès lors qu'une personne se rapproche de cette dernière. La personne en face va de ce fait pouvoir déposer ses détritus même en ayant les mains encombrées. Ce projet, sous la forme d'un personnage possédant une bouche et des yeux, est "M.I.O.M" (mi homme) mi robot.

## Fonctionnement:

Dès lors que le capteur à ultrason va détecter la présence d'un objet ou d'une personne à proximité de M.I.O.M, le servomoteur va pivoter d'environ 90 degrés pour tirer légèrement la ficelle reliée à un trombone situé de l'autre côté du couvercle afin de faire basculer ce dernier, ce qui va éclairer la led et permettre l'ouverture du couvercle cartonné. Afin de garder un suivi de son utilisation, une notification est reçue sur le téléphone à chaque ouverture de la poubelle, informant ainsi la personne de son usage.

## Montage:

### Pour ce qui concerne le montage électronique

Tout d'abord, il fallait relier le capteur à ultrason à la carte arduino grâce à des cables, pour ce faire j'ai utilisé un premier cable pour relier le Vcc du capteur à ultrason au 5v de la carte arduino UNO ensuite le Trig à la borne 9 de la carte puis Echo à la borne 8 et pour finir le GND du capteur à ultrason au GND de la carte arduino UNO. Maintenant que notre carte arduino UNO et notre capteur à ultrason sont reliés, nous pouvons nous occuper du micro servo. J'ai donc relié la première entrée du servo à la borne 7 de la carte, la deuxième au 5v de la carte et la dernière au GND de la carte. Nous pouvons maintenant rajouter la led aux bornes GND et 13 de notre carte arduino UNO. 
Le montage électronique terminé, j'ai téleversé mon code sur la carte arduino UNO.

### Pour ce qui concerne le montage de M.I.O.M

J'ai pris soin d'acheter deux poubelles de deux tailles différentes, la poubelle la plus grande servant uniquement pour l'esthétique (cacher les composants du montage électronique qui se trouvent sur les parois de la petite poubelle).

#### Pour la petite poubelle:
Pour la conception du couvercle, j'ai pris une feuille cartonnée blanche sur laquelle j'ai tracé le contour du diamètre supérieur de la poubelle que j'ai ensuite coupé en deux, puis scotché les deux demi-cercles côte à côte tout en laissant un petit espace entre eux (ce qui permettra de faciliter l'ouverture de la poubelle).
Par la suite, j'ai percé l'un des deux demi-cercles (qui servira pour le rabatement) à l'aide d'un trombone pour y faire glisser un fil (de la face extérieure à intérieure). J'ai raccroché le fil à un trombone sur la face intérieure du demi-cercle. J'ai rejoint l'autre bout du fil à l'hélice du servomoteur puis fait un noeud de manière à ce que la longueur du fil permette l'ouverture et la fermeture du demi-cercle sur la poubelle.

#### Pour la grande poubelle:
J'ai conçu et imprimé une feuille A3 que j'ai redimensionné puis découpé pour l'adapter aux formes de la poubelle. Pour le couvercle, j'ai tracé le diamètre supérieur de la poubelle à l'intérieur duquel j'ai traçé le cercle correspondant à la taille du couvercle de la petite poubelle. J'ai ensuite découpé l'intérieur du tracé du petit couvercle de manière à pouvoir placer la petite poubelle dans la grande sans la gênance du couvercle de la grande poubelle. Pour finir, j'ai eu besoin de faire plusieurs trous sur les côtés de la grande poubelle, deux pour y faire passer le capteur à ultrason, un pour y glisser la LED et un dernier pour faire passer le cable qui sera rattaché à l'ordinateur. Pour cela, j'ai utilisé une perceuse.

## Matériel utilisé:

- Carte arduino UNO R3
- Capteur à ultrason HC-Sr04
- Micro Servo SG90 9G
- Cables
- 1 Led
- 1 Trombone
- 1 Ficelle
- 1 Petite poubelle
- 1 Grosse poubelle

## Schéma du montage électronique:
![Schema_M I O M](https://user-images.githubusercontent.com/103646329/172897034-52f10820-697f-4ee3-bbc4-f27be2aa0730.jpg)

## Visuel principal de la poubelle:
![Affiche-M I O M](https://user-images.githubusercontent.com/103646329/175002147-3dcea911-ce37-4e03-b085-57e18e28b94d.jpg)

Sans oublier le matériel visible par dessus l'affiche:
- Le capteur à ultrason se trouve au niveau des ronds blancs pour que cela puisse ressembler à des yeux.
- Une led se situe au dessus du I de M.I.O.M et s'éclaire lorsque la poubelle s'ouvre.

## Visuel final de M.I.O.M:
![MIOM_face](https://user-images.githubusercontent.com/103646329/175829824-02bf90fe-bf2a-4f62-b118-a1af6a07f23a.jpg)
![MIOM_dessus](https://user-images.githubusercontent.com/103646329/175829828-d70d33b5-0d70-402d-8fc0-c54b49478a32.jpg)
