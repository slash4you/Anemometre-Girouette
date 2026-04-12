# Anémomètre+Girouette
Projet de construction DIY d'un anémomètre et d‘ une girouette connectés à Home Assistant.
|                 DIY| |
|---|---|
| 100% imprimable (PETG ou ABS, TPU), compacte, autonome (solaire)  | ![Modèle 3D](https://github.com/slash4you/Anemometre-Girouette/blob/main/images/Anemometre+Girouette%20v399_3.png?raw=true "Modèle 3D")  |
| assemblage par visserie standard, colle au silicone (étanchéité de la boite de commande), colle cyanoacrylate (selon l‘ ajustement des queues d‘ arronde) |  ![Modèle 2D](https://github.com/slash4you/Anemometre-Girouette/blob/main/images/Anemometre+Girouette%20v400.png?raw=true "Modèle 2D") |
| composants low-cost, logiciel opensource, connectée, esphome ready |  ![Calculateur](https://github.com/slash4you/Anemometre-Girouette/blob/main/images/Anemometre%20Electronic%20v15_2.png?raw=true "Calculateur") |
|   modifiable, évolutive, sources partagées | ![PCB](https://github.com/slash4you/Anemometre-Girouette/blob/main/kicad/doc/PCB.png?raw=true "PCB")  |

## GitHub

Ce dépôt regroupe l‘ ensemble des données nécessaires à la construction de cet anémomètre, organisées de la façon suivante:
+ [fusion360](https://github.com/slash4you/Anemometre-Girouette/blob/main/fusion360) → contient le modèle 3D au format f3d
+ [bambustudio](https://github.com/slash4you/Anemometre-Girouette/blob/main/bambustudio) → contient le modèle d ‘impression au format 3mf
+ [stl](https://github.com/slash4you/Anemometre-Girouette/blob/main/stl) → contient le fichier de maillage de chaque composant au format stl
+ [esphome](https://github.com/slash4you/Anemometre-Girouette/blob/main/esphome) → contient la description du firmware au format yaml
+ [images](https://github.com/slash4you/Anemometre-Girouette/blob/main/images) → contient un ensemble d ‘ images du modèle et photos du prototype
+ [kicad](https://github.com/slash4you/Anemometre-Girouette/blob/main/kicad)  → contient la définition du PCB au format kicad et gerber

## Makerworld

Le projet d‘ impression correspondant est disponible ici:  [Anémomètre+Girouette](https://makerworld.com/fr/models/2154241) .

## Avancement

**NB: A ce stade le premier prototype n‘ est pas encore fonctionnel. Il est donc vivement recommandé d‘ attendre 
avant d‘ imprimer le modèle car plusieurs composants sont encore potentiellement modifiables.**

Il reste encore beaucoup de travail avant que ce projet soit utilisable sans trop d‘ efforts par tout un chacun. 
Le premier objectif est la mise au point d‘ un prototype fonctionnel (version beta du projet), avant de capitaliser les informations et 
formaliser la documentation indispensable à une diffusion plus large (version release du projet). 

Pour les impatients sachez que ce n ‘est pas l‘ envie qui fait défaut mais bien le temps... d‘ autant qu‘ il s‘ agit de ma première 
expérience en modélisation 3D, en conception de PCB, et que l‘ impression 3D est une expérience très récente. Toute aide est la 
bienvenue pour corriger, améliorer, tester.. bref partager.

Ci-après une estimation de l‘ état d‘ avancement des activités envisagées : 

### 1. Version beta: prototypage

- [ ]   95%  : modélisation de la structure mécanique
- [x] 100%  : approvisionnement des composants tierces
- [ ]   80%  : impression/assemblage de la structure mécanique
- [ ]   90%  : assemblage des composants électroniques ( panneau solaire + calculateur + batterie + CI )
- [ ]   80%  : développement du firmware du calculateur
- [ ]   50% : intégration des capteurs de mesure de l‘ anémomètre
- [ ]      0% : 🍾
- [ ]      0% : intégration des capteurs de mesure de la girouette
- [ ]      0% : 🍾
- [ ]      0% : tests en environnement réel
- [ ]      0% : 🎉
      
### 2. Version release: partage et support

- [ ]    0%  : étalonnage des mesures et optimisation de leur durée d‘ intégration
- [ ]    0%  : optimisation de la charge en fonction de l‘ ensoleillement, de la saison, de l‘ heure, ...
- [ ]    0%  : publication d‘ un profil d‘ impression makerworld « plug-and-play »
- [x] 100%  : documentation/schéma électronique/inventaire des composants électroniques
- [ ]    0%  : documentation/inventaire des composants mécaniques
- [ ]    0%  : documentation/tutoriel de montage

## Licence

L e projet est publié sous licence [Creative Commons Attribution-Noncommercial-Share Alike](https://github.com/slash4you/Anemometre-Girouette/blob/main/LICENSE.md).