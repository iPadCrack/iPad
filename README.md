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
   
7) Supprimez "profile-58a3e6aebe69b06efc831fe5c7d8100beb27dcc67222a985e77dd193f4ba7e6a.xml" et "profile-9c39fa2c22c1bfce337e0c01990d1a7359198a5a78d79ce87eb88ca0a2eabfca.xml"

![image](https://github.com/user-attachments/assets/11581db3-eb96-4776-a78a-f1f970072765)

8) Fermez iBackupBot

9) Cherchez le dossier de la sauvegarde modifiée et déplacez-la dans "%appdata%\Apple Computer\MobileSync\Backup"

![image](https://github.com/user-attachments/assets/27df34d7-11a9-4635-a158-b82f817ec953)

10) Ouvrez iTunes et accédez à l'interface de l'iPad

![image](https://github.com/user-attachments/assets/674ae4df-ab27-4064-a174-c94a48d90e8f)

11) Restaurez la sauvegarde

![image](https://github.com/user-attachments/assets/3400ebdf-0623-4817-b1a1-0765cfeacfda)

12) Tapez votre code sur l'iPad pour confirmer la restauration

13) Fermez iTunes

14) Installez vos applications depuis l'App Store, puis cachez-les en appuyant sur 'Exiger Touch ID'

![image](https://github.com/user-attachments/assets/40453814-891e-4488-90f7-db724ca9f3c4)

## Partie 2 : Maintenant que vos application sont installer, il faut resychroniser les profiles de sécurité (aussi afin de cacher les racourcis web qui pourrez vous faire distinguer d'un iPad normal)

15) Supprimez les sauvegardes dans "%appdata%\Apple Computer\MobileSync\Backup"

16) Faites une nouvelle sauvegarde de l'iPad (refaite les étapes 2 à 4)

17) Naviguez sur iBackupBot dans System Files > SysSharedContainerDomain-systemgroup.com.apple.configurationprofiles > Library > Configuration Profiles

18) Supprimez "HomeScreenLayout.plist"

19) Restaurez la nouvelle sauvegarde (étapes 8 à 12)

20) Vos applications sur l'accueil seront toutes désorganisées. Il faudra patienter pour qu'elles se remettent automatiquement en place.

### Tout devrait être bon. Si vous voulez installer à nouveau d'autres applications, vous pouvez refaire toutes les étapes, mais vous n'aurez plus qu'à supprimer "profile-9c39fa2c22c1bfce337e0c01990d1a7359198a5a78d79ce87eb88ca0a2eabfca.xml" dans l'étape 7.
