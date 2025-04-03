# Installer les application que vous voulez sur l'iPad

Application requises:
iTunes: https://www.apple.com/itunes/download/win64/
iBackupBot: https://www.icopybot.com/ibackupbot_setup.exe

1) Déconnecter le compte Apple du lycée dans les réglages (vous devrez créer votre propre compte Apple)

2) Lancer iBackupBot puis brancher l'iPad, puis clicker sur Backup Now
![vlc_dOB9yqqMYZ](https://github.com/user-attachments/assets/b329f639-2421-4d79-ad20-49a4f42ca94a)

3) Choisisser un chemin où vous aller faire la backup
![image](https://github.com/user-attachments/assets/9cae5f52-7100-418c-b9de-1e6e3f4fdb09)

4) Quand la backup est terminée, charger la
![image](https://github.com/user-attachments/assets/28f52e57-4fad-46ec-b403-fed9f8d8cf89)

5) Fait des copies de la backup si vous souhaiter la restaurer plus tard

6) Naviguer sur iBackupBot dans System Files > SysSharedContainerDomain-systemgroup.com.apple.configurationprofiles > Library > Configuration Profiles
   
7) Supprimer "profile-58a3e6aebe69b06efc831fe5c7d8100beb27dcc67222a985e77dd193f4ba7e6a.xml" et "profile-9c39fa2c22c1bfce337e0c01990d1a7359198a5a78d79ce87eb88ca0a2eabfca.xml"

![image](https://github.com/user-attachments/assets/11581db3-eb96-4776-a78a-f1f970072765)

8) Fermer iBackupBot

9) Chercher le dossier de la backup modifier, et déplacer la dans "%appdata%\Apple Computer\MobileSync\Backup"
![image](https://github.com/user-attachments/assets/27df34d7-11a9-4635-a158-b82f817ec953)

10) Ouvrez iTunes et ouvrer l'interface de l'iPad
![image](https://github.com/user-attachments/assets/674ae4df-ab27-4064-a174-c94a48d90e8f)

11) Restaurer la sauvegarde
![image](https://github.com/user-attachments/assets/3400ebdf-0623-4817-b1a1-0765cfeacfda)

12) Taper votre code sur l'iPad pour confirmer la restauration

13) Installer vos application, puis cacher les en appuyant sur "Exiger Touch ID"

14) Supprimer les backup dans "%appdata%\Apple Computer\MobileSync\Backup"

15) Refaite une backup de l'iPad (refaite les étapes 2 à 4)

16) Naviguer sur iBackupBot dans System Files > SysSharedContainerDomain-systemgroup.com.apple.configurationprofiles > Library > Configuration Profiles

17) Supprimer "HomeScreenLayout.plist"

18) Restaurer la nouvelle backup de nouveau (étapes 8 à 12)

19) Vos application sur l'accueil seront tout déranger, il faudra juste patienter pour qu'elle se remettent automatiquement.
