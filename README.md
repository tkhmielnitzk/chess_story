# Chess Story

Transformer des parties d'échecs réelles en histoires narratives.

Chaque pièce, chaque mouvement, chaque capture porte en elle une infinité de métaphores. Une partie d'échecs n'est pas qu'un jeu — c'est un squelette dramatique prêt à recevoir la chair d'un récit.

## Principe

1. On part d'une partie réelle (format PGN)
2. On analyse sa structure dramatique
3. On assigne des rôles narratifs aux pièces selon leurs propriétés intrinsèques
4. On transpose les événements de la partie en scènes d'une histoire
5. L'histoire doit tenir debout **sans aucune connaissance des échecs**

## Structure

```
reference/       → Propriétés des pièces, événements et dynamiques
pipeline.md      → Les étapes de transposition
games/           → Parties au format PGN
stories/         → Histoires générées (un dossier par partie)
```
