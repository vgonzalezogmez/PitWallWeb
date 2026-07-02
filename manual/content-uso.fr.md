# Manuel d'utilisation — PitWall (organisation / direction de course)

Guide destiné à celui qui **opère** PitWall : monter la course, la diriger en direct, corriger des tours et sortir les résultats.

---

## 1. Introduction
![img: 01-home.png]

**PitWall** est le système de chronométrage et de gestion de courses de slot. Il détecte le passage de chaque voiture sur la ligne d'arrivée grâce au matériel de chronométrage, avec deux options compatibles :

- **DS-300** — par **port série**. Tu peux relier **jusqu'à 6 circuits** DS-300 dans une seule course : chaque boîtier chronomètre ses voies et PitWall les combine.
- **BART (Policar)** — par **Bluetooth**. Il admet **jusqu'au nombre maximal de voies que permet BART** (actuellement **32**).

Tu peux utiliser l'une ou l'autre source ; pour PitWall le flux de passages est équivalent.

- Depuis l'**écran d'accueil**, tu accèdes aux **Courses**, aux **Réglages** et au reste des modules.
- En bas à droite, tu vois toujours l'**état de la liaison** (vert = connecté ; « Sans signal » = vérifie le câble/port ou le Bluetooth).

**La liste des courses** te montre toutes tes courses avec leur état (en attente / active / terminée) et le bouton *Nouvelle course (« + Nueva carrera »)*.

![img: 02-races-list.png]

## 2. Scénarios, catégories et catalogues (ta bibliothèque)

Pour ne pas reconfigurer la même chose à chaque course, PitWall enregistre des **modèles réutilisables** que tu choisis ensuite au moment de créer une course.

**Scénarios (circuits enregistrés).** Un **scénario** est une piste physique enregistrée : nombre de circuits et de voies (par ex. `8+8+8 = 24`), sa **séquence de voies** (rotation) et le **temps minimum par défaut**. Toute course affectée à ce scénario en hérite automatiquement.

![img: op-escenarios.png]

Lors de l'édition d'un scénario, tu définis son nom, la configuration des voies, tu fais glisser la **séquence de rotation** (avec des **repos DSC** s'il y a trop de pilotes), le **temps minimum par défaut** et, en option, des **tours minimums par catégorie** (un Pt différent pour GT, Tourisme, Classiques… sur cette même piste).

![img: op-escenario-form.png]

**Catégories.** Groupes de niveau/classe (GT, Tourisme, Classiques…) qui servent à **surcharger le temps minimum (Pt) par catégorie** dans chaque scénario et à classer voitures et pilotes.

![img: op-categorias.png]

**Catalogues réutilisables (pilotes, équipes, voitures).** Tiens à jour ta **base de données** de participants et de matériel pour la réutiliser d'une course à l'autre :
- **Pilotes** — nom et catégorie ; chaque pilote peut avoir son **QR** d'identification.
- **Équipes** — nom, couleur, pays, voiture et membres.
- **Voitures** — marque, modèle et catégorie.

Tous peuvent être **importés en bloc depuis un CSV** (boutons *Modèle CSV (« Plantilla CSV »)* et *Importer CSV (« Importar CSV »)*, avec un aperçu des nouveautés vs. doublons) et exportés.

![img: op-catalogo-pilotos.png]

![img: op-qr-pilotos.png]

> Avec *Exporter QR (« Exportar QR »)*, tu imprimes les cartes QR de tous les pilotes (pour le changement de pilote par scan en endurance — voir *Contrôle des relais*).

## 3. Créer une course
![img: 03-wizard-step1.png]

Appuie sur *Nouvelle course (« + Nueva carrera »)* et suis l'assistant :

- **Type** :
  - *Sprint* → une **course rapide**, de **pilotes ou d'équipes**.
  - *Endurance* → une **course d'endurance** (par équipes), qui ajoute le **contrôle du temps couru par chaque pilote** de l'équipe (voir *Contrôle des relais de pilote*).
- **Voies et circuits** : nombre total de voies et répartition entre les boîtiers (par ex. 8+8+6 = 3 boîtiers DS-300).
- **Temps minimum de tour (Pt)** : en dessous de ce temps, un passage est considéré comme **fantôme** (rebond/double lecture) et ne compte pas.
- **Passages** : combien de fois la **séquence de voies entière** est parcourue. 2 passages = la rotation complète est courue 2 fois (deux fois plus de manches).
- **Répéter la voie** : chaque voie est courue ce nombre de **manches d'affilée** (même voie), en cumulant les tours — pour comparer chaque répétition.
- **Pole** (facultatif) et **règles de pilote** (championnat uniquement : min/max par pilote, blocage de changement en fin de manche).

> Les **passages** et la **répétition de voie** ne changent que la façon dont les manches sont générées ; les totaux se cumulent par participant.

## 4. Séries, participants et rotation
![img: 34-tanda.png]

Une **série** regroupe les participants et leur **rotation de voies** par manche. Lorsque tu ajoutes les **équipes/pilotes**, PitWall génère automatiquement toutes les **manches**.

**Comment fonctionne la rotation.** Chaque participant change de voie de manche en manche en suivant la séquence configurée (par ex. `1, 3, 5, 6, 4, 2`). Ainsi, tout le monde passe par toutes les voies et les conditions s'égalisent.

- *Exemple (6 voies, 6 pilotes) :* dans la manche 1, le pilote A court sur la voie 1 ; dans la manche 2, la 3 ; dans la 3, la 5… jusqu'à avoir fait le tour de toutes les voies.

**Rotation à ta guise.** PitWall propose automatiquement une rotation équilibrée, mais **tu peux la gérer comme tu veux** : réordonne la **séquence de voies** à la main (en faisant glisser) pour décider exactement par quelle voie passe chaque participant à chaque manche.

**Repos.** S'il y a **plus de participants que de voies**, la séquence inclut des trous (`0` / `DSC`) qui sont des **repos** : dans cette manche, ce participant ne court pas. PitWall les répartit de façon équilibrée, mais **tu peux aussi les placer où tu veux** dans la rotation (fais-les glisser à la position que tu préfères).

**Avec passages / répétition de voie :**
- *2 passages* → la séquence entière se répète : `1,3,5,6,4,2, 1,3,5,6,4,2`.
- *Répéter la voie 2* → chaque voie, deux manches d'affilée : `1,1,3,3,5,5,6,6,4,4,2,2`.

## 5. Éditer la course, les séries et les manches

Après avoir créé une course, tu peux la retoucher :
- **Éditer la course** — changer le **nom** et, si elle **n'a pas encore de tours enregistrés**, le circuit/scénario. S'il y a déjà des tours, le circuit reste **verrouillé** (pour ne pas casser les données).

![img: op-edit-carrera.png]

- **Éditer la série** — changer les **noms** des participants et, si la série n'a pas encore commencé, sa composition. Si elle a déjà des manches lancées, elle passe en **mode renommer seulement** (on n'ajoute ni ne retire de participants, pour ne pas déséquilibrer la rotation).

![img: op-edit-tanda.png]

- **Éditer la manche** — changer **qui court sur chaque voie** dans une manche précise, sans régénérer toute la série (utile si une équipe ne se présente pas ou en cas de changement de dernière minute).

## 6. Pole (qualification préalable)
![img: 44-pole-setup.png]

La **pole** est un tour qualificatif **avant** la course pour décider l'ordre de départ. Elle est facultative ; elle s'active à la création de la course (**Pole**) et se lance depuis la page de la course → *Configurer la Pole Position (« Configurar Pole Position »)*.

- **Participants** : tous les inscrits apparaissent. L'**ordre de la liste** est l'ordre dans lequel ils sortiront faire leur tour ; appuie sur *🎲 Aléatoire (« 🎲 Aleatorio »)* pour le mélanger.
- **Voie de pole** : **tous** font leur tour qualificatif sur la **même voie** (pour que ce soit comparable). Choisis-la avec **−/+** ou avec *🎲 Aléatoire (« 🎲 Aleatorio »)*.
- Appuie sur *Commencer la Pole (« Empezar Pole »)* : chaque participant entre à tour de rôle, fait son tour et PitWall enregistre son meilleur temps. Dans le chronométrage, tu peux activer *Ignorer le 1er passage (out-lap) (« Omitir 1er cruce »)* pour ne pas compter le tour de lancement.

**Résultats de la pole.** À la fin apparaît *Résultats Pole (« Resultados Pole »)* avec le **classement final** (du plus rapide au plus lent, avec l'écart au leader et le **meilleur tour**). D'ici, tu peux *✏️ Éditer les temps (« ✏️ Editar tiempos »)* s'il y a eu une erreur, ou continuer avec *🚦 Attribuer les voies de départ (« 🚦 Asignar carriles de salida »)*.

![img: 46-pole-results.png]

**Attribuer les voies après la pole.** La pole ne répartit pas les voies automatiquement : elle ouvre l'écran *Choix de voie (« Elección de carril »)*, où chaque participant **choisit** sa voie **dans l'ordre du classement** — le **poleman** (le plus rapide) choisit en premier, puis le 2e, et ainsi de suite. C'est le classique « le plus rapide choisit sa voie ».

![img: 47-pole-lanes.png]

- La bannière *Choix en cours (« Eligiendo ahora »)* indique à qui c'est le tour ; à gauche tu vois l'**ordre de choix** (le classement) et à droite les **voies disponibles** (avec leur couleur).
- Chacun appuie sur la voie qu'il veut ; cette voie disparaît des disponibles et le tour passe au suivant.
- **S'il y a plus de participants que de voies**, des trous de *💤 Repos (« 💤 Descanso »)* apparaissent : celui qui choisit le repos **ne court pas la manche 1** et **entre dans la rotation à partir de la manche 2**.
- Quand tout le monde a choisi, appuie sur *🏁 Créer la Première Série (« 🏁 Crear Primera Tanda »)* : PitWall crée la série et génère toutes les manches avec cette grille comme point de départ (l'ordre de choix définit la position initiale dans la rotation des voies). À partir de là, la course fait tourner les voies de manche en manche comme d'habitude (voir *Séries et rotation*).

> La pole ne rapporte pas de points dans la course : elle décide seulement **qui choisit sa voie en premier** et, par là, la grille de départ de la première manche.

## 7. PitWall Lap — PIN pour les équipes
![img: 43-lap-pins.png]

**PitWall Lap** est la vue mobile qui permet à chaque **équipe/pilote** de suivre son propre chronométrage depuis le téléphone (ses tours, annoncés par la voix, et sa position). Pour qu'ils accèdent uniquement à *leur* panneau, un **PIN** est distribué par équipe.

- Entre dans **PitWall Lap · PINs** de la course. Tu verras l'adresse que les équipes ouvrent sur le mobile (par ex. `http://<IP-du-serveur>:3000/lap/<id>`) et le tableau **ÉQUIPE → PIN**.
- Donne à chaque équipe **son PIN**. En ouvrant l'adresse et en le saisissant, ils entrent directement sur leur panneau.
- *Nouveau (« Nuevo »)* régénère le PIN d'une équipe (au cas où il aurait fuité ou qu'ils veuillent le changer).

> Les mobiles doivent être sur le **même réseau** que l'ordinateur qui fait office de serveur. Utilise l'IP de la machine, pas `localhost`, quand ils l'ouvrent depuis le téléphone.

## 8. Diriger la course en direct
![img: 20-live-timing.png]

Depuis la page de la course :

1. **Armer la manche** (▶). Elle reste prête, en attente du **GO** du boîtier.
2. **GO** : au moment du départ donné sur le boîtier, le **feu tricolore** apparaît et le chronomètre démarre. Chaque circuit a sa propre horloge (C1/C2/C3).
3. Pendant la manche, tu vois par voie : **total de tours**, **dernier**, **moyenne**, **meilleur**, et en haut la bannière du **meilleur tour**.
4. **Pause / Reprendre / Arrêter** la manche au besoin.
5. À la fin (drapeau ou fin de temps), la manche se ferme et la **suivante** se prépare.
6. Quand toutes les manches d'une série sont terminées, la **série suivante** démarre.

**Choisir la vue.** Avec le bouton *Vue (« Vista »)*, tu changes la mise en page selon les voies : *Lignes horizontales* (peu de voies), *Grille compacte* (beaucoup) ou *Cartes détaillées* (avec tours/sorties/pit/Δ par carte).

**Changer de série, répéter une manche et terminer.** Depuis le direct lui-même, tu as des raccourcis sans quitter l'écran :
- **Série suivante** — quand les manches d'une série se terminent, passe directement à la suivante.
- **Répéter la manche** — si une manche a été jugée mauvaise (faux départ, incident), tu la relances avec les mêmes participants et voies.
- **Terminer la course** — clôt la course (le « drapeau ») : le classement se fige et le résumé est généré pour les résultats et pour les mobiles (PitWall Lap).

> Avertissement **« Sans signal du DS-300 »** : tant qu'il est présent, les tours **ne sont pas enregistrés**. Vérifie la connexion avant de donner le GO.

## 9. Contrôle des relais de pilote (championnats)

Dans les courses de **championnat par équipes**, tu peux imposer des règles de partage du volant entre les pilotes d'une équipe. Elles se définissent à la création de la course :
- **Temps minimum / maximum par pilote** — chaque pilote doit rouler au moins X et au plus Y.
- **Blocage après un changement** — un minimum de temps avant de pouvoir rechanger de pilote.
- **Maximum de relais par pilote**.

Les **changements de pilote** s'enregistrent en scannant le **QR du pilote** (ou en saisissant son code) à l'entrée en piste. Depuis le direct, tu ouvres **Contrôle des relais**, qui affiche le **pilote actuel par voie**, le **temps cumulé** de chacun (en signalant s'il enfreint une règle) et l'**historique des relais** ; si un changement a été mal enregistré, tu peux **corriger le temps** du relais.

## 10. Tour par tour et corrections (ajouter / retirer des tours)
![img: 30-correcciones.png]

Depuis la course (bouton de **correction des tours** dans le direct ou dans les résultats), tu accèdes au **tour par tour** de chaque manche. Il sert à corriger les lectures mal enregistrées.

- **Gauche** : les voies de la manche ; choisis l'équipe/le pilote à revoir.
- **Droite** : sa liste de tours — **TR** (n°), **TEMPS**, **HORLOGE** (moment de course) et **Δ PRÉC.** (différence avec le tour précédent).
- **Actions par tour** :
  - **Transférer** (↔) — passer le tour à **une autre voie/équipe** (si le système l'a mal attribué).
  - **Fantôme** — marquer le tour comme non valide (il ne compte pas) sans le supprimer ; on peut le **restaurer**.
  - **Supprimer** (🗑) — éliminer un tour.
  - **Ajouter un tour manuel** — s'il a manqué un passage, tu l'ajoutes à la main.

> Utilise-le avec discernement : les corrections modifient les totaux, les moyennes et le classement de cette manche.

## 11. Résultats et exports
![img: 10-results-comparativa.png]

À la fin (ou à tout moment), entre dans **Résultats** :

- **Comparatif** (grille) : par participant, chaque voie avec **Rapide / Moyenne / Consistance / Sorties / Pit-stops**. Dans les courses à **passages/répétition de voie**, chaque voie se décompose en ses **occurrences** (1/2, 2/2) pour comparer.
- **Progression / Positions / Écart au leader / Écart (grille) / Statistiques avancées** : différentes vues d'analyse (expliquées en détail dans le *Manuel de statistiques*).
- **Exports** : **Excel**, **Points (xlsx/csv)**, **Control (csv)**, **Exporter pour GitHub**, **PDF**.

**Résultats publics.** Il existe une page ouverte — **Résultats**, dans le menu d'accueil — où n'importe qui peut consulter (sans rien toucher ni pouvoir éditer) les résultats des courses **terminées**. C'est celle que tu partages avec les pilotes et le public pour qu'ils regardent le classement et les statistiques de la course.

![img: op-resultados-publicos.png]

## 12. Entraînement
![img: 40-training.png]

En plus des courses, PitWall dispose d'un mode **Entraînement** (depuis l'écran d'accueil) pour rouler sans monter une compétition complète. Il y a deux modalités :

- **Entraînement libre** : enregistre des **tours par voie sans structure d'équipes**. Idéal pour des séances ouvertes où chacun teste voiture et piste ; il n'y a ni rotation ni classement, seulement des temps par voie.
- **De compétition** : équipes ou pilotes affectés à des voies avec **rotation automatique après chaque série**, comme une course mais pensé pour s'entraîner au format championnat.

Choisis la modalité, attribue les voies et appuie sur *Commencer (« Empezar »)*. Le chronométrage en direct fonctionne comme en course (GO du boîtier, tours, meilleur/moyenne par voie).

## 13. Réglages
![img: 04-settings.png]

- **Matériel / ports** : configure les circuits série (DS-300) et leur nombre de voies.
- **Circuits** : définis des pistes enregistrées (séquence de voies, temps minimum).
- **Licence** et langue (ES/EN).

## 14. Glossaire (opération)
- **Course** : l'événement complet. Il se compose de séries.
- **Série** : groupe de participants avec sa rotation ; elle se compose de manches.
- **Manche** : une tirée chronométrée (toutes les voies en même temps) d'une durée donnée.
- **Rotation** : comment les participants changent de voie d'une manche à l'autre.
- **Repos** : manche dans laquelle un participant ne court pas (trou `0` dans la séquence).
- **Passage** : parcours complet de la séquence de voies ; N passages = N× manches.
- **Répéter la voie** : courir chaque voie N manches d'affilée, en cumulant les tours.
- **GO** : le signal de départ (du boîtier DS-300) qui lance la manche.
- **Tour fantôme** : tour marqué comme non valide (il ne compte pas), restaurable.
- **Pole** : séance de qualification préalable (facultative) ; tous roulent sur la même voie et leur meilleur tour fixe la grille de départ.
- **Entraînement libre** : mode pour enregistrer des tours par voie sans équipes ni rotation (séance ouverte).
- **PitWall Lap** : vue mobile par équipe/pilote (ses tours annoncés et sa position).
- **PIN** : code par équipe pour entrer sur son panneau dans PitWall Lap.
- **Pt (temps minimum)** : seuil en dessous duquel un tour est considéré comme un passage fantôme et ne compte pas.
- **Scénario** : piste enregistrée (circuits, voies, séquence et temps minimum) réutilisable dans plusieurs courses.
- **Catégorie** : classe de voiture/pilote (GT, Tourisme, Classiques…) ; permet un Pt différent par catégorie.
- **Catalogue** : bibliothèque réutilisable de pilotes, équipes et voitures (importable par CSV).
- **QR de pilote** : code qui identifie le pilote pour enregistrer son relais lors du scan.
- **Relais (shift)** : période pendant laquelle un pilote est au volant au sein de son équipe en endurance.
- **DS-300** : le boîtier de chronométrage qui détecte le passage sur la ligne d'arrivée.
