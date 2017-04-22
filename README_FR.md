# ArcticFox
*[NFE Team](http://nfeteam.org) présente un microprogramme personnalisé pour les mods de batterie Joyetech, Wismec et Eleaf

![](http://i.imgur.com/JP4KC8A.png)
![](http://i.imgur.com/E1e7cs1.png)

![](http://i.imgur.com/kYJcp6I.png)
![](http://i.imgur.com/TnqNYK1.png)
![](http://i.imgur.com/0XTV9xD.png)

**Utilisez [NFE Toolbox](https://github.com/TBXin/NFirmwareEditor/releases) pour [installer le microprogramme](https://github.com/maelstrom2001/ArcticFox/wiki/How-to-install) et configurer votre appareil.**

## Liste des périphériques pris en charge:
### Joyetech:
* eVic VTC Mini
* eVic VTC Dual
* eVic VTwo Mini
* eVic VTwo
* eVic AIO
* eVic Basic
* eGrip II / Light
* Cuboid Mini
* Cuboid
* Cuboid 200

### Wismec:
* Presa TC75W
* Presa TC100W
* Reuleaux RX75
* Reuleaux RXmini
* Reuleaux RX200
* Reuleaux RX200S
* Reuleaux RX2/3
* Reuleaux RX300
* VF Lite
* VF Stout
* VF Classic
* BV Centurion
* La Petite Box

### Eleaf:
* Aster
* iStick Pico 75W
* iStick Pico Mega 80W
* iStick Pico Dual
* iStick TC100W
* iStick TC200W
* iStick iPower 80W

## Profils
La principale différence est l'interface utilisateur basée sur le profil, donc le style ADN, 
et l'accent mis sur la personnalisation que le microprogramme original Joyetech. 
Le profil est l'ensemble des paramètres de l'atomiseur utilisé, tels que le matériau de la bobine, la résistance, 
la puissance et les valeurs de température. 
L'utilisateur dispose de 8 profils qui peuvent être édités avec NFE Toolbox et qui peuvent être affectés à ses atomiseurs préférés.

![](http://i.imgur.com/UjtY7Ir.png)

Les profils peuvent être commutés automatiquement, en fonction de la résistance de la bobine enregistrée, et en mode manuel. 
Tout ce que vous devez utiliser le commutateur automatique est d'activer le mode "intelligent", installer l'atomiseur et les affecter au profil désiré.

![](http://i.imgur.com/fadryzQ.png)

Lorsque vous réinstallez cet atomiseur plus tard, le profil attribué sera activé automatiquement. 
Si la résistance de l'atomiseur installé n'est pas trouvée dans les profils, vous serez invité à sélectionner un nouveau profil ou à ré-attribuer existant. 
Lorsque vous basculez manuellement sur un profil qui a enregistré une incompatibilité de résistance, 
vous serez invité à mettre à jour ou à garder les paramètres du profil sélectionné.

## Menu principal

Tenez les boutons Fire et Plus pendant 1 seconde pour accéder au menu.

![](http://i.imgur.com/XSWOLDJ.png)

## Menu du profil

![](http://i.imgur.com/HOO0KiF.png) ![](http://i.imgur.com/2UPcLHy.png) ![](http://i.imgur.com/yNH5crk.png) ![](http://i.imgur.com/kc0PYf7.png) ![](http://i.imgur.com/CNzn7vQ.png) ![](http://i.imgur.com/3MHoldt.png)

* **Wire** - Le matériau coil, la détection de la température ou non (VW) peut être réglé sur un TFR standard ou défini par l'utilisateur;
* **Coil** - résistance enregistrée;
* **TCR** - La valeur TCR peut être modifiée lorsque sélectionné Joyetech TC algo avec TCR personnalisé;
* **T. Dom** - style de régulation dominant la température;
* **Preheat** - contrôle de puissance, utilisation préchauffage ou courbe de puissance;
* **PI-Reg** - Régulateur PI pour le mode TC, améliore la stabilisation de la puissance et de la température:
     - PI-Reg On/Off - basculer entre le stock Joyetech et la réglementation PI;
     - Range - 0..100% - plage de température lorsque la régulation PI devient active. 0 signifie que le régulateur est toujours allumé et contrôle la distribution de puissance depuis le début de la bouffée, 20% par exemple - le régulateur PI s'allume lorsque la température de la bobine atteint 20% des paramètres du profil;
     - P - constante proportionnelle, plus elle est grande, plus la puissance est nette;
     - I - constante intégrale, plus elle est grande, la distribution de puissance installée est plus lisse.

## Menu d'écran

![](http://i.imgur.com/6jddZL9.png) ![](http://i.imgur.com/3fRgkGN.png) ![](http://i.imgur.com/FmVjNro.png) ![](http://i.imgur.com/2UYldpC.png)

* **Dim** - Temps d'affichage faible;
* **Wake <>** - mode réveil en appuyant sur les boutons réglementaires;
* **Charge** - afficher des informations supplémentaires sur l'écran de chargement, la tension de la batterie et la température du panneau;
* **Logo** - afficher le logo sur l'écran principal;
* **Clock** - horloge à l'écran:
     - Type - analogique ou numérique;
     - On Main - affiche l'horloge sur l'écran principal;
     - Saver - affiche l'horloge en mode veille;
* **Contrast** - régler la luminosité de l' affichage;
* **Skin** - modifiez le style de l'écran principal.

## Menu Paramètres

![](http://i.imgur.com/aDuSk3n.png) ![](http://i.imgur.com/3JeWUqf.png) ![](http://i.imgur.com/8V1VCeo.png)

* **1 Watt** - puissance d'incrémentation / décrémentation de 1,0 Watt;
* **Menu** - New -  changer les profils à l'aide du sélecteur, Ancien-commutateur via standard Modifier Action principale;
* **Smart** - Paramètres des profils de commutation automatique:
     - On/Off;
     - Tolérance de résistance;
     - Afficher le menu du profil après avoir attribué de nouveaux;
* **Clicks** - Actions assignées au 2/3/4 Fire button clicks:
     - None;
     - Edit Main - Joyetech action par défaut de 3-clics;
     - Profiles - Sélecteur de profils;
     - T. Dom - dominante de la température on/off;
     - Clock - afficher / masquer l'horloge sur l'écran principal;
     - On/Off - commute le mod on/off;
     - LSL - le mode de veille lumineuse on/off;
     - Main Menu - entre dans Menu principal, identique à Fire + ;
     - Preheat - préchauffer les paramètres du profil actif;
     - Edit Profile - entrer le menu Profil;
     - Smart On/Off
     - Afficher l'écran d'informations
* **RTC** - configuration de l'horloge en temps réel;
* **Expert** - paramètres pour les utilisateurs avancés:

![](http://i.imgur.com/UZBrHjJ.png) ![](http://i.imgur.com/7fT0pNi.png) ![](http://i.imgur.com/edejq3z.png) ![](http://i.imgur.com/FoH1vaE.png)

* **USB**
     - NoSlp - n'entrent pas en mode sommeil profond pendant que vous êtes connecté à USB;
     - Charge -  l'appareil charge les piles tout en étant connecté à l'USB;
* **BVO** - tension des batteries décalées;
* **BATT** - profil de décharge de la batterie;
* **SHUNT** - Correction Ohm-meter;
* **ChkTCR** - vérifiez le TCR du coil, la désactivation de cette option peut éliminer l'erreur TCR sur les coils lourds;
* **RCOBC** - Réinitialiser les compteurs sur la modification de la batterie, effacer les statistiques de vaping;
* **X32** - Le module RTC utilise un oscillateur secondaire 32768Hz, s'il est présent;
* **LSL** - Light Sleep Mode, pour les appareils sans oscillateur secondaire, conservez RTC précis. Il prend plus d'énergie en mode veille, de sorte que l'utilisateur sera averti! Signe l'indicateur de l'indicateur de batterie;
* **TEMP** - capteur de température du panneau, Ext - thermistor, Int - MCU


## Écran d'information
![](http://i.imgur.com/2QoKfkX.png)

Affiche de brèves informations sur le matériel et certaines statistiques.

###Merci beaucoup à:
     * TBXin - for NFE Products, ideas and tests
     * Zinger - for graphics, ideas and tests
     * ClockSelect - for great project called myevic

# Avertissement:

Le firmware est distribué dans l'espoir qu'il sera utile, mais sans garantie. Il est fourni "tel quel" sans garantie d'aucune sorte, expresse ou implicite, y compris, mais sans s'y limiter, les garanties implicites de qualité marchande et de conditionnement physique à des fins particulières. L'intégralité du risque de qualité et de performance du firmware est avec vous.

# Dons:
Si vous aimez notre projet et que vous souhaitez contribuer à son développement, vous pouvez nous faire un don en argent, que vous jugez acceptable.
