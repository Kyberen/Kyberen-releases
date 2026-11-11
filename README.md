# Kyberen : téléchargements

Kyberen surveille la sécurité des PME. Il lit les journaux Windows et une boîte mail dédiée, détecte les attaques connues et prévient par e-mail. Une personne de l'entreprise décide ensuite. Kyberen tourne entièrement sur votre machine : aucun journal n'est envoyé à l'extérieur.

Ce dépôt ne contient que les installateurs Windows. Le code source de Kyberen n'est pas public.

Site : https://kyberen.com

## Télécharger

**[Dernière version](https://github.com/Kyberen/Kyberen-releases/releases/latest)** : prenez le fichier `Kyberen-Setup-<version>.exe`.

- Windows 10 ou 11, ou Windows Server 2019 ou plus récent, 64 bits.
- L'installation se fait pour votre compte Windows, dans `%LOCALAPPDATA%\Programs\Kyberen`, sans droits administrateur.
- Sans licence, Kyberen démarre en lecture seule.

## Vérifier le fichier avant de le lancer

Chaque version est accompagnée d'un fichier `.sha256`. Dans PowerShell, depuis le dossier du téléchargement :

```powershell
Get-FileHash .\Kyberen-Setup-<version>.exe -Algorithm SHA256
```

Le résultat doit être identique à la valeur écrite dans `Kyberen-Setup-<version>.exe.sha256`. S'il diffère, ne lancez pas le fichier et écrivez à security@kyberen.com.

## Avertissement de Windows

L'installateur n'est pas encore signé. Windows SmartScreen peut afficher « Windows a protégé votre ordinateur » : cliquez sur « Informations complémentaires », puis sur « Exécuter quand même ». Faites-le seulement après avoir vérifié le fichier comme indiqué ci-dessus.

## Contact

- Questions, licence, installation : contact@kyberen.com
- Signaler une faille de sécurité : security@kyberen.com

Kyberen est un logiciel propriétaire. Son utilisation est régie par le contrat de licence.
