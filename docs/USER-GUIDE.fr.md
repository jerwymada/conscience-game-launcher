# Guide utilisateur

## Bibliothèque

Le Dashboard affiche **Games** par défaut. Le sélecteur Games/Mods sous la
recherche permet de changer de bibliothèque.

- **Refresh** relance la détection des jeux et outils de mod connus.
- **Add > Add Game** ajoute manuellement l'exécutable d'un jeu.
- **Add > Add Mod** ajoute un mod, trainer ou gestionnaire de mods.
- La suppression d'un élément manuel se trouve dans son menu kebab.

La suppression retire seulement l'entrée de la bibliothèque. Aucun fichier du
jeu ou du mod n'est effacé. Un élément détecté automatiquement ne peut pas être
supprimé ; un jeu peut être masqué depuis son menu kebab.

## Session Solo

1. Sélectionne un jeu.
2. Choisis **Play Solo**.
3. Accepte la demande UAC lorsqu'une opération Windows protégée est nécessaire.
4. Attends la validation de toutes les étapes et la détection du processus jeu.
5. Lance les outils identifiés depuis la zone **Solo Mods**.
6. Ferme normalement le jeu ou utilise **Abort Session & Restore**.

L'isolation reste active pendant le démarrage différé d'un launcher officiel.
Si tu quittes l'application pendant une session protégée, elle annule d'abord
la session et attend la fin de la restauration.

## Session Online

1. Ferme les outils de mod non gérés par l'application.
2. Sélectionne le jeu et choisis **Play Online**.
3. L'application ferme les outils identifiés, nettoie les traces gérées,
   supprime l'isolation Solo et vérifie le réseau avant le lancement.

Les boutons de lancement des mods sont indisponibles en Online. Ne lance aucun
trainer ou outil de mod manuellement pendant une session Online.

## Réglages

- **Hosts blocking** : active le blocage hosts géré en Solo.
- **Killswitch** : désactive tous les adaptateurs physiques ciblés et annule
  l'opération si l'un d'eux ne peut pas être désactivé.
- **Save backup** : sauvegarde les parties avant la session choisie.
- **Auto Close** : surveille le jeu jusqu'à la fermeture de son processus.
- **Block mod tool Internet access** : maintient des règles pare-feu sortantes
  pour les exécutables des outils de mod enregistrés.
- **Start with Windows** : désactivé par défaut.
- **Minimize to notification area** : désactivé par défaut.

Les réglages sont enregistrés automatiquement et restent sur le PC.

## Diagnostics

L'onglet Diagnostics contrôle le fichier hosts, les règles pare-feu, la
restauration réseau, les services anti-cheat et les règles réseau persistantes
des mods. Utilise l'action de récupération correspondante lorsqu'un contrôle
demande une restauration.
