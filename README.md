# motorstorm-split-screen-fix

Profil RPCS3 pour corriger les problèmes d’affichage en écran partagé de **MotorStorm: Pacific Rift**, sans supprimer les ombres ni les effets.

**Cause probable :** le preset automatique de RPCS3 peut imposer `MSAA: Disabled` malgré les réglages globaux. Un profil personnalisé du jeu évite ce remplacement.

**Pour le jeu BCES00129, mise à jour 1.03.**

## Installation rapide

1. Clique sur **Code → Download ZIP** en haut de ce dépôt, puis décompresse l’archive.
2. **Ferme RPCS3.** Copie [`config_BCES00129.yml`](config_BCES00129.yml) dans le dossier suivant de ton installation RPCS3 :

   ```text
   config/custom_configs/config_BCES00129.yml
   ```

   Crée `custom_configs` si nécessaire. **Si le fichier existe déjà, sauvegarde-le avant de le remplacer.**

3. Rouvre RPCS3 et **double-clique sur le jeu comme d’habitude**. Les réglages s’appliquent automatiquement.

**Aucun `.cmd`, terminal ou script n’est nécessaire.** Ne lance pas le jeu avec l’option qui ignore sa configuration personnalisée.

## À savoir

- **Définition :** le profil utilise le rendu **1440p**. Pour alléger la charge, remplace `Resolution Scale: 200` par `Resolution Scale: 100` (720p).
- **Quatre joueurs :** dans les réglages de manettes de RPCS3, affecte une manette différente à chacun des ports 1 à 4. Aucun profil de manettes personnel n’est remplacé par ce fichier.
- **Autre édition du jeu :** ce fichier est spécifique à **BCES00129**. Il n’est pas appliqué automatiquement aux autres identifiants.
- **Retour arrière :** ferme RPCS3 et restaure ton ancien profil. Si aucun profil n’existait avant, retire simplement celui ajouté ici.

Ce dépôt contient uniquement le guide et les réglages ; aucun jeu, firmware ou fichier modifié de RPCS3.

### Références

- [Réglages AA/AF et problèmes d’écran partagé](https://github.com/RPCS3/rpcs3/issues/14758)
- [Priorité des profils personnalisés dans RPCS3](https://github.com/RPCS3/rpcs3/blob/6c44fff7549e941389a4ce072a95c5ff9db7237c/rpcs3/Emu/System.cpp#L1813-L1863)
