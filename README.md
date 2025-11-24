# Flexilogis Studio 3D

Une expérience 3D ultra-rapide pour concevoir des chambres d'hôtel, couloirs et zones modulaires directement depuis un navigateur moderne. Cette version relookée fournit une interface remaniée, des contrôles de transformation guidés et une documentation complète pour accélérer la prise en main.

## Sommaire
- [Fonctionnalités clés](#fonctionnalités-clés)
- [Démarrage](#démarrage)
- [Parcours de l'interface](#parcours-de-linterface)
- [Création et édition des espaces](#création-et-édition-des-espaces)
- [Mobilier et accessoires](#mobilier-et-accessoires)
- [Gestion des niveaux](#gestion-des-niveaux)
- [Rotation guidée et alignements](#rotation-guidée-et-alignements)
- [Sauvegarde et chargement](#sauvegarde-et-chargement)
- [Raccourcis clavier](#raccourcis-clavier)
- [Dépannage rapide](#dépannage-rapide)

## Fonctionnalités clés
- Interface "glassmorphism" clarifiée : ruban de commande centré, panneaux regroupés et indicateurs contextuels.
- Inspecteur enrichi : badges pour la cible de couleur, niveau courant et type de sélection.
- Palette de couleurs améliorée avec bascule explicite entre murs et étiquettes.
- Rotations guidées avec axes et angles prédéfinis en complément du mode libre.
- Gestion multi-niveaux (création, duplication, navigation étage/global).
- Système d'annulation/rétablissement et toasts d'état intégrés.

## Démarrage
1. Ouvrez `V3.html` dans un navigateur moderne (Chrome, Edge, Firefox) avec internet actif pour charger les dépendances CDN.
2. Attendez la disparition de l'écran de chargement, puis utilisez le clic gauche pour sélectionner et les commandes listées ci-dessous pour manipuler la scène.

## Parcours de l'interface
- **Ruban supérieur** : indique le mode actif, la sélection courante et rappelle les gestes de navigation.
- **Panneau gauche** :
  - Gestion des étages (création, duplication, navigation).
  - Bibliothèque d'objets (chambre complète, couloir, escalier, zone libre).
  - Statistiques projet (nombre de chambres, surface estimée).
- **Panneau droit** :
  - Bascules de vue (étage / global) avec rappel de la grille.
  - Outils de transformation (déplacement, rotation libre, échelle).
  - Inspecteur détaillé : nommage, rotations guidées, couleurs, tailles, étiquettes, mobilier.
  - Actions de fichier (sauvegarde/chargement) et réinitialisation.

## Création et édition des espaces
1. Ajoutez des pièces via la bibliothèque (bouton "Chambre Complète" ou autres modèles).
2. Sélectionnez un bloc pour activer l'inspecteur :
   - **Nom** : renseignez un identifiant puis validez avec le bouton de confirmation.
   - **Couleur** : choisissez d'abord la cible **Murs** ou **Étiquette** (l'état est visible grâce au badge). La palette applique ensuite la teinte sélectionnée.
   - **Taille rapide** : utilisez S / M / L pour ajuster rapidement les proportions du bloc.

## Mobilier et accessoires
- Utilisez la section **Objets de la chambre** pour ajouter ou supprimer des meubles prédéfinis (lits, bureau, douche, etc.).
- La section **Dimensions mobilier** permet d'ajuster largeur/hauteur/profondeur ainsi que la rotation libre (axe Y par défaut).

## Gestion des niveaux
- Les boutons fléchés changent d'étage. Ajoutez ou dupliquez un niveau pour réutiliser des compositions existantes.
- Le badge "Niveau" dans l'inspecteur rappelle en permanence le plan concerné par la sélection.
- La vue **Global** rend visibles tous les niveaux et désactive temporairement les contrôles de transformation pour éviter les maladresses.

## Rotation guidée et alignements
- Dans l'inspecteur, choisissez un **axe** (X, Y ou Z) et un **angle prédéfini** (15°, 30°, 45°, 90°, 180°).
- Utilisez les boutons **Rotation -** ou **Rotation +** pour appliquer l'angle sélectionné au dernier objet choisi.
- Le mode libre de `TransformControls` reste disponible via l'outil Rotation (touche `E`) pour des ajustements fins.

## Sauvegarde et chargement
- **Sauver** : génère un fichier JSON contenant la scène complète (niveaux, couleurs, mobilier, étiquettes).
- **Ouvrir** : recharge un fichier exporté précédemment.
- **Réinitialiser** : vide la scène et recrée une chambre par défaut (l'historique est également purgé).

## Raccourcis clavier
- `W` : Mode déplacement
- `E` : Mode rotation libre
- `R` : Mode échelle
- `Ctrl/Cmd + Z` : Annuler
- `Ctrl/Cmd + Y` : Rétablir
- `Suppr` ou `Retour arrière` : Supprimer la sélection

## Dépannage rapide
- **Icônes manquantes** : vérifiez la connexion internet (icônes Lucide et Three.js sont servis via CDN).
- **Palette inactive** : assurez-vous d'avoir sélectionné une pièce (pas un meuble) et que la cible est réglée sur "Murs" ou "Étiquette" selon le besoin.
- **Rotations guidées sans effet** : sélectionnez un objet, choisissez un axe et un angle puis cliquez sur Rotation +/- ; le toast de confirmation doit apparaître.

Bonne conception !
