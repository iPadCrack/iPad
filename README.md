# Installer les applications que vous voulez sur l'iPad

## À lire avant de commencer

Ce guide est fourni uniquement à des fins éducatives et informatives. Il a pour but d'expliquer le fonctionnement des outils mentionnés et ne doit en aucun cas être utilisé pour contourner des restrictions mises en place par un établissement ou une organisation.

L'utilisation des méthodes décrites relève de la seule responsabilité de la personne qui les applique. En aucun cas, je ne peux être tenu responsable des conséquences, directes ou indirectes, liées à leur utilisation.

En poursuivant la lecture et/ou en appliquant ces étapes, vous reconnaissez agir en pleine connaissance de cause et sous votre entière responsabilité.

## Applications requises :

iTunes: https://www.apple.com/itunes/download/win64/

iBackupBot: https://www.icopybot.com/ibackupbot_setup.exe

## Partie 1 : Retirer les restrictions de l'AppStore

1) Déconnectez le compte Apple du lycée dans les réglages (vous devrez créer votre propre compte Apple)

2) Lancez iBackupBot, branchez l'iPad, puis cliquez sur 'Backup Now'

![vlc_dOB9yqqMYZ](https://github.com/user-attachments/assets/b329f639-2421-4d79-ad20-49a4f42ca94a)

3) Choisissez le chemin où vous allez faire la sauvegarde

![image](https://github.com/user-attachments/assets/9cae5f52-7100-418c-b9de-1e6e3f4fdb09)

4) Quand la sauvegarde est terminée, ouvrez-la dans l'application

5) Faites des copies de la sauvegarde si vous souhaitez la restaurer plus tard

6) Naviguez sur iBackupBot (en cliquant sur le "+" à gauche de la backup) dans System Files > SysSharedContainerDomain-systemgroup.com.apple.configurationprofiles > Library > Configuration Profiles
   
7) Supprimez les fichiers suivants :
   - `profile-58a3e6aebe69b06efc831fe5c7d8100beb27dcc67222a985e77dd193f4ba7e6a.xml`
   - `profile-9c39fa2c22c1bfce337e0c01990d1a7359198a5a78d79ce87eb88ca0a2eabfca.xml`

![image](https://github.com/user-attachments/assets/11581db3-eb96-4776-a78a-f1f970072765)

8) Fermez iBackupBot

9) Faites Windows + R et taper "%appdata%". Ensuite, vous aurez sois un dossier "Apple" ou "Apple Computer" selon votre ordinateur. Aller dedans, puis dans "MobileSync", puis "Backup". Déplacer votre backup modifier dans ce dossier (celle que vous avez créée à l’étape 3)
    - ⚠️ Si des dossiers sont déjà présents dans le dossier "Backup" de Apple, supprimez-les ou déplacez-les autre part pour éviter toute confusion lors de la restauration.

![image](https://github.com/user-attachments/assets/27df34d7-11a9-4635-a158-b82f817ec953)

10) Ouvrez iTunes et accédez à l'interface de l'iPad

![image](https://github.com/user-attachments/assets/674ae4df-ab27-4064-a174-c94a48d90e8f)

11) Restaurez la sauvegarde

![image](https://github.com/user-attachments/assets/3400ebdf-0623-4817-b1a1-0765cfeacfda)

12) Tapez votre code sur l'iPad pour confirmer la restauration

13) Quand la restauration est terminé, fermez iTunes

14) Installez vos applications depuis l'App Store, puis cachez-les en appuyant sur 'Exiger Touch ID' sur l'icon.

*Info: Vous pourrez utiliser le cloud gaming xbox en suivant ce tuto: https://better-xcloud.github.io/safari/*

## Partie 2 : Maintenant que vos application sont installer, il faut resychroniser les profiles de sécurité
### Vous avez peut-être remarqué des raccourcis web spécifiques aux iPads des enseignants, qui pourraient faire distinguer d'un iPad normal. Il est donc fortement recommandé de réappliquer les profils de sécurité pour masquer cette différence.

15) Faites une nouvelle sauvegarde de l'iPad en répétant les étapes 2 à 4

16) Naviguez sur iBackupBot dans System Files > SysSharedContainerDomain-systemgroup.com.apple.configurationprofiles > Library > Configuration Profiles

17) Supprimez le fichier `HomeScreenLayout.plist`

18) Restaurez la nouvelle sauvegarde modifiée en répétant les étapes 8 à 13
    - ➡️ Lors de l'étape 9, supprimez d'abord tout le contenu du dossier Backup (comme indiqué dans l'avertissement), puis placez-y votre nouvelle sauvegarde.

20) Vos applications sur l'écran d'accueil seront toutes désorganisées. Il faudra patienter pour qu'elles se remettent automatiquement en place.

## Notes

* ⚠️ Il n’y aura pas de mise à jour automatique des applications installées. Vous devrez refaire une sauvegarde via iTunes, puis la restaurer sans rien modifier pour que les mises à jour se fassent automatiquement pendant la restauration.

- ⚠️ Les signet web tel que Amazon Luna et GeForce NOW (cloud gaming) ne fonctionneront plus après avoir remis les sécurité en place. Seul le cloud gaming de Xbox peut fonctionner en suivant l'info en dessous de l'étape 14.

* Vous pourrez cacher les application FaceTime et Itunes Store en allant dans Réglages > Temps d'écran > Contenu et confidentialité > Apps et fonctionnalités approuvées puis en décochant les applications que vous souhaitait cacher.
  
* Si vous voulez installer à nouveau d'autres applications, vous devrais refaire toutes les étapes, mais vous n'aurez plus qu'à supprimer "profile-9c39fa2c22c1bfce337e0c01990d1a7359198a5a78d79ce87eb88ca0a2eabfca.xml" dans l'étape 7.
