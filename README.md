# Conception et réalisation d'un robot manipulateur á trois degrés de liberté et à commande vocale (ROMA3DL)🦾

# Description:
Le projet ***ROMA3DL***(Robot manipulateur á 3 dégrès de  liberté) a pour but de concevoir, fabriquer et piloter un robot manipulateur articulé possédant trois degrés de liberté. En robotique, un degré de liberté correspond à une direction indépendante de mouvement (comme une rotation ou une translation). Un bras robotisé avec 3 degrés de liberté peut donc effectuer des mouvements complexes dans un plan ou dans une partie de l'espace tridimensionnel.

🦾 Ce que cela signifie :
Ce type de robot est composé de trois articulations : ***deux articulations rotatives*** qui permettent de pivoter autour de l'axe Oz et Oy et ***une articulation de translation*** qui permet un mouvement linéaire suivant l'axe Ox, ou parfois une troisième rotation de la pince.

Cela lui permet de réaliser des tâches de type prise avec des objets et de se déplacer dans une certaine zone restreinte de l'espace.
<br><br><img align="center" src= "https://github.com/user-attachments/assets/ec1ecd6c-881a-4389-8f1f-4fbe2099ea83" alt="ROMA3DL_logo" width="100%" /><br><br>
ROMA3DL est un bras robotique à trois degrés de liberté conçu pour offrir une solution polyvalente en matière de manipulation d’objets. Il s’inscrit dans le cadre d’un projet de fin d’année destiné aux étudiants en deuxième année de classes préparatoires D'ESEO-France délocalisées au Togo au Lycée International Cours Lumière, combinant des aspects de conception mécanique, d’électronique et de programmation. C’est donc une synthèse des compétences acquises durant l’année qui a pour objectif principal de permettre aux étudiants d’explorer les concepts fondamentaux de la robotique et de l’automatisation en développant un système fonctionnel et interactif.
<br>

# Sommaire  

[I. Qui sommes-nous ?](#i-Qui-sommes-nous-)

[II. Objectifs projet ](#ii-Objectif-du-projet)

[III. Fonctionnalités](#iii-Fonctionnalités)

[IV. Liste de matériel](#iv-Liste-de-matériel)

[V. Déroulement ](#v-Déroulement)

  [1. Esquis](#1-Esquis)
  
  [2. modèle 3D](#2-Modèle-3D)
  
  [3. Circuit  èléctronique ](#3-Circuit-èléctronique)
 
  [4. codes](#4-Codes)

[VI. Licence](#vi-Licence)

[VII. Contributions](#vii-Contributions)

[VIII. Remerciements](#viii-Remerciements)

## I. Qui sommes-nous ?

Durant notre deuxième année de classe préparatoire au cycle ingénieur à ***l'ESEO-Cours Lumière au Togo***, nous avons eu à réaliser un projet d’études visant à mettre en application l’ensemble des compétences acquises durant les années préparatoires qui viennent de s'écouler. Notre équipe est constituée de 9 personnes dont:
<br>
<br>**AGBOKOU Guillaume**: agbogui@efecourslumiere.org,<br/> 
<br>**AKPAH Starker**: kanakp@efecourslumiere.org,<br/> 
<br>**BADJA Jules**: poubad@efecourslumiere.org,<br/> 
<br>**BANIZA Emmanuel**: magban@efecourslumiere.org,<br/>
<br>**BANKA Wilfried**: wilban@efecourslumiere.org,<br/>
<br>**COQUEREL Michel**: miccoq@efecourslumiere.org,<br/>
<br>**DOUMBIA Aïchata**: aicdou@efecourslumiere.org,<br/>
<br>**GOUDOU Ariel**: arigou@efecourslumiere.org,<br/>
<br>**KORDOHOU Errath**: errkor@efecourslumiere.org<br/>
<br>
Afin de réaliser du projet, trois équipes ont été formées pour l'aboutissement d'un résultat:
<br>
<br>**Equipe modélisation**:</br>-***AGBOKOU Guillaume***,<br>-***GOUDOU Ariel***</br>
<br>**Equipe programmation manuelle**:</br>-***BANIZA Emmanuel***,<br>-***BADJA Jules***</br>
<br>**Equipe commande vocal**: </br>-***AKPAH Starker***,<br>-***BANKA Wilfried***,<br>-***COQUEREL Michel***</br>
<br>**Equipe documentation**:</br>-***DOUMBIA Aïchata***,<br>-***KORDOHOU Errath***</br> 
<br>
Ce projet, baptisé ***ROMA3DL***, vise à concevoir et à réaliser un robot manipulateur innovant, capable d’être contrôlé de manière hybride, à la fois manuellement mais aussi virtuellement. Pour le contrôle manuel, nous avons intégré des joysticks permettant une prise en main intuitive et une manipulation précise en temps réel. Parralèllement, une application mobile  basée sur la technologie Bluetooth a été développée afin d’offrir une interface de commande virtuelle, rendant possible le pilotage à distance du robot. Ce projet mobilise des compétences transversales en mécanique (pour la structure et les articulations du bras robotisé), en électronique (pour le traitement des signaux, l’alimentation et le pilotage des moteurs), ainsi qu’en modélisation 3D (pour la conception assistée par ordinateur et l’impression des pièces mécaniques). ***ROMA3DL*** incarne ainsi une approche pluridisciplinaire, alliant théorie et pratique, en vue de proposer une solution technologique fonctionnelle, évolutive et pédagogique.
<br>Il représente pour nous une opportunité de mettre en pratique nos connaissances et d’acquérir une expérience concrète en  ingénierie.</br>
## II. Objectif du projet
**ROMA3DL**  assure une immersion concrète dans la robotique en mettant en pratique leurs connaissances en cinématique, mécanique, électronique et informatique. En concevant un bras robotique à trois degrés de liberté doté d'une commande vocale, nos futurs ingénieurs apprennent à modéliser en CAO(Conception Assistée par Ordinateur), à choisir les moteurs et capteurs adaptés, à programmer des microcontrôleurs et à intégrer des solutions de communication sans fil. Ce projet multidisciplinaire renforce leur autonomie, le travail en équipe et leur capacité à gérer un projet complexe, les préparant ainsi efficacement à leur future carrière d'ingénieur au sein d'écoles prestigieuses comme l'**ESEO**.<br>Le projet ROMA3DL vise à concevoir et développer un robot manipulateur à trois degrés de liberté contrôlé par commande vocale, intégrant des technologies avancées pour améliorer l'interaction humain-robot. Les objectifs spécifiques du projet peuvent être décrits comme suit :</br>

<br>1. Développement technique :
<br>▶Concevoir un système mécanique robuste : Le robot doit posséder une structure mécanique solide et fiable, capable de réaliser des tâches précises avec trois degrés de liberté.</br>
<br>▶Intégrer la commande vocale : Utiliser l'assistant Google pour recevoir et interpréter les commandes vocales, permettant ainsi une manipulation intuitive et sans contact physique.</br>
<br>▶Développer une application mobile : Créer une application via Flutter qui servira d'interface pour la configuration et le contrôle vocal du robot.</br>

<br>2. Innovation technologique :
<br>▶Exploiter les avancées en IA et traitement du langage naturel : Tirer parti des dernières innovations en intelligence artificielle pour améliorer la reconnaissance vocale et la compréhension des commandes.</br>
<br>▶Optimiser la réponse du système : Assurer une réponse rapide et précise du robot aux commandes vocales, minimisant ainsi les délais et les erreurs dans l'exécution des tâches.</br>

<br>3. Application et impact :
<br>▶Évaluation en environnement réel : Tester le robot dans des scénarios réels pour évaluer sa performance et son utilité pratique, notamment dans des environnements industriels ou de recherche.</br>
<br>▶Améliorer l'ergonomie et la sécurité au travail : Démontrer comment le contrôle vocal peut réduire la fatigue et les risques d'accidents, en particulier dans des contextes où les interactions physiques avec les machines présentent des risques.</br>
<br>▶Contribuer à l'éducation et la formation : Utiliser le projet comme outil pédagogique pour les étudiants en ingénierie, leur permettant d'apprendre les principes de la robotique, du contrôle vocal, et de l'interaction homme-machine.</br>

<br>4. Durabilité et évolutivité :
<br>▶Concevoir avec une perspective de durabilité : Assurer que le robot est construit avec des matériaux durables et une conception qui permet des mises à jour faciles.</br>
<br>▶Planifier pour l'évolutivité : Structurer le projet de manière à ce qu'il puisse être facilement amélioré ou modifié pour inclure plus de fonctionnalités ou s'adapter à différents usages.</br>


## III. Fonctionnalités
<br>✅ **Commande vocale**  – Contrôle du bras par des ordres simples via Bluetooth.(A revoir)
<br>
Le bras robotisé est doté d’un système de reconnaissance vocale permettant à l'utilisateur de le contrôler par des commandes simples et intuitives. Grâce à la connectivité Bluetooth, les ordres vocaux sont transmis en temps réel à l’unité centrale du bras, qui les interprète pour exécuter des actions pour saisir, effectuer des rotations et des translations. Cette fonctionnalité rend le dispositif particulièrement accessible aux personnes à mobilité réduite ou dans des contextes où les mains ne peuvent pas être utilisées.
</br>
<br>✅ **Saisie et manipulation d’objets** – Pince robotisée avec capteurs pour ajuster la prise.
<br>
La pince robotisée située à l'extrémité du bras est équipée d'un servomoteur. Avec le code implanté dans l'arduino, la vitesse du  servomoteur utilisé est plus lente qu'un servomoteur d'origine. Ceci permet donc d'adapter automatiquement la force de préhension selon la nature de l'objet à manipuler, évitant ainsi toute casse ou glissement. Cette précision rend possible la saisie d’objets variés, allant de petits éléments fragiles à des pièces plus robustes, et permet une manipulation stable et sécurisée.
</br>
<br>✅ **Contrôle à distance**  – Pilotage via application mobile ou PC.(A revoir)
<br>
Le bras peut également être piloté à distance via une interface dédiée réalisée à partir de flutter et disponible sur ordinateur. L'utilisateur peut envoyer des commandes manuelles ou prédéfinies, et ajuster les paramètres de mouvement selon ses besoins. Cette fonctionnalité est idéale pour les tâches nécessitant une intervention à distance, comme en milieu médical, industriel ou dans les environnements hostiles.
</br>

## IV. Liste de matériel

Le matériel utilisé pour la réalisation de ce projet peut etre répertorié dans le tableau ci-dessous:

| **Systemes**            | **Materielles**                           | **Utilité**                                                |
|-------------------------|--------------------------------------------------|-------------------------------------------------------------|
|🖥️**Microcontrôleur**    | Arduino Mega , Arduino Uno                       |Rélie les différents composants du circuit                  |
|📟**Commande**    |Joysticks                                         |  Controle tous les servomoteurs avec une seule plaque      |
|🦼**Moteur**             |   servomoteur MG90S,servomoteur MG996R           |Crée le mouvement et réduit la vitesse et l'augmente        |
| 🔋**Baterrie**          | 14 volts et 9 volts                              | alimenter  le microcontroleur                              |            
| 📳**module Bluetooth**  | HC-05                                            | Envoyer des commandes vocales depuis une application mobile|   
| **Modélisation 3D** |        Fusion 360     |   pour la  modelisation 3D  |
 |**Impression 3D** |    imprimante Pursa MK4 , Bobine PLA      | Pour l'impression 3D |
## V.  Déroulement 
  ### 1. Esquis
  
<p align="center"><img src="https://github.com/user-attachments/assets/9c078148-df42-43bf-9e1f-611d65630f8c" alt="ROMA3DL_support" width="100%"/></p>

 <p align="center"><img src="https://github.com/user-attachments/assets/6bef7af4-bcb3-4209-ac4b-f498a655eca0" alt="ROMA3DL_bras" width="100%"/></p>
  Ces  images illustrent  les différentes composantes du bras mécanique :
<br>Le bras: élément central assurant la liaison entre les avant-bras et le support de la pince.
<br>Les avant-bras: structures allongées fixées au bras principal, servant de prolongement mécanique. 
<br>Le support de la pince: pièce de fixation qui accueille le système de préhension.
<br>Une pince: outil terminal permettant la saisie d’objets, ici entraîné par un engrenage
<br><br>

  <p align="center"><img src="https://github.com/user-attachments/assets/41cef1cd-ff78-4d63-8d6e-4881f8ae9848"alt="ROMA3DL_repere" width="100%"/></p>
   
   ### 2. Modèle 3D

 <p align="center"><img src="https://github.com/user-attachments/assets/a4c42c1e-4e45-4b38-88c3-af5037b1adf9" alt="ROMA3DL_modele" width="100%" /></p>

  ### 3.Circuit électronique
  <p align="center"><img src="https://github.com/user-attachments/assets/a79ec248-ee8a-40f8-b851-e9fbba729f04" alt="RAMO3DL" width="100%" /></p>
                       
  ### 4. Codes
  ***Commande manuelle***

 ## VI. Licence
Ce programme est un logiciel libre ; vous pouvez le redistribuer et/ou le modifier selon les termes de la Licence Publique Générale GNU 
telle que publiée par la Free Software Foundation ; soit la version 3 de la licence, soit (à votre choix) toute version ultérieure.

## VII. Contributions
 <br>Mr Marc Mino-Matot : Dans l'obtention des materiaux</br>
<br>Mr Hankem Justin: Supervision et controle<br/> 

## VIII. Remerciements
<br>Nous tenons à exprimer notre profonde gratitude aux fondateurs du Lycée International Cours Lumière pour leur soutien financier sans lequel la réalisation de ce projet n’aurait pas été possible. Leur engagement constant envers la réussite des étudiants a été une véritable source de motivation. Nos remerciements vont également à Monsieur Justin Hankem pour ses conseils avisés et son accompagnement tout au long de ce travail. Enfin, nous saluons l’implication et la collaboration de toute la classe de 2e année, dont l’esprit d’équipe et la détermination ont grandement contribué au succès de ce projet.<br/> 

