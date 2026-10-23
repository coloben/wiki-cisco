# Fiabilité du wiki

Ce wiki sépare volontairement ce qui est **confirmé dans l'instance** de ce qui doit encore être testé ou documenté.

## Les trois états

- **Vérifié — fichiers installés** : information lue dans le nom du `.jar`, `META-INF/mods.toml`, les données JSON du mod ou la configuration de l'instance.
- **Vérifié — guide intégré** : information également présente dans un livre ou une traduction livrée avec l'instance.
- **À compléter** : le mod est présent, mais aucune mécanique n'est affirmée tant que sa fiche n'a pas été contrôlée.

## Sources locales utilisées

- l'inventaire `arborescence.txt` du dossier `minecraft/mods` ;
- les métadonnées embarquées dans les `.jar` ;
- `Apotheosis-1.19.2-6.5.2.jar`, notamment ses données de gemmes, traductions et avancements ;
- `config/apotheosis/apotheosis.cfg`, qui confirme l'activation du module Aventure ;
- le guide français Apotheosis installé via Paxi dans l'instance.

## Limites importantes

Un nom de fichier confirme la présence d'un mod, pas que toutes ses fonctions sont accessibles sur le serveur. Les recettes et valeurs peuvent aussi être modifiées par KubeJS, CraftTweaker, datapacks ou configuration. Pour cette raison, le wiki conseille **JEI en jeu** pour les recettes et évite de recopier des recettes non vérifiées.

## Images et licences

L'illustration de l'accueil a été créée spécialement pour ce wiki. Les petites icônes d'objets sont extraites des versions exactes installées afin d'éviter de montrer un objet d'une autre version :

- **Apotheosis 6.5.2**, par Shadows_of_Fire — licence MIT ;
- **Tom's Simple Storage 1.5.11**, par tom5454 — licence MIT ;
- **Nature's Compass 1.10.0** et **Explorer's Compass 1.3.0**, par ChaosTheDude — licence CC BY-NC-SA 4.0.

Ces textures servent uniquement à reconnaître les objets concernés. Les mods et leurs illustrations restent attribués à leurs auteurs.

## Corriger une page

Pour compléter une mécanique, noter idéalement :

1. le nom de l'objet affiché en jeu ;
2. le nom du mod indiqué dans l'infobulle ;
3. la recette visible dans JEI ;
4. une capture ou un test reproductible ;
5. la version du `.jar` concerné.

