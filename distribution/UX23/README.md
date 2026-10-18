# SINGELAND 3.3.0 — TEST CHAPITRE 4 / UX23

PRE-RELEASE / BETA INTERNE — QA = PARTIAL

Cette distribution reprend exactement les fichiers runtime du candidat Windows UX23 atteste dans TASK-0005. Le jeu n'a pas ete reconstruit. Seul le dossier BurstDebugInformation_DoNotShip, reserve au diagnostic du compilateur Burst et inutile a l'execution, est omis.

## Limites connues
- BUG-0001 : crash natif a la fermeture toujours ouvert (OPEN).
- Android physique non valide ; aucun APK n'est distribue dans cette preversion Windows.
- Manette physique non validee.
- Regression complete C1–C3 non terminee.
- Les controles locaux UX ne constituent pas une QA independante du jeu.

## Tester avec le launcher
1. Telecharger et extraire SingeLand-Launcher-2.2.4-TEST-UX23-Windows.zip dans un nouveau dossier.
2. Ouvrir « SingeLand Launcher TEST UX23.exe » puis choisir volontairement « TEST 3.3.0 · Chapitre 4 / UX23 » dans le menu CANAL.
3. Lire les avertissements et confirmer l'installation du TEST. Aucun jeu n'est telecharge automatiquement en changeant de canal.

Le canal public reste selectionne au demarrage. L'installation TEST et son current.json se trouvent dans un sous-dossier test-ux23, separe de l'installation publique. Le launcher historique n'est pas remplace.

## Retour a la version publique
Choisir « Version publique » ou le bouton « Revenir a la version publique ». La version publique deja installee et ses fichiers sont conserves. Le TEST reste disponible dans son dossier separe. La version publique actuelle est 3.2.5 ; son manifeste et ses archives GitHub sont inchanges.

Les sauvegardes de campagne du jeu restent communes : avant chaque lancement TEST, le nouveau launcher copie les fichiers campagne-v1.json et leurs sauvegardes/archives connus dans son dossier sauvegardes-avant-test. Les originaux ne sont pas modifies par cette copie. La compatibilite d'une progression C4 avec le jeu public 3.2.5 n'est pas validee ; le retour des binaires ne restaure pas automatiquement une ancienne partie. Garder ces copies pour recuperation manuelle si necessaire.

Cette publication sert a l'essai utilisateur. Aucun essai gameplay complet, aucune installation personnelle, aucune publication Google Play ou Microsoft Store ne sont effectues par cette tache.
## Empreintes

7ecc287ae3e80c9325820dad38fe97568fadfeba23150bafeed688ed06176e6e  FILES-UX23-SHA256.json
675cff1d96e3cf53a751c79be0ae9e71a7469547c42945d14e4027b68ffe26b9  manifest-test.json
aaa63ca96acfe1957bc8dae799ca57ac17f75e6b63934dc0d40dff12e897d1a9  Notes-TEST-UX23.txt
075a76b0c0d4f6db24c18142af805f331e8876b9007b2f8ca85def17f17ae456  SingeLand-3.3.0-TEST-UX23-Windows.zip
bdb29d91e56372df0164a21f24025e0f7b9f1a91af0a6fabf85976e82dc77599  SingeLand-Launcher-2.2.4-TEST-UX23-Windows.zip

Commit de cette branche : metadonnees de distribution uniquement. Le candidat de jeu est atteste par TASK-0005 et ses empreintes ; sa revision source exacte n'est pas etablie par ce commit.
