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

### 2c. Fusils et résonances
Consulter `reference/techniques.md`. Pour chaque élément qui porte du poids narratif (une compétence, un objet, un savoir, un lieu) :
- Dans quel contexte est-il introduit ?
- Existe-t-il un **deuxième contexte** où il pourrait résonner de manière inattendue ?
- Si oui, noter le transfert prévu. L'introduction dans le contexte A doit être naturelle — le transfert vers B se planifie ici mais ne se signale jamais au lecteur.

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

## Étape 4 : Audit narratif — Chasse au banal

Sortie : `stories/game_XX/4_audit.md`

Objectif : relire le synopsis et identifier chaque élément **banal, passif, prévisible ou commode**, puis le justifier ou le corriger. Identifier aussi les éléments **intéressants/originaux** pour s'assurer qu'on les exploite à fond.

### Pourquoi cette étape AVANT la densification :
Il ne sert à rien de densifier (ajouter du détail) à une scène fondamentalement ennuyeuse. On corrige d'abord la structure narrative, PUIS on remplit les blancs.

---

### A. Éléments à traquer (le banal)

Pour chaque passage du synopsis, se demander : **"est-ce que ce choix est le PREMIER qui vient à l'esprit ?"** Si oui, c'est probablement banal.

**6 catégories de banal :**

#### 1. Personnage passif
Le personnage reçoit l'information au lieu de la produire. Il attend qu'on lui dise, qu'on lui montre, qu'on lui donne.
- **Test** : retirer le personnage de la scène. Si l'information arrive quand même (via un témoin, un document trouvé, un aveu spontané), le personnage est passif — il est un réceptacle, pas un moteur.
- **Exemples** : un enquêteur à qui les témoins racontent tout. Un scientifique qui trouve la preuve par hasard. Un héros qui assiste à la révélation au lieu de la provoquer.
- **Fix** : le personnage doit DÉDUIRE, PROVOQUER ou CONSTRUIRE l'information. Il agit sur le monde, pas l'inverse.
- **Exception justifiable** : la passivité est un choix narratif (un personnage volontairement paralysé, un blocage psychologique qui sera surmonté). Dans ce cas, la passivité doit être RESSENTIE comme un problème par le personnage et par le lecteur.

#### 2. Choix prévisible
Le premier choix, le plus évident, le plus attendu pour le genre.
- **Test** : si quelqu'un résume l'histoire en une phrase et que l'interlocuteur répond "ah oui, classique", c'est prévisible.
- **Exemples** : partie d'échecs → guerre médiévale. Meurtre → enquêteur alcoolique. Entreprise → PDG cupide. Trahison → la femme/le meilleur ami.
- **Fix** : garder le genre mais TORDRE l'angle. Pas une guerre → un procès. Pas un enquêteur alcoolique → une gendarme-oenologue. Le twist n'est pas dans l'intrigue mais dans le REGARD porté sur l'intrigue.

#### 3. Mécanisme commode
L'information arrive au bon moment, par le bon canal, sans effort.
- **Test** : le personnage avait-il une RAISON de chercher cette information à ce moment précis ? Si non, c'est commode.
- **Exemples** : "un voisin se souvient soudain d'un détail crucial." "Un document tombe du dossier." "Le suspect avoue sous la pression." Un témoin qui révèle l'info clé sans qu'on la lui demande.
- **Fix** : le personnage doit avoir une MÉTHODE. Il cherche au bon endroit parce qu'il a DÉDUIT que c'est le bon endroit. Le témoin parle parce que le personnage a posé la BONNE question. La preuve est trouvée parce que le personnage savait QUOI chercher.

#### 4. Résolution facile
Le problème est résolu sans coût réel, sans résistance, sans sacrifice.
- **Test** : le personnage est-il dans une situation PIRE après la résolution qu'avant ? Si non, c'est trop facile.
- **Exemples** : le héros dénonce le méchant et gagne. L'enquêteur trouve le coupable et reçoit une promotion. Le scientifique publie et est reconnu.
- **Fix** : le personnage PAYE quelque chose. Il résout le problème mais perd son poste, sa relation, son confort, sa réputation. La résolution crée un NOUVEAU problème.

#### 5. Cliché narratif
Un schéma si souvent utilisé qu'il ne surprend plus.
- **Test** : est-ce qu'on pourrait deviner la suite en connaissant le genre ?
- **Exemples** : le mentor qui meurt pour motiver le héros. Le twist final "c'était lui depuis le début." Le flashback explicatif au moment du dénouement. La confrontation finale avec discours du méchant.
- **Fix** : soit SUPPRIMER (le cliché n'est pas nécessaire), soit INVERSER (le mentor survit mais trahit ; le twist n'est pas QUI mais POURQUOI ; pas de confrontation finale, juste un silence).

#### 6. Scène sans enjeu
Une scène qui ne change rien. Si on la retire, l'histoire continue exactement pareil.
- **Test** : retirer la scène. Si rien ne change dans les scènes suivantes, elle est inutile.
- **Exemples** : une scène d'exposition qui répète ce qu'on sait déjà. Un interrogatoire qui ne produit rien. Une réunion qui confirme le plan sans le modifier.
- **Fix** : soit la SUPPRIMER, soit y injecter un élément qui CHANGE la direction (un détail inattendu, une information qui contredit ce qu'on pensait).

---

### B. Éléments à repérer (l'intéressant)

Ne pas seulement chasser le mauvais — identifier ce qui FONCTIONNE pour ne pas l'écraser et l'amplifier.

**6 catégories d'intéressant :**

1. **Compétence rare** — le personnage possède un savoir inhabituel qui crée des connexions que personne d'autre ne voit. (Ex : Noor + chimie oenologique. Marc + pharmacologie.) → Amplifier : faire travailler cette compétence PLUSIEURS FOIS, pas une seule.

2. **Déduction non-linéaire** — le personnage connecte des points que le lecteur n'aurait pas connectés. La logique est implacable mais surprenante. (Ex : maquillage en accident → art. 726 → héritier.) → Amplifier : montrer le RAISONNEMENT, pas juste la conclusion.

3. **Sacrifice coûteux** — le personnage paie un VRAI prix pour avancer. Pas un sacrifice symbolique — un sacrifice qui change sa vie. (Ex : Noor perd son mandat.) → Amplifier : montrer les conséquences APRÈS le sacrifice, pas juste le moment.

4. **Ironie dramatique** — le lecteur sait quelque chose que les personnages ne savent pas, ou un personnage se trahit sans le savoir. (Ex : Hélène qui ne montre aucune surprise → elle se trahit par l'ABSENCE de réaction.) → Amplifier : laisser le lecteur sentir l'ironie avant de l'expliquer.

5. **Détail technique surprenant** — un fait réel qui semble inventé. (Ex : la granulométrie fine du métabisulfite. L'article 726 du code civil.) → Amplifier : intégrer le détail dans le RAISONNEMENT du personnage, pas en note de bas de page.

6. **Inversion d'attente** — le choix narratif va CONTRE ce que le genre promet. (Ex : dans un polar, le moment clé n'est pas un interrogatoire mais un calcul sur un cahier. Le "gun" de l'histoire est un taux de SO2, pas une arme.) → Amplifier : assumer l'inversion, ne pas la compenser par un retour au cliché.

7. **Fusil transféré** — un élément posé dans un contexte A réapparaît dans un contexte B inattendu (voir `reference/techniques.md`). → Vérifier : des éléments déjà posés pourraient-ils résonner dans un deuxième contexte ? Si oui et que ce n'était pas planifié à l'étape 2, l'intégrer maintenant.

---

### Format du document :

```
### Élément N : [citation ou résumé du passage]
**Verdict :** 🔴 Banal / 🟢 Intéressant
**Catégorie :** [une des 12 catégories ci-dessus]
**Analyse :** pourquoi c'est banal/intéressant
**Action :** [si banal] comment corriger — [si intéressant] comment amplifier
```

### Règles :
- Être IMPITOYABLE. Si c'est le premier choix qui vient, c'est probablement le mauvais.
- Un élément peut être à la fois intéressant ET partiellement banal (ex : bonne idée, exécution paresseuse).
- L'audit doit être fait AVANT la densification : on corrige la structure avant de remplir les détails.
- Après l'audit, RÉÉCRIRE les passages du synopsis qui ont été identifiés comme banals avant de passer à l'étape 5.

---

## Étape 5 : Densification — Chasse au flou

Sortie : `stories/game_XX/5_densification.md`

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
- Mettre à jour le synopsis (étape 3) avec les enrichissements validés avant de passer à l'écriture (étape 6).

---

## Étape 6 : Écriture

Sortie : `stories/game_XX/6_story.md`

Objectif : écrire l'histoire complète.

### Principes :
- **Regrouper les coups** — un chapitre n'est pas un coup. Plusieurs coups forment une scène.
- **Le rythme suit la partie** — ouverture calme = exposition posée. Milieu tactique = tempo qui s'accélère. Finale = tension maximale ou intimité.
- **Les captures sont des scènes, pas des mentions** — chaque capture importante mérite sa scène.
- **Les coups anodins = ellipses narratives** — "les semaines passèrent" plutôt que de forcer un sens à chaque coup.
- **Montrer, ne pas dire** — le lecteur ne doit jamais sentir le mécanisme échiquéen derrière.

---

## Étape 7 : Relecture de cohérence

Checklist finale :
- [ ] Un lecteur non-joueur d'échecs comprendrait-il et apprécierait-il cette histoire ?
- [ ] Les retournements de l'histoire correspondent-ils aux retournements de la partie ?
- [ ] Aucun personnage n'agit de manière incohérente pour "coller" à la partie ?
- [ ] L'histoire a-t-elle sa propre identité, ou sent-on qu'elle est "générée" ?
- [ ] Relire la partie d'échecs en parallèle : les grands moments sont-ils tous là ?

Si tout est bon → publication dans `stories/game_XX/6_story.md` (version finale).
