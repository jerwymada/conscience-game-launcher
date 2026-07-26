# Conscience Game Launcher

**Conscience Game Launcher** prépare, surveille et restaure des sessions de jeu
Solo ou Online plus sûres sous Windows. L'application réunit lancement des
jeux, gestion des outils de mod, isolation réseau, diagnostics et récupération
locale.

> [Read in English](README.md)

## Téléchargement

| Édition | Recommandée pour | Téléchargement |
|---|---|---|
| Setup | La majorité des utilisateurs. Installation en un clic et installation automatique des prérequis. | [Télécharger le Setup 1.2.1](downloads/ConscienceGameLauncher-Setup-v1.2.1.exe) |
| Portable | Une utilisation depuis un dossier autonome ou un support amovible. Les runtimes Microsoft doivent déjà être installés. | [Télécharger la version Portable 1.2.1](downloads/ConscienceGameLauncher-v1.2.1-portable-win-x64.zip) |

Prérequis :

- Windows 10 ou Windows 11, x64
- [.NET 10 Desktop Runtime, x64](https://aka.ms/dotnet/10.0/windowsdesktop-runtime-win-x64.exe)
- [Microsoft Edge WebView2 Evergreen Runtime](https://go.microsoft.com/fwlink/p/?LinkId=2124703)

Le Setup télécharge automatiquement les prérequis Microsoft manquants.

## Fonctions principales

- Détection des jeux installés via les launchers officiels compatibles et les
  exécutables Windows classiques.
- Maintien de l'isolation Solo pendant le démarrage différé d'un launcher.
- Vérification et restauration du pare-feu, du fichier hosts et des adaptateurs.
- Détection prudente des gestionnaires de mods et trainers connus.
- Lancement manuel des outils de mod uniquement après détection du jeu en Solo.
- Fermeture des outils de mod identifiés avant une session Online.
- Demande UAC ciblée pour les opérations Windows protégées.
- Stockage local uniquement, sans vérification distante des mises à jour.
- Diagnostics et actions de récupération intégrés.

## Bien démarrer

1. Consulte le [guide d'installation](docs/INSTALLATION.md).
2. Suis le [guide utilisateur](docs/USER-GUIDE.fr.md).
3. Vérifie le téléchargement avec le
   [guide des sommes SHA-256](docs/VERIFY-DOWNLOADS.md).
4. Consulte le [dépannage](docs/TROUBLESHOOTING.fr.md) en cas de problème.

## Avertissement

L'application réduit les risques de mélange accidentel entre modding Solo et
jeu Online, mais elle ne peut garantir la compatibilité avec tous les jeux,
anti-cheats, launchers, mods ou règlements d'éditeur. Respecte toujours les
règles du jeu et de la plateforme. Ne lance aucun outil de mod en Online.

## Données et confidentialité

L'application n'envoie aucun jeu, mod, réglage ou diagnostic vers un serveur.

- Édition installée : `%LocalAppData%\ConscienceGameLauncher`
- Édition portable : dossier `Data` à côté de l'exécutable

La version 1.2.1 n'est pas signée numériquement. Vérifie toujours les empreintes
publiées dans [SHA256SUMS.txt](downloads/SHA256SUMS.txt).

Copyright © 2026 JERWY. Tous droits réservés.
