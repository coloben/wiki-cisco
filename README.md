# Wiki Cisco

Wiki communautaire en français pour **Cisco's Fantasy Medieval RPG [Ultimate]**, construit avec MkDocs Material.

**Wiki en ligne :** https://coloben.github.io/wiki-cisco/

**Dépôt GitHub :** https://github.com/coloben/wiki-cisco

## Voir le wiki sur son PC

Avec Python installé, ouvrir un terminal dans ce dossier puis lancer :

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
mkdocs serve
```

Ouvrir ensuite l'adresse affichée, normalement `http://127.0.0.1:8000/`.

## Vérifier la construction

```powershell
mkdocs build --strict
```

Le site généré apparaît dans `site/`, dossier volontairement ignoré par Git.

## Publier sur GitHub Pages

1. Créer un dépôt GitHub vide, par exemple `wiki-cisco`.
2. Copier tout le contenu de ce dossier dans le dépôt.
3. Faire le premier commit puis pousser la branche `main`.
4. Sur GitHub, ouvrir **Settings → Pages**.
5. Dans **Build and deployment → Source**, choisir **GitHub Actions**.
6. Ouvrir l'onglet **Actions** et attendre la fin du workflow « Déployer le wiki ».

L'URL finale sera généralement `https://UTILISATEUR.github.io/wiki-cisco/`.

## Mettre l'index des mods à jour

Le fichier `tools/generate_mod_index.py` lit les `.jar`, récupère leur nom dans `META-INF/mods.toml` quand il existe, puis régénère :

- `data/mod-jars.txt` ;
- `data/mods.json` ;
- `docs/mods/index.md` ;
- `docs/mods/fichiers.md`.

Exemple :

```powershell
python tools/generate_mod_index.py "C:\chemin\vers\minecraft\mods"
```

L'export source retrouvé contient **293 entrées de fichiers**, mais l'une d'elles est `arborescence.txt` : l'inventaire vérifié comprend donc **292 fichiers `.jar`**.

