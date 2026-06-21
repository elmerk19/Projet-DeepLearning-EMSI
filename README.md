# Projet Deep Learning — EMSI Casablanca

Projet de fin de module Deep Learning (4IIR, EMSI Casablanca, 2025–2026).
Implémentation, comparaison et analyse critique de trois familles d'architectures de deep learning sous PyTorch, appliquées à des données réelles de natures différentes.

## Contenu

| Partie | Architecture | Dataset | Tâche |
|---|---|---|---|
| I | MLP | Breast Cancer Wisconsin (569 obs., 30 variables) | Classification binaire tabulaire |
| II | CNN | UCI Digits (1797 images 8×8) | Classification d'images |
| III | RNN / LSTM / GRU / Seq2Seq | Corpus EN–FR (68 paires de phrases) | Modélisation de langage et traduction |

## Structure du dépôt

```
.
├── notebook/
│   └── Projet_DeepLearning_EMSI.ipynb   # Notebook complet, exécuté (code + résultats)
├── rapport/
│   ├── rapport.tex                      # Rapport scientifique complet (LaTeX)
│   ├── rapport.pdf                      # Rapport compilé (24 pages)
│   └── figures/                         # Figures du rapport (courbes, matrices, ablations)
└── README.md
```

## Points clés

- **Partie I (MLP)** : comparaison de 3 stratégies d'initialisation (Xavier/Glorot retenue), 96,5 % d'accuracy test, F1 = 0,972.
- **Partie II (CNN)** : étude d'ablation (padding, stride, pooling, nombre de filtres), vérification manuelle de la corrélation croisée 2D, 97,4 % d'accuracy test (meilleure configuration).
- **Partie III (RNN/LSTM/GRU/Seq2Seq)** : comparaison des trois cellules récurrentes, étude du gradient clipping (BPTT), système encodeur-décodeur avec teacher forcing, décodage glouton vs beam search.

## Environnement

Python 3.11, PyTorch, scikit-learn, NumPy, Matplotlib. Exécution CPU (architectures volontairement compactes).

## Auteur

Elmer — EMSI Casablanca, filière Informatique (4IIR)
