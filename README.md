# CNN_catsdogs-AbdouSalamNIANG
readme_text = """# CNN vs Transfer Learning — Cats vs Dogs (Nom Prenom)

## Objectif
Comparer un CNN entraîné from-scratch et un modèle en transfer learning sur le même jeu de données (Cats vs Dogs).

## Environnement
Python >= 3.8
pip install -r requirements.txt

## Organisation des données
Télécharger le dataset Cats vs Dogs (Kaggle ou source fournie en cours) et placer :
data/cats-vs-dogs/train/
data/cats-vs-dogs/val/
data/cats-vs-dogs/test/

## Commandes exemples
# From scratch (Adam)
python train.py --experiment scratch --optimizer adam --lr 1e-3 --epochs 20 --batch_size 32 --data_dir data/cats-vs-dogs --checkpoint_path best_scratch.pth

# Transfer learning (freeze backbone)
python train.py --experiment transfer --freeze_backbone --optimizer sgd --lr 1e-3 --epochs 12 --batch_size 32 --checkpoint_path best_transfer_freeze.pth

## Résultats attendus
Présenter courbes : loss/accuracy/precision/recall pour train & val pour les deux expériences.
Inclure matrice de confusion et discussion résumée (2-3 paragraphs).

## .gitignore (extrait)
data/
*.pth
runs/
__pycache__/

## Notes
- Ne pas pousser les modèles (.pth) ni les données sur GitHub.
"""
with open('README_PROJECT.md','w',encoding='utf-8') as f:
    f.write(readme_text)
print('README_PROJECT.md créé dans le workspace.')
