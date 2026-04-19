# Anémomètre+Girouette
Projet de construction DIY d'un anémomètre et d‘ une girouette connectés à Home Assistant.

|  | DIY | |
|--|---------------------------------------|----------------------------------------------------------|
| ![Imprimante 3D]( https://github.com/slash4you/Anemometre-Girouette/blob/main/images//imprimante-3d.png?raw=true "Imprimante 3D" ) | 100% imprimable (PETG ou ABS, TPU), compacte, alimentation par batterie 18650 au Lithium (3800mAh) , recharge par panneau solaire (2W), mesure de la vitesse du vent par capteur à effet hall, mesure de la direction du vent (en cours)  | ![Modèle 3D](https://github.com/slash4you/Anemometre-Girouette/blob/main/images/Anemometre+Girouette%20v399_3.png?raw=true "Modèle 3D")  |
|  | assemblage par visserie standard, colle au silicone (étanchéité de la boite de commande), colle cyanoacrylate (selon l‘ ajustement des queues d‘ arronde) |  ![Modèle 2D](https://github.com/slash4you/Anemometre-Girouette/blob/main/images/Anemometre+Girouette%20v400.png?raw=true "Modèle 2D") |
|  | composants low-cost, firmware opensource, connection WIFI au serveur domotique, esphome ready, optimisation de l‘ autonomie |  ![Calculateur](https://github.com/slash4you/Anemometre-Girouette/blob/main/images/Anemometre%20Electronic%20v15_2.png?raw=true "Calculateur") |
|  |   conception modifiable, évolutive, toutes les données partagées, personnalisable à volonté | ![PCB](https://github.com/slash4you/Anemometre-Girouette/blob/main/kicad/doc/PCB.png?raw=true "PCB")  |

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

NB : A ce stade le premier prototype n‘ est pas encore fonctionnel. Il est donc vivement recommandé d‘ attendre 
avant d‘ imprimer le modèle car plusieurs composants sont encore potentiellement modifiables.

Il reste encore beaucoup de travail avant que ce projet soit utilisable sans trop d‘ efforts par tout un chacun. 
Le premier objectif est la mise au point d‘ un prototype fonctionnel (version beta du projet), avant de capitaliser les informations et 
formaliser la documentation indispensable à une diffusion plus large (version release du projet). 

> Pour les impatients sachez que ce n ‘est pas l‘ envie qui fait défaut mais bien le temps... d‘ autant qu‘ il s‘ agit de ma première
> expérience en modélisation 3D, en conception de PCB, et que l‘ impression 3D est une expérience très récente. Toute aide est la
> bienvenue pour corriger, améliorer, tester.. bref partager.

Ci-après une estimation de l‘ état d‘ avancement des activités envisagées : 

#### 1. Version beta (V0) : prototypage

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
      
#### 2. Version release (V1) : partage et support

- [ ]    0%  : étalonnage des mesures et optimisation de leur durée d‘ intégration
- [ ]    0%  : optimisation de la charge en fonction de l‘ ensoleillement, de la saison, de l‘ heure, ...
- [ ]    0%  : publication d‘ un profil d‘ impression makerworld « plug-and-play »
- [x] 100%  : documentation/schéma électronique/inventaire des composants électroniques
- [ ]    0%  : documentation/inventaire des composants mécaniques
- [ ]    0%  : documentation/tutoriel de montage

## Inventaire des composants/matériaux

La liste des composants pour le PCB  :
| N° | Référence | Valeur/Modèle | Désignation |
|----------------|-----------|-------|---------|
| 1 | C1 | 100nF | [C_Disc_D3.0mm_W2.0mm_P2.50m](https://fr.aliexpress.com/item/32973259342.html) |
| 2 | C2 | 100µF | [CP_Radial_D6.3mm_P2.50mm](https://fr.aliexpress.com/item/1005002524973878.html) |
| 3 | R1 | 330Ω | [R_Axial_DIN0414_L11.9mm_D4.5mm_P15.24mm_Horizontal](https://fr.aliexpress.com/item/1005007032692303.html) |
| 4 | R2 | 330Ω | [R_Axial_DIN0414_L11.9mm_D4.5mm_P15.24mm_Horizontal](https://fr.aliexpress.com/item/1005007032692303.html) |
| 5 | R3 | 100KΩ | [R_Axial_DIN0414_L11.9mm_D4.5mm_P15.24mm_Horizontal](https://fr.aliexpress.com/item/1005007032692303.html) |
| 6 | U1 | WeMos D1 mini pro | [WEMOS_D1_mini_light](https://fr.aliexpress.com/item/1005007475726143.html) |
| 7 | U2 | MCP1700-330 TO-92 | [TO-92_Inline](https://fr.aliexpress.com/item/1005007167297693.html) |
| 8 | Q1 | IRLZ44N TO-220 | [TO-220-3_Vertical](https://fr.aliexpress.com/item/1005007174659364.html) |
| 9 | TP1 | TP4056 USB-C | [TP4056_module](https://fr.aliexpress.com/item/1005006124994712.html) |
| 10 | J1 | XH2.54-2P | [JST_XH_B2B-XH-A_1x02_P2.50mm_Vertical](https://fr.aliexpress.com/item/1005004985397880.html) |
| 11 | J2 | PH2.0-2P | [JST_PH_B2B-PH-K_1x02_P2.00mm_Vertical](https://fr.aliexpress.com/item/1005007441813591.html) |
| 12 | J3 | PH2.0-5P | [JST_PH_B5B-PH-K_1x05_P2.00mm_Vertical](https://fr.aliexpress.com/item/1005007441813591.html) |
| 13 | J4 | PH2.0-5P | [JST_PH_B5B-PH-K_1x05_P2.00mm_Vertical](https://fr.aliexpress.com/item/1005007441813591.html) |
| 14 | J5 | XH2.54-2P | [PinHeader_1x02_P2.54mm_Vertical](https://fr.aliexpress.com/item/4000988113226.html) |

La liste des composants pour l‘ alimentation :
| N° | Qté | Valeur/Modèle | Désignation |
|---|---|---|---|
| 1 | 1| 18650 Lithium 3.7V 3800mAh XH2.54-2P | [Batterie Lithium](https://fr.aliexpress.com/item/1005007257546981.html)|
| 2 | 2| 5V 1W 107x61mm| [Panneaux solaires](https://fr.aliexpress.com/item/1005006711306491.html)|

La liste des composants pour les mesures :
| N° | Qté | Valeur/Modèle | Désignation |
|---|---|---|---|
|  1 | 1| KY-003 A3144|         [Capteur à effet hall](https://fr.aliexpress.com/item/1005007985856987.html)         |
|  2  | 2 |       Disque 5x3mm      |                                               [Aimants ferrite](https://fr.aliexpress.com/item/1005008858265927.html)                                               |
|   3  |  N |         TODO        |                                                 TODO                                                 |

La liste des consommables pour l‘ impression 3D :
| N° | Qté | Valeur/Modèle | Désignation |
|---|---|---|---|
|  1 | NNNg| PETG HF|         [blanc](https://eu.store.bambulab.com/fr/products/petg-hf?id=49068714787164)         |
|  2  |   NNNg  |   PETG HF  |                                               [noir](https://eu.store.bambulab.com/fr/products/petg-hf?id=49068714754396)                                               |
|  3  |   NNNg  |   TPU  |                                               [noir](https://eu.store.bambulab.com/fr/products/tpu-95a-hf?id=47305218687324)                                               |

La liste des consommables pour l‘ anémomètre :
| N° | Qté | Valeur/Modèle | Désignation |
|---|---|---|---|
|  1 | 2| M4x200|         [Tiges filetées](https://fr.aliexpress.com/item/1005008105589322.html)         |
|  2  |   4  |   5x10x4mm  |                                               [Roulements](https://fr.aliexpress.com/item/1005007668446060.html)                                               |
|  3  |   N  |   M4  |                                               Ecrous                                               |
|   4  |   4   |    M3x30   |                                                  [Vis](https://fr.aliexpress.com/item/1005002011961287.html)                                                  |
|   5   |    4   |     M3    |                                                    Ecrous                                                   |
|   6  |   N   |    TODO   |                                                  TODO                                                  |

## Licence

L e projet est publié sous licence [Creative Commons Attribution-Noncommercial-Share Alike](https://github.com/slash4you/Anemometre-Girouette/blob/main/LICENSE.md).

![Licence](https://mirrors.creativecommons.org/presskit/buttons/88x31/png/by-nc-sa.eu.png)
