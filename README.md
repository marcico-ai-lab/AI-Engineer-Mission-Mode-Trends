# Installation du projet

## Prérequis

- Un environnement compatible avec les notebooks Jupyter (VS Code, JupyterLab, etc.)
- [Git](https://git-scm.com/)
- [UV](https://docs.astral.sh/uv/getting-started/installation/) pour la gestion de Python et des dépendances
- Un compte [Hugging Face](https://huggingface.co/) avec un token d'accès à l'API d'inférence

## 1. Cloner le dépôt

```bash
git clone git@github.com:marcico-ai-lab/AI-Engineer-Mission-Mode-Trends.git
cd AI-Engineer-Mission-Mode-Trends
```

## 2. Installer les dépendances

```bash
uv sync
```

UV installe la version de Python requise si nécessaire, crée l'environnement virtuel `.venv` et installe les dépendances définies dans `pyproject.toml`.

## 3. Configurer le token Hugging Face

Créer un fichier `.env` à la racine du projet :

```dotenv
HUGGING_FACE_TOKEN=votre_token_hugging_face
```

Le fichier `.env` est exclu du dépôt Git.

## 4. Ajouter les images

Créer le dossier `data/images/` à la racine du projet et y placer les images à analyser au format `.jpg` ou `.png`.

## 5. Exécuter le notebook

1. Ouvrir `huggingface_clothes_segformer.ipynb`.
2. Sélectionner le noyau Python de l'environnement virtuel `.venv`.
3. Ajuster la variable `MAX_IMAGES` selon le nombre d'images à traiter.
4. Exécuter les cellules du notebook dans l'ordre.
