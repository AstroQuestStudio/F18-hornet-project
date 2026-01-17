# Projet "Hornet Evo" : Dossier de Projet & Stratégie Budgétaire

## Introduction

Le projet "Hornet Evo" vise à créer un cockpit de simulation de vol pour l'avion F-18, en utilisant des matériaux et des composants électroniques de haute qualité. Ce dossier présente la liste complète des pièces et matériaux nécessaires pour la Phase 1 du projet, ainsi que les justifications pour chaque choix.

### Objectifs de la Phase 1

- Construire la structure complète du cockpit.
- Intégrer l'électronique de base.
- Assembler et peindre le cockpit aux couleurs de l'IPSA Flight.
- Rendre les boutons et lumières fonctionnels, interfacés avec un PC portable de test.

### Budget Total Estimé

Le budget total estimé pour la Phase 1 est de 2 500 €.

## Stratégie d'Optimisation des Coûts

Pour optimiser les coûts, nous avons mis en place plusieurs stratégies :

1. **Internalisation de la Production** : En utilisant nos propres imprimantes 3D et les machines disponibles dans le FabLab, nous pouvons réduire les coûts de production. Cela nous permet de ne budgétiser que les consommables (filament, résine) et non la sous-traitance de pièces.

2. **Financement Échelonné** : Au lieu de demander une enveloppe globale, nous proposons un financement par objectifs. Cela permet de reporter l'achat du matériel coûteux (PC de simulation, casque VR) à la fin du projet, conditionné à la réussite de la construction physique.

3. **Réutilisation Matériel** : Pour la phase de construction et de test, nous utiliserons les PC personnels des membres ou les machines actuelles de l'association, repoussant l'achat de la "Station de Combat" à la livraison finale.

## Liste Détaillée des Pièces et Matériaux

### 1. Bois et Panneaux

| Matériau | Dimensions | Quantité | Justification |
|----------|------------|----------|---------------|
| MDF 18 mm | 2440 × 1220 mm | 5 plaques | Utilisé pour la structure porteuse du cockpit, y compris la base, les consoles et les supports principaux. Le MDF est choisi pour sa stabilité et sa facilité de découpe. |
| MDF 12 mm | 2440 × 1220 mm | 3 plaques | Utilisé pour les cadres internes et les supports écrans. Une épaisseur moindre est suffisante pour ces éléments. |
| MDF 6 mm | 2440 × 1220 mm | 2 plaques | Utilisé pour les cloisons et les séparateurs internes. Une épaisseur réduite permet une meilleure flexibilité. |
| Contreplaqué bouleau 18 mm | 2440 × 1220 mm | 2 plaques (optionnel) | Utilisé pour la base du cockpit et les supports de siège. Le contreplaqué offre une meilleure rigidité que le MDF. |
| Tasseaux pin 30×30 mm | 12 m | | Utilisés pour les renforts et les fixations des panneaux. Le pin est léger et facile à travailler. |
| Tasseaux pin 40×40 mm | 6 m | | Utilisés pour les supports écrans et les renforts supplémentaires. |

### 2. Acrylique et Panneaux Gravés

| Matériau | Dimensions | Quantité | Justification |
|----------|------------|----------|---------------|
| Acrylique noir 3 mm | 600 × 400 mm | 10 plaques | Utilisé pour les panneaux rétroéclairés. L'acrylique noir permet un meilleur contraste pour les lumières. |
| Acrylique blanc translucide 3 mm | 600 × 400 mm | 8 plaques | Utilisé pour le rétroéclairage. L'acrylique blanc translucide diffuse uniformément la lumière. |

### 3. Électronique

#### Microcontrôleurs

| Composant | Quantité | Justification |
|-----------|----------|---------------|
| Arduino Mega 2560 | 3 | Utilisés comme unités principales de contrôle pour les entrées/sorties (I/O) des panneaux de contrôle. Choisis pour leur stabilité et compatibilité avec DCS-BIOS. |
| Arduino Nano / Pro Micro | 8 | Utilisés pour les sous-panneaux et modules locaux. Leur petite taille et leur flexibilité en font un choix idéal pour les espaces restreints. |
| ESP32 (optionnel) | 1-2 | Utilisés pour les fonctionnalités réseau et WiFi. Optionnel pour les extensions futures. |

#### Bus et Communication

| Composant | Quantité | Justification |
|-----------|----------|---------------|
| Module RS-485 (MAX485) | 12 | Utilisés pour la communication entre les microcontrôleurs. Le protocole RS-485 est choisi pour sa robustesse et sa capacité à transmettre des signaux sur de longues distances. |
| Résistances 120Ω | 10 | Utilisées pour la terminaison des lignes RS-485. Essentielles pour éviter les réflexions de signal. |
| Câble torsadé (RS-485) | 20 m | Utilisé pour les connexions RS-485. Le câble torsadé réduit les interférences électromagnétiques. |

#### Interrupteurs (Switches)

| Type | Quantité | Justification |
|------|----------|---------------|
| SPST ON-OFF | 60 | Utilisés pour les interrupteurs principaux. Leur simplicité et leur fiabilité en font un choix idéal. |
| SPDT ON-OFF-ON | 30 | Utilisés pour les interrupteurs à trois positions. Permettent une plus grande flexibilité dans le contrôle. |
| DPDT ON-OFF | 10 | Utilisés pour les interrupteurs à double pôle. Idéaux pour les applications nécessitant une commutation de plusieurs circuits. |
| Momentary ON-(OFF) | 20 | Utilisés pour les boutons momentanés. Parfaits pour les actions temporaires. |
| Push button tactile | 50 | Utilisés pour les boutons tactiles. Leur sensibilité et leur durabilité en font un choix populaire. |

#### Encodeurs Rotatifs

| Type | Quantité | Justification |
|------|----------|---------------|
| Encodeur rotatif 24 pas | 20 | Utilisés pour les contrôles de précision, comme les réglages de radio et de HUD. Leur résolution élevée permet un contrôle fin. |
| Encodeur avec push | 10 | Utilisés pour les contrôles combinés rotation/poussoir, comme dans l'UFC (Unit Function Controller). |

#### LEDs et Rétroéclairage

| Type | Quantité | Justification |
|------|----------|---------------|
| LED 3 mm vert | 100 | Utilisées pour les indicateurs de statut et les lumières de contrôle. Le vert est souvent utilisé pour les états actifs. |
| LED 3 mm ambre | 60 | Utilisées pour les indicateurs d'avertissement. L'ambre est une couleur standard pour les alertes. |
| LED 3 mm rouge | 40 | Utilisées pour les indicateurs d'urgence. Le rouge est universellement reconnu pour les situations critiques. |
| LED 3 mm blanc | 80 | Utilisées pour l'éclairage général et les indicateurs neutres. |
| Ruban LED 12 V blanc | 10 m | Utilisé pour le rétroéclairage des panneaux. Offre une lumière uniforme et est facile à installer. |
| Résistances LED (220Ω / 330Ω) | 300 | Utilisées pour limiter le courant à travers les LEDs. Essentielles pour éviter la surchauffe et prolonger la durée de vie des LEDs. |

#### Afficheurs

| Composant | Quantité | Justification |
|-----------|----------|---------------|
| Écran HDMI 8" (DDI) | 3 | Utilisés pour les affichages principaux dans le cockpit. Leur taille et leur résolution sont idéales pour les informations de vol. |
| Écran HDMI 5" (AMPCD) | 1 | Utilisé pour l'affichage auxiliaire. Plus petit, mais suffisant pour les informations secondaires. |
| Écran OLED / LCD IFEI | 1 | Utilisé pour l'interface de contrôle des systèmes de l'avion. Sa petite taille et sa haute résolution en font un choix idéal. |
| Carte driver écran | 5 | Utilisées pour contrôler les écrans. Essentielles pour la compatibilité et la fonctionnalité des écrans. |

#### Audio et Divers

| Composant | Quantité | Justification |
|-----------|----------|---------------|
| Amplificateur audio | 1 | Utilisé pour amplifier les sons du cockpit. Essentiel pour une expérience immersive. |
| Haut-parleurs | 2 | Utilisés pour la diffusion du son. Placés stratégiquement pour un son surround. |
| Buzzers | 4 | Utilisés pour les alarmes et les signaux sonores. Leur son distinctif est crucial pour les alertes. |

#### Connectique et Câblage

| Élément | Quantité | Justification |
|---------|----------|---------------|
| Fils Dupont (M/F/F) | 500 | Utilisés pour les connexions électroniques. Leur flexibilité et leur facilité d'utilisation en font un choix idéal. |
| Câble multibrin | 50 m | Utilisé pour le câblage général. Sa durabilité et sa flexibilité sont essentielles. |
| Borniers à vis | 50 | Utilisés pour les connexions sécurisées. Permettent une installation et un retrait faciles. |
| Connecteurs JST | 100 | Utilisés pour les connexions modulaires. Leur fiabilité et leur compacité sont appréciées. |
| Gaines thermo | 5 m | Utilisées pour protéger et organiser les câbles. Essentielles pour une gestion propre des câbles. |

#### Alimentation

| Élément | Quantité | Justification |
|---------|----------|---------------|
| Alimentation 12 V 20 A | 1 | Utilisée pour alimenter l'ensemble du système électronique. Sa capacité est suffisante pour tous les composants. |
| Convertisseur buck 12→5 V | 5 | Utilisés pour convertir la tension pour les composants nécessitant 5 V. Essentiels pour la compatibilité des composants. |
| Fusibles + porte-fusibles | 10 | Utilisés pour protéger les circuits contre les surtensions. Essentiels pour la sécurité et la durabilité du système. |

### 4. Pièces Imprimées en 3D

#### Boutons

| Type de bouton | Quantité | Justification |
|----------------|----------|---------------|
| Boutons ronds 12 mm | 120 | Utilisés pour les contrôles principaux des consoles et du LIP (Left Instrument Panel). Leur taille et leur forme sont ergonomiques. |
| Boutons carrés 12×12 mm | 40 | Utilisés pour l'UIP (Upper Instrument Panel). Leur forme carrée est adaptée aux panneaux de contrôle. |
| Boutons rectangulaires | 20 | Utilisés pour l'UFC (Unit Function Controller). Leur forme rectangulaire est idéale pour les contrôles spécifiques. |
| Boutons translucides (backlight) | 60 | Utilisés pour tous les panneaux. Leur translucité permet un rétroéclairage efficace. |

#### Molette et Knobs

| Type | Quantité | Justification |
|------|----------|---------------|
| Knobs standards (petits) | 30 | Utilisés pour les contrôles des radios et du HUD. Leur petite taille est adaptée aux réglages fins. |
| Knobs moyens | 20 | Utilisés pour les consoles. Leur taille moyenne est idéale pour une variété de contrôles. |
| Knobs larges crantés | 10 | Utilisés pour le radar et le HSI (Horizontal Situation Indicator). Leur grande taille et leurs crans permettent un contrôle précis. |
| Knobs concentriques | 6 | Utilisés pour l'UFC et les communications. Leur conception concentrique permet des contrôles multiples sur un seul knob. |

#### Stick F-18

| Élément | Quantité | Justification |
|---------|----------|---------------|
| Grip F-18 (coques) | 2 | Utilisés pour le grip du stick. Leur conception est fidèle à l'original pour une expérience réaliste. |
| Chapeau Trim | 1 | Utilisé pour les réglages fins du stick. Essentiel pour la précision des contrôles. |
| Castle switch | 1 | Utilisé pour le contrôle principal du stick. Sa position et sa fonction sont cruciales. |
| Sensor Select | 1 | Utilisé pour la sélection des capteurs. Essentiel pour les fonctions de combat. |
| Trigger (2 parties) | 2 | Utilisé pour la gâchette du stick. Sa conception en deux parties permet une meilleure ergonomie. |
| Supports internes | 4 | Utilisés pour la structure interne du stick. Essentiels pour la stabilité et la durabilité. |

#### Throttle

| Élément | Quantité | Justification |
|---------|----------|---------------|
| Coques throttle gauche/droite | 2 | Utilisées pour les coques du throttle. Leur conception est fidèle à l'original pour une expérience réaliste. |
| Levier Idle / Cutoff | 2 | Utilisés pour les contrôles du throttle. Essentiels pour le fonctionnement du moteur. |
| Molettes radar | 2 | Utilisées pour les contrôles du radar. Leur position et leur fonction sont cruciales. |
| Supports capteurs Hall | 4 | Utilisés pour les capteurs Hall. Essentiels pour la détection précise des mouvements du throttle. |

#### Supports et Brackets

| Type | Quantité | Justification |
|------|----------|---------------|
| Supports écrans DDI | 3 | Utilisés pour les écrans DDI (Digital Display Indicator). Leur conception permet une fixation sécurisée. |
| Support AMPCD | 1 | Utilisé pour l'écran AMPCD (Advanced Multi-Purpose Color Display). Essentiel pour la stabilité de l'écran. |
| Supports IFEI | 1 | Utilisé pour l'IFEI (Integrated Flight and Engine Indicator). Sa conception est adaptée à la taille et au poids de l'écran. |
| Brackets Arduino | 10 | Utilisés pour les microcontrôleurs Arduino. Leur conception permet une fixation sécurisée et une bonne dissipation de la chaleur. |
| Supports PCB | 20 | Utilisés pour les cartes de circuit imprimé. Essentiels pour la stabilité et la durabilité des circuits. |

#### Panneaux Imprimés

| Élément | Quantité | Justification |
|---------|----------|---------------|
| Façades UFC | 1 | Utilisée pour la façade de l'UFC. Sa conception est fidèle à l'original pour une expérience réaliste. |
| Cadres boutons UFC | 2 | Utilisés pour les cadres des boutons de l'UFC. Leur conception permet une fixation sécurisée des boutons. |
| Cadres encodeurs | 10 | Utilisés pour les cadres des encodeurs. Leur conception permet une fixation sécurisée et une bonne accessibilité. |
| Inserts légendes | 50 | Utilisés pour les légendes des boutons et des encodeurs. Essentiels pour l'identification et l'utilisation des contrôles. |

#### Entretoises et Petites Pièces

| Type | Quantité | Justification |
|------|----------|---------------|
| Entretoises M3 (10–20 mm) | 200 | Utilisées pour les fixations des panneaux et des composants. Leur longueur variable permet une adaptation à différentes épaisseurs. |
| Clips câble | 50 | Utilisés pour la gestion des câbles. Essentiels pour une organisation propre et sécurisée des câbles. |
| Guides LED | 60 | Utilisés pour les guides de lumière des LEDs. Leur conception permet une diffusion uniforme de la lumière. |

### 5. Visserie et Quincaillerie

#### Vis Métriques

| Type | Longueur | Quantité | Justification |
|------|----------|----------|---------------|
| Vis M3 | 6 mm | 300 | Utilisées pour les fixations des PCB et des boutons. Leur petite taille est adaptée aux composants électroniques. |
| Vis M3 | 8 mm | 300 | Utilisées pour les panneaux fins. Leur longueur est adaptée à l'épaisseur des panneaux. |
| Vis M3 | 10 mm | 250 | Utilisées pour les pièces imprimées en 3D. Leur longueur est adaptée à l'épaisseur des pièces. |
| Vis M3 | 16 mm | 200 | Utilisées pour les brackets. Leur longueur est adaptée à l'épaisseur des brackets. |
| Vis M3 | 20 mm | 100 | Utilisées pour les supports épais. Leur longueur est adaptée à l'épaisseur des supports. |
| Vis M4 | 10 mm | 150 | Utilisées pour les supports écrans. Leur longueur est adaptée à l'épaisseur des supports. |
| Vis M4 | 16 mm | 150 | Utilisées pour les consoles. Leur longueur est adaptée à l'épaisseur des consoles. |
| Vis M4 | 20 mm | 120 | Utilisées pour la structure. Leur longueur est adaptée à l'épaisseur de la structure. |
| Vis M4 | 30 mm | 80 | Utilisées pour la base du cockpit. Leur longueur est adaptée à l'épaisseur de la base. |

#### Vis Bois

| Type | Dimensions | Quantité | Justification |
|------|------------|----------|---------------|
| Vis bois | 3×15 mm | 300 | Utilisées pour les panneaux MDF de 6 mm. Leur longueur est adaptée à l'épaisseur des panneaux. |
| Vis bois | 4×20 mm | 400 | Utilisées pour les panneaux MDF de 12 mm. Leur longueur est adaptée à l'épaisseur des panneaux. |
| Vis bois | 4×40 mm | 500 | Utilisées pour les panneaux MDF de 18 mm. Leur longueur est adaptée à l'épaisseur des panneaux. |
| Vis bois | 5×60 mm | 150 | Utilisées pour la base du cockpit. Leur longueur est adaptée à l'épaisseur de la base. |

#### Écrous, Rondelles et Entretoises

| Type | Quantité | Justification |
|------|----------|---------------|
| Écrou M3 | 600 | Utilisés pour les fixations des composants électroniques. Leur taille est adaptée aux vis M3. |
| Écrou M4 | 300 | Utilisés pour les fixations de la structure. Leur taille est adaptée aux vis M4. |
| Écrou frein M3 | 200 | Utilisés pour les fixations sécurisées des composants électroniques. Leur conception empêche le desserrage. |
| Écrou frein M4 | 150 | Utilisés pour les fixations sécurisées de la structure. Leur conception empêche le desserrage. |
| Rondelle M3 | 800 | Utilisées pour répartir la charge des vis M3. Essentielles pour la stabilité des fixations. |
| Rondelle M4 | 500 | Utilisées pour répartir la charge des vis M4. Essentielles pour la stabilité des fixations. |
| Entretoise M3 | 6 mm | 100 | Utilisées pour les fixations des panneaux. Leur longueur est adaptée à l'épaisseur des panneaux. |
| Entretoise M3 | 10 mm | 150 | Utilisées pour les fixations des composants électroniques. Leur longueur est adaptée à l'épaisseur des composants. |
| Entretoise M3 | 20 mm | 100 | Utilisées pour les fixations des supports. Leur longueur est adaptée à l'épaisseur des supports. |
| Entretoise M4 | 10 mm | 80 | Utilisées pour les fixations des écrans. Leur longueur est adaptée à l'épaisseur des écrans. |

#### Inserts Filetés

| Type | Quantité | Justification |
|------|----------|---------------|
| Insert M3 laiton | 400 | Utilisés pour les fixations des pièces imprimées en 3D. Leur conception permet une fixation sécurisée et durable. |
| Insert M4 laiton | 200 | Utilisés pour les fixations de la structure. Leur conception permet une fixation sécurisée et durable. |

#### Quincaillerie Diverse

| Élément | Quantité | Justification |
|---------|----------|---------------|
| Équerres métalliques | 40 | Utilisées pour la base et les consoles. Leur conception permet une fixation sécurisée et une bonne stabilité. |
| Charnières | 10 | Utilisées pour les panneaux ouvrants. Leur conception permet une ouverture et une fermeture faciles. |
| Aimants néodyme | 40 | Utilisés pour les accès de maintenance. Leur force magnétique permet une fixation sécurisée et une ouverture facile. |
| Colliers de serrage | 200 | Utilisés pour le câblage. Leur conception permet une organisation propre et sécurisée des câbles. |
| Velcro industriel | 5 m | Utilisé pour les fixations temporaires. Sa conception permet une fixation et un retrait faciles. |

### 6. Licences Logicielles

| Logiciel | Coût | Justification |
|----------|------|---------------|
| Flight Simulator | 20-25 € | Utilisé pour la simulation de vol. Son coût est raisonnable et il est compatible avec les systèmes de contrôle. |
| DCS World | 80 € (hors réductions) | Utilisé pour la simulation de combat. Son coût est justifié par sa haute qualité et sa compatibilité avec les systèmes de contrôle. |

## Budget Détaillé

| Poste de Dépense | Coût Estimé |
|------------------|-------------|
| Structure (Le "Tub") | 500 € |
| Consommables 3D | 450 € |
| Électronique Cœur | 700 € |
| Esthétique & Branding | 500 € |
| Quincaillerie | 350 € |
| **Total** | **2 500 €** |

## Justification des Choix

### Bois et Panneaux

- **MDF** : Choisis pour sa stabilité et sa facilité de découpe. Le MDF est un matériau économique et facile à travailler, idéal pour la structure principale du cockpit.
- **Contreplaqué** : Optionnel pour une meilleure rigidité. Le contreplaqué est plus résistant que le MDF et est utilisé pour les zones porteuses.

### Acrylique

- **Acrylique noir et blanc translucide** : Choisis pour les panneaux rétroéclairés. L'acrylique noir offre un bon contraste pour les lumières, tandis que l'acrylique blanc translucide diffuse uniformément la lumière.

### Électronique

- **Arduino** : Choisis pour leur stabilité et leur compatibilité avec DCS-BIOS. Les Arduino Mega sont utilisés pour les contrôles principaux en raison de leur grande quantité d'entrées/sorties.
- **Modules RS-485** : Choisis pour leur robustesse et leur capacité à transmettre des signaux sur de longues distances. Essentiels pour la communication entre les microcontrôleurs.
- **LEDs et Ruban LED** : Choisis pour leur efficacité énergétique et leur durabilité. Les LEDs sont utilisées pour les indicateurs de statut et les lumières de contrôle, tandis que le ruban LED est utilisé pour le rétroéclairage des panneaux.

### Pièces Imprimées en 3D

- **Boutons et Knobs** : Choisis pour leur ergonomie et leur fidélité à l'original. Les boutons et les knobs sont conçus pour offrir une expérience réaliste et confortable.
- **Stick et Throttle** : Choisis pour leur fidélité à l'original et leur ergonomie. Les pièces du stick et du throttle sont conçues pour offrir une expérience de vol réaliste.

### Visserie et Quincaillerie

- **Vis et Écrous** : Choisis pour leur compatibilité et leur durabilité. Les vis et écrous sont sélectionnés pour offrir une fixation sécurisée et durable.
- **Quincaillerie diverse** : Choisie pour sa fonctionnalité et sa durabilité. Les équerres, charnières, aimants, colliers de serrage et velcro industriel sont sélectionnés pour offrir une fixation sécurisée et une organisation propre des câbles.

### Licences Logicielles

- **Flight Simulator et DCS World** : Choisis pour leur qualité et leur compatibilité avec les systèmes de contrôle. Les licences sont nécessaires pour une expérience de simulation complète et réaliste.

## Prochaines Étapes

1. **Création de versions PDF et Excel** : Pour faciliter la gestion et l'achat des pièces et matériaux.
2. **Organisation par sous-module** : Pour une meilleure planification et exécution du projet.

Ce document devrait couvrir toutes les pièces et matériaux nécessaires pour le projet "Hornet Evo" de Mathis, avec des justifications détaillées pour chaque choix.
