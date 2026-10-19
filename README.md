# Afri Connect Aurora

[Français](#francais) · [English](#english)

<a id="francais"></a>
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

---

<a id="english"></a>
## English
**Bring your Aurora Looks and filters back to Photoshop on an Apple Silicon Mac.**

Creative Tools by **Robin Kapka** · **Afri-Plugin**

### Free download
[Download the Mac installer](https://github.com/afriction/afri-connect-aurora/releases/latest)

### What it does
Afri Connect Aurora is an independent bridge between native Photoshop and your existing Aurora HDR installation. It opens Aurora's original **Create HDR** workflow, Looks and filters, then brings the rendered result back into Photoshop as a **new Smart Object**, preserving the source document.

This is an action-based workflow, not a native rebuild of Aurora or its old Intel Photoshop plugin. Aurora itself still needs to run through Rosetta.

### Requirements and tested setup
- Apple Silicon Mac; macOS 12 or later for the launcher.
- Working, separately licensed installations of **Photoshop** and **Aurora HDR 2019**.
- Tested locally with **Photoshop 27.6.0** and **Aurora HDR 1.0.2 (6495)**.
- RGB 8-bit and 16-bit transfers tested. Other versions and configurations remain unverified.
- The app is ad hoc signed and **not notarized by Apple**. macOS may block its opening on another Mac.

### Install
1. Download **Afri-Connect-Aurora-Mac.zip** from [Releases](https://github.com/afriction/afri-connect-aurora/releases/latest) and unzip it.
2. Open **Installer Afri Connect Aurora.app**. The installer interface is currently in French.
3. Check the detected applications and click **Installer**.
4. If macOS asks, allow the installer to control Photoshop so it can load the action.
5. Click **Commencer** to finish and show Photoshop.

No administrator password is required.

### Use
1. Open your image in Photoshop.
2. Choose **Window → Actions → Afri Connect Aurora**, then play the action. Shortcut: **Command + Shift + F12**, with Fn if required.
3. In Aurora, click **Create HDR**.
4. Pick a Look, adjust filters and click **Apply**.
5. The rendered image returns to Photoshop as a new Smart Object.

Cancel exits without adding a result. Aurora may take a little time to open.

### Uninstall
Run the installer again. **Désinstaller** appears when an earlier installation is detected in a managed location. Confirm to remove the launcher and Photoshop action. Transferred files are retained in a local backup. Photoshop, Aurora and your images are kept.

### Scope and limitations
The bridge transfers the **document's visible composite**, not only the selected layer. The transfer copy is flattened; the original document and its Smart Objects remain intact. The returned Smart Object contains the render, not editable Aurora filter settings. Process one session at a time and keep the source document open and unchanged. Artboards, very large images and other color modes are not validated. This tool does not merge a bracketed exposure sequence inside Photoshop and does not fix Aurora failing to launch as a standalone app.

### Feedback and distribution
[Report issues](https://github.com/afriction/afri-connect-aurora/issues) with your macOS, Photoshop and Aurora versions, Mac chip and reproduction steps. Remove personal information from screenshots or logs.

Download and use are free, with no limits added by the launcher. This repository contains documentation and the installer, **not the development sources**. Runtime Photoshop scripts are included inside the installer because they are required for the tool to function.

Independent solution by Robin Kapka. No affiliation with or endorsement by Adobe, Apple or Skylum is claimed. Photoshop and Aurora HDR are not included.

**Creative Tools by Robin Kapka**
