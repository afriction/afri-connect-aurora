# Afri Connect Aurora
**Retrouvez vos Looks et filtres Aurora sur votre Mac à puce Apple Silicon.**

Creative Tools by **Robin Kapka** · Suite **Afri-Plugin**

**[Télécharger gratuitement l’installateur Mac](https://github.com/afriction/afri-connect-aurora/releases/latest)**

## Pourquoi cet outil ?
L’ancien plugin Photoshop d’Aurora HDR est conçu pour Intel et ne se charge pas dans Photoshop natif sur Apple Silicon. Afri Connect Aurora rétablit le transfert entre les deux applications, en utilisant Aurora HDR installé sur votre Mac.

Vous retrouvez le véritable écran **Créer HDR**, les Looks et les filtres d’Aurora. Après **Appliquer**, le résultat revient automatiquement dans Photoshop sous forme d’un **nouvel objet dynamique**. Le document source reste intact.

## Prérequis et configurations testées
- Mac **Apple Silicon**, macOS **12 ou ultérieur** pour le lanceur.
- **Photoshop** et **Aurora HDR 2019** déjà installés, fonctionnels et utilisés avec leurs licences respectives.
- Rosetta doit permettre à l’application Aurora Intel de fonctionner.
- Validation locale : **Photoshop 27.6.0**, **Aurora HDR 1.0.2 (6495)**.
- Transfert RVB **8 et 16 bits** validé. Les autres versions et configurations ne sont pas garanties.

L’outil ne réécrit pas Aurora pour Apple Silicon : il connecte Photoshop natif à l’application Aurora existante.

## Installation
1. Ouvrez la rubrique [Releases](https://github.com/afriction/afri-connect-aurora/releases/latest).
2. Téléchargez **Afri-Connect-Aurora-Mac.zip** puis décompressez-le.
3. Ouvrez **Installer Afri Connect Aurora.app**.
4. Vérifiez les applications détectées et cliquez sur **Installer**.
5. Si macOS demande une autorisation, autorisez le contrôle de Photoshop pour charger l’action.
6. Cliquez sur **Commencer**.

Le lanceur s’installe dans votre Bibliothèque utilisateur ; aucun mot de passe administrateur n’est nécessaire.

**Signature de l’application :** signature locale ad hoc, sans notarisation Apple. Les contrôles macOS peuvent empêcher son ouverture sur une autre machine. Cette première publication sert aussi à recueillir les retours de compatibilité.

## Utilisation
1. Ouvrez votre image dans Photoshop.
2. **Fenêtre → Actions → Afri Connect Aurora**, puis lancez l’action. Raccourci : **⌘ Maj F12**, avec **Fn** si nécessaire.
3. Dans Aurora, cliquez sur **Créer HDR**.
4. Choisissez un Look, ajustez les filtres puis cliquez sur **Appliquer**.
5. Le résultat revient dans Photoshop dans un nouvel objet dynamique.

**Annuler** quitte sans ajouter de résultat. L’ouverture d’Aurora peut prendre un moment.

## Désinstallation
Relancez l’installateur. Si une installation précédente est détectée, le bouton **Désinstaller** apparaît. Après confirmation, le lanceur et l’action sont retirés ; une sauvegarde locale conserve les fichiers de transfert. Aurora, Photoshop et vos images restent en place.

## Limites
- Le transfert utilise le **composite visible du document**, pas uniquement le calque sélectionné.
- La copie envoyée à Aurora est aplatie. Le document source et ses objets dynamiques sont conservés.
- Le résultat est un objet dynamique contenant le rendu ; les réglages Aurora ne sont pas exposés comme filtre dynamique Photoshop.
- Une session à la fois. Ne fermez pas et ne modifiez pas le document source pendant le traitement.
- Les très grandes images, les plans de travail et les autres modes colorimétriques ne sont pas validés.

## Retours
Signalez un problème dans [Issues](https://github.com/afriction/afri-connect-aurora/issues) en indiquant vos versions de macOS, Photoshop et Aurora, la puce de votre Mac et les étapes du problème. Retirez les informations personnelles de vos captures et journaux.

## Distribution
Téléchargement et utilisation gratuits, sans limite ajoutée par le lanceur. Ce dépôt propose la documentation et l’installateur, **sans publier les sources de développement**. L’installateur contient les scripts nécessaires à son fonctionnement dans Photoshop.

Solution indépendante créée par Robin Kapka. Aucune affiliation ni approbation d’Adobe, d’Apple ou de Skylum n’est revendiquée. Photoshop et Aurora HDR ne sont pas inclus ; seuls les composants de la passerelle et leurs ressources d’interface sont distribués.

**Creative Tools by Robin Kapka**
