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

## Étape 4 : Densification — Chasse au flou

Sortie : `stories/game_XX/4_densification.md`

Objectif : relire le synopsis et identifier chaque zone **vague, générique ou trop facile**, puis la rendre concrète et crédible.

### Méthode :

1. **Scanner le synopsis** — repérer chaque passage qui pourrait s'appliquer à n'importe quelle histoire (phrases creuses, raccourcis narratifs, détails manquants, motivations floues, mécanismes non expliqués).

2. **Classer chaque zone floue** dans l'une de ces catégories :
   - **Décor vague** — un lieu, une institution, une entreprise qui manque de chair (ex : "un cabinet d'avocats" → lequel ? combien de personnes ? quelle réputation ? quel étage ?)
   - **Mécanisme non expliqué** — un événement narratif qui arrive sans qu'on comprenne le COMMENT technique/concret (ex : "il perd son appartement" → par quelle procédure exactement ? quel délai ? quelles étapes ?)
   - **Personnage carton** — un personnage dont on ne comprend pas la motivation profonde, ou dont le comportement est trop archétypal (ex : "le PDG arrogant" → pourquoi est-il arrogant ? qu'est-ce qui l'a rendu comme ça ?)
   - **Raccourci émotionnel** — un moment censé être fort mais qu'on RACONTE au lieu de le MONTRER (ex : "Marc est effondré" → qu'est-ce qu'il fait concrètement à ce moment-là ? il mange quoi ? il dort où ?)
   - **Fait technique vague** — un élément scientifique, juridique, médical, technique qui sonne bien mais manque de précision (ex : "les données montrent un problème" → quelles données ? quel format ? quel chiffre ?)

3. **Pour chaque zone identifiée, enrichir** en utilisant l'une des deux approches :
   - **Imagination guidée** — inventer un détail concret, sensoriel, spécifique qui ancre la scène dans le réel (un nom de rue, un bruit, un geste, un chiffre)
   - **Inspiration factuelle mélangée** — s'inspirer de faits réels (scandales, procès, événements documentés) en les MÉLANGEANT : prendre le mécanisme d'une affaire, le contexte d'une autre, le dénouement d'une troisième. Ne jamais reproduire une affaire à l'identique. Le but est la vraisemblance, pas le documentaire.

### Format du document :

Pour chaque zone floue identifiée :
```
### Zone N : [citation du passage vague]
**Catégorie :** décor vague / mécanisme non expliqué / personnage carton / raccourci émotionnel / fait technique vague
**Problème :** en quoi c'est trop flou
**Enrichissement :** le détail concret qui remplace le flou
**Source d'inspiration :** [si basé sur du réel] quelles affaires/faits mélangés, et comment
```

### Règles :
- Ne JAMAIS copier-coller une affaire réelle. Toujours mélanger au moins 2 sources.
- Privilégier les détails sensoriels et concrets plutôt que les descriptions abstraites.
- Chaque enrichissement doit passer le test : "est-ce que quelqu'un qui connaît le sujet trouverait ça crédible ?"
- Mettre à jour le synopsis (étape 3) avec les enrichissements validés avant de passer à l'écriture.

---

## Étape 5 : Écriture

Sortie : `stories/game_XX/5_story.md`

Objectif : écrire l'histoire complète.

### Principes :
- **Regrouper les coups** — un chapitre n'est pas un coup. Plusieurs coups forment une scène.
- **Le rythme suit la partie** — ouverture calme = exposition posée. Milieu tactique = tempo qui s'accélère. Finale = tension maximale ou intimité.
- **Les captures sont des scènes, pas des mentions** — chaque capture importante mérite sa scène.
- **Les coups anodins = ellipses narratives** — "les semaines passèrent" plutôt que de forcer un sens à chaque coup.
- **Montrer, ne pas dire** — le lecteur ne doit jamais sentir le mécanisme échiquéen derrière.

---

## Étape 6 : Relecture de cohérence

Checklist finale :
- [ ] Un lecteur non-joueur d'échecs comprendrait-il et apprécierait-il cette histoire ?
- [ ] Les retournements de l'histoire correspondent-ils aux retournements de la partie ?
- [ ] Aucun personnage n'agit de manière incohérente pour "coller" à la partie ?
- [ ] L'histoire a-t-elle sa propre identité, ou sent-on qu'elle est "générée" ?
- [ ] Relire la partie d'échecs en parallèle : les grands moments sont-ils tous là ?

Si tout est bon → publication dans `stories/game_XX/5_story.md` (version finale).
