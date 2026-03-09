# Pipeline — De la partie à l'histoire

## Étape 1 : Analyse brute de la partie

Entrée : fichier PGN
Sortie : `stories/game_XX/1_analysis.md`

Objectif : comprendre la partie **en tant que partie d'échecs**, sans penser à l'histoire.

### À identifier :
- **Arc global** : qui domine au début ? Y a-t-il une bascule ? Quand ? Comment ça finit ?
- **Moments clés** (5 à 15) : les coups qui changent tout — sacrifices, captures décisives, erreurs fatales, promotions, mat
- **Pièces protagonistes** : quelles pièces sont les plus actives, les plus décisives ? Quelles pièces ne font rien ?
- **Style** : partie agressive/tactique ? Positionnelle/lente ? Chaotique ? Un côté attaque pendant que l'autre défend ?
- **Ouverture** : quel est son nom ? Quelle atmosphère ça évoque ?
- **Fin** : mat, abandon, nulle ? Comment on en arrive là ?

### Règle : pas de métaphore ici. Juste de l'analyse échiquéenne.

---

## Étape 2 : Cadre narratif

Sortie : `stories/game_XX/2_framework.md`

Objectif : choisir le genre et assigner les rôles.

### 2a. Genre / ton
Le style de la partie (étape 1) suggère un genre :
- Partie tactique agressive → action, fantasy épique, thriller
- Partie positionnelle lente → drame psychologique, thriller cérébral
- Partie avec sacrifice majeur → tragédie, récit héroïque
- Partie avec comeback → récit de rédemption, underdog story
- Partie nulle → drame existentiel, compromis amer

Ce n'est pas rigide. Le genre peut aussi venir d'une envie créative. Mais la partie doit le supporter.

### 2b. Assignation des rôles
Pour chaque pièce **qui compte** dans cette partie :
1. Consulter `reference/pieces.md` pour ses propriétés intrinsèques
2. Choisir une transposition qui sert le genre ET le rôle de cette pièce dans CETTE partie spécifique
3. **Justifier** : pourquoi cette association ? (propriétés intrinsèques + comportement dans la partie)

### Règles :
- Les pièces inactives = figurants ou absentes du récit. Ne pas forcer.
- Les deux camps ne sont pas nécessairement "bien" vs "mal". Choisir la dualité qui sert l'histoire.
- Les relations entre pièces (voir `reference/dynamics.md`) définissent les relations entre personnages.

---

## Étape 3 : Synopsis

Sortie : `stories/game_XX/3_synopsis.md`

Objectif : écrire le résumé complet de l'histoire en 1-2 pages AVANT d'écrire.

### À faire :
1. Lister les moments clés de la partie (étape 1)
2. Transposer chaque moment en scène narrative grâce aux rôles (étape 2) et aux événements (`reference/events.md`)
3. Rédiger le synopsis : début → développement → climax → dénouement

### Test de cohérence (CRITIQUE) :
Relire le synopsis en se posant ces questions :
- [ ] Est-ce que l'histoire tient debout **sans savoir qu'elle vient d'une partie d'échecs** ?
- [ ] Les motivations des personnages sont-elles crédibles ?
- [ ] Les retournements sont-ils "earned" (préparés narrativement) ou sortent-ils de nulle part ?
- [ ] Le ton est-il cohérent du début à la fin ?
- [ ] Y a-t-il des personnages/éléments qui apparaissent et disparaissent sans raison ?

Si une réponse est non → ajuster les assignations (étape 2) ou regrouper/supprimer des moments.

---

## Étape 4 : Écriture

Sortie : `stories/game_XX/4_story.md`

Objectif : écrire l'histoire complète.

### Principes :
- **Regrouper les coups** — un chapitre n'est pas un coup. Plusieurs coups forment une scène.
- **Le rythme suit la partie** — ouverture calme = exposition posée. Milieu tactique = tempo qui s'accélère. Finale = tension maximale ou intimité.
- **Les captures sont des scènes, pas des mentions** — chaque capture importante mérite sa scène.
- **Les coups anodins = ellipses narratives** — "les semaines passèrent" plutôt que de forcer un sens à chaque coup.
- **Montrer, ne pas dire** — le lecteur ne doit jamais sentir le mécanisme échiquéen derrière.

---

## Étape 5 : Relecture de cohérence

Checklist finale :
- [ ] Un lecteur non-joueur d'échecs comprendrait-il et apprécierait-il cette histoire ?
- [ ] Les retournements de l'histoire correspondent-ils aux retournements de la partie ?
- [ ] Aucun personnage n'agit de manière incohérente pour "coller" à la partie ?
- [ ] L'histoire a-t-elle sa propre identité, ou sent-on qu'elle est "générée" ?
- [ ] Relire la partie d'échecs en parallèle : les grands moments sont-ils tous là ?

Si tout est bon → publication dans `stories/game_XX/4_story.md` (version finale).
