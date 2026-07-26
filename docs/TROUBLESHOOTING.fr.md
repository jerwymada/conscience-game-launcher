# Dépannage

## L'application ne démarre pas

- Vérifie que Windows est en x64.
- Installe [.NET 10 Desktop Runtime x64](https://aka.ms/dotnet/10.0/windowsdesktop-runtime-win-x64.exe).
- Installe [Microsoft Edge WebView2 Evergreen Runtime](https://go.microsoft.com/fwlink/p/?LinkId=2124703).
- Pour la version portable, extrais complètement le ZIP.
- Vérifie la somme SHA-256 du téléchargement.

## Windows SmartScreen affiche un avertissement

La version 1.2.1 n'est pas signée. Compare l'empreinte SHA-256 du fichier avec
`downloads/SHA256SUMS.txt`. Ne continue que si elle correspond au fichier
téléchargé depuis ce dépôt.

## Une autre instance est déjà ouverte

Restaure la fenêtre depuis la zone de notification et ferme-la normalement.
L'application autorise une seule interface et un seul helper UAC restreint.

## L'application refuse le mode administrateur

C'est volontaire. Ferme l'instance élevée et utilise le raccourci normal. L'UI,
les jeux et les mods doivent fonctionner avec des droits standards.

## L'UAC est accepté mais le lancement reste bloqué

Lis l'étape en échec. L'acceptation UAC démarre seulement le helper restreint ;
une vérification suivante peut encore échouer. Ouvre Diagnostics et restaure
l'environnement avant de réessayer.

## Le processus du jeu n'est pas détecté

Un launcher officiel peut prendre plusieurs minutes avant de démarrer le vrai
processus du jeu. En Solo, l'isolation reste active pendant cette attente. Pour
un jeu manuel, vérifie que l'EXE choisi est celui du jeu et non un updater.

## Le bouton d'un mod est désactivé

Le lancement nécessite une session Solo active, la détection du processus jeu,
un exécutable de mod présent et un outil qui n'est pas déjà lancé. Utilise
**Add > Add Mod** si la détection automatique n'a pas trouvé d'exécutable.

## La restauration demande une intervention

Garde l'application ouverte, va dans Diagnostics et utilise l'action de
restauration correspondante. Ne démarre pas de session Online tant que les
contrôles hosts, pare-feu, réseau et anti-cheat ne sont pas revenus à un état
correct.

Emplacements des logs :

- Installation : `%LocalAppData%\ConscienceGameLauncher\Logs`
- Portable : `Data\Logs` à côté de l'EXE
