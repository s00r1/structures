# Flexilogis Studio 3D

> Conceptez des chambres d'hôtel, couloirs et zones modulaires directement depuis votre navigateur. Flexilogis propose une interface repensée, des contrôles guidés et une documentation enrichie pour passer de l'idée au plan 3D en quelques minutes.

## Sommaire
- [Vue d'ensemble](#vue-densemble)
- [Fonctionnalités clés](#fonctionnalités-clés)
- [Prérequis](#prérequis)
- [Démarrage express](#démarrage-express)
- [Navigation et contrôles](#navigation-et-contrôles)
- [Parcours de l'interface](#parcours-de-linterface)
- [Créer et éditer des espaces](#créer-et-éditer-des-espaces)
- [Mobilier et accessoires](#mobilier-et-accessoires)
- [Gestion des niveaux](#gestion-des-niveaux)
- [Alignements et rotations guidées](#alignements-et-rotations-guidées)
- [Sauvegarder, charger et réinitialiser](#sauvegarder-charger-et-réinitialiser)
- [Raccourcis clavier](#raccourcis-clavier)
- [Dépannage rapide](#dépannage-rapide)

## Vue d'ensemble
Flexilogis est une expérience 3D ultra-rapide pour préparer des configurations hôtelières modulaires. Cette version met l'accent sur la lisibilité (ruban recentré, badges contextuels), les contrôles guidés (rotations prédéfinies, tailles rapides) et des repères constants (niveau actif, mode courant, cible couleur).

## Fonctionnalités clés
- **Interface glassmorphism** : ruban de commande centré, panneaux regroupés et indicateurs contextuels permanents.
- **Inspecteur enrichi** : badges visibles pour la cible de couleur, le niveau courant et le type de sélection.
- **Palette clarifiée** : bascule explicite entre la couleur des **murs** et celle des **étiquettes**.
- **Rotations guidées** : axes et angles prédéfinis (15° à 180°) en complément du mode libre.
- **Multi-niveaux** : création, duplication, navigation entre étages ou vue globale.
- **Historique intégré** : annulation/rétablissement avec toasts de confirmation.

## Prérequis
- Navigateur moderne (Chrome, Edge ou Firefox) avec accès internet pour charger les dépendances CDN.
- Aucun serveur requis : l'application peut être lancée en local en ouvrant le fichier HTML.

## Démarrage express
1. Ouvrez le fichier `V3.html` dans votre navigateur.
2. Attendez la fin de l'écran de chargement.
3. Sélectionnez un bloc avec un clic gauche, puis utilisez le ruban et les panneaux pour manipuler la scène.
4. Référez-vous aux raccourcis clavier pour gagner du temps lors des transformations.

## Navigation et contrôles
- **Sélection** : clic gauche sur un bloc ou un meuble.
- **Orbit/Zoom** : gestuelle standard Three.js (glisser droit pour orbiter, molette pour zoomer, clic milieu pour déplacer).
- **Transformations libres** : `W` (déplacer), `E` (rotation), `R` (échelle) via `TransformControls`.
- **Guidage visuel** : badges indiquant le niveau actif, la cible couleur et le mode sélectionné.

## Parcours de l'interface
- **Ruban supérieur** : affiche le mode actif, la sélection courante et rappelle les gestes de navigation.
- **Panneau gauche**
  - Gestion des étages : création, duplication, navigation.
  - Bibliothèque d'objets : chambre complète, couloir, escalier, zone libre.
  - Statistiques projet : compte des chambres, surface estimée.
- **Panneau droit**
  - Bascules de vue : étage ou global avec rappel de la grille.
  - Outils de transformation : déplacement, rotation libre, échelle.
  - Inspecteur détaillé : nommage, rotations guidées, couleurs, tailles rapides, étiquettes, mobilier.
  - Actions de fichier : sauvegarde/chargement et réinitialisation.

## Créer et éditer des espaces
1. **Ajouter des pièces** via la bibliothèque (bouton "Chambre complète", couloir, escalier ou zone libre).
2. **Sélectionner un bloc** pour activer l'inspecteur.
3. **Nommer** la pièce puis valider avec le bouton de confirmation.
4. **Choisir la cible couleur** (badge **Murs** ou **Étiquette**), puis appliquer une teinte.
5. **Ajuster la taille** avec les profils rapides S / M / L ou avec les outils de transformation.

## Mobilier et accessoires
- Section **Objets de la chambre** : ajoutez ou supprimez des meubles prédéfinis (lit, bureau, douche, etc.).
- Section **Dimensions mobilier** : modifiez largeur/hauteur/profondeur et rotation libre (axe Y par défaut).

## Gestion des niveaux
- Utilisez les flèches pour changer d'étage ou dupliquez un niveau pour réutiliser une composition.
- Le badge **Niveau** dans l'inspecteur rappelle en permanence le plan concerné.
- La **vue Global** rend visibles tous les niveaux et verrouille temporairement les transformations pour éviter les maladresses.

## Alignements et rotations guidées
- Sélectionnez un **axe** (X, Y ou Z) puis un **angle prédéfini** (15°, 30°, 45°, 90° ou 180°).
- Cliquez sur **Rotation -** ou **Rotation +** pour appliquer l'angle choisi à l'objet sélectionné.
- Le mode libre reste disponible via l'outil Rotation (`E`) pour les ajustements fins.

## Sauvegarder, charger et réinitialiser
- **Sauver** : exporte un fichier JSON contenant niveaux, couleurs, mobilier et étiquettes.
- **Ouvrir** : recharge un fichier exporté précédemment et restaure l'état complet de la scène.
- **Réinitialiser** : vide la scène et recrée une chambre par défaut (l'historique est également purgé).

## Raccourcis clavier
- `W` : Mode déplacement
- `E` : Mode rotation libre
- `R` : Mode échelle
- `Ctrl/Cmd + Z` : Annuler
- `Ctrl/Cmd + Y` : Rétablir
- `Suppr` ou `Retour arrière` : Supprimer la sélection

## Dépannage rapide
- **Icônes manquantes** : vérifiez la connexion internet (icônes Lucide et Three.js sont chargés via CDN).
- **Palette inactive** : assurez-vous d'avoir sélectionné une pièce (pas un meuble) et que la cible est réglée sur "Murs" ou "Étiquette".
- **Rotations guidées sans effet** : sélectionnez un objet, choisissez un axe et un angle puis cliquez sur Rotation +/- ; un toast de confirmation doit apparaître.
- **Actions grisées** : aucune sélection ou vue globale active ; repassez en vue étage pour modifier des blocs.

Bonne conception !
