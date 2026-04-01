# Pipeline — De la partie à l'histoire

## Boucles et versioning

La pipeline n'est PAS linéaire. Les étapes se nourrissent mutuellement.

### Boucles autorisées :
- **Étape 4 (audit) → peut RÉÉCRIRE l'étape 3 (synopsis) et MODIFIER l'étape 2 (framework)** si un élément est structurellement banal.
- **Étape 5 (densification) → peut RÉÉCRIRE l'étape 3 (synopsis)** si un enrichissement change la logique de l'histoire.
- **Étape 7 (relecture) → peut renvoyer à N'IMPORTE quelle étape.**

### Versioning :
Quand un fichier est réécrit suite à une boucle, noter la version dans le fichier :
```
<!-- v2 — post-audit : réécriture de Noor en déductrice -->
```
Ne pas supprimer les versions précédentes du git history — elles documentent l'évolution des choix narratifs.

---

## Étape 0 : Sélection de la partie

Entrée : un genre/ton voulu (optionnel) OU une partie déjà choisie
Sortie : fichier PGN dans `games/`

### Deux modes :

**Mode A — Partie d'abord.** On a une partie en tête (célèbre, intéressante, coup de coeur). On la prend et on voit quel genre elle supporte. C'est le mode exploratoire.

**Mode B — Genre d'abord.** On sait quel type d'histoire on veut. On identifie d'abord les **propriétés échiquéennes** qui servent ce genre, puis on cherche une partie qui les contient.

| Genre voulu | Propriétés échiquéennes à chercher |
|-------------|-----------------------------------|
| Enquête / polar | Accumulation de pièces mineures, manoeuvres longues, combinaison finale = construction d'un dossier |
| Traque / chasse | Chasse au roi, échecs successifs, roi qui traverse l'échiquier |
| Thriller psychologique | Partie positionnelle, zugzwang, étranglement lent |
| Drame / tragédie | Sacrifice majeur (dame, tour), perte irréversible pour un gain moral |
| Comeback / rédemption | Position perdue retournée, défense héroïque, contreattaque |
| Drame existentiel | Nulle, pat, forteresse imprenable |
| Corruption / infiltration | Cavalier en avant-poste, pièce infiltrée en territoire ennemi |
| Surveillance / contrôle | Tours connectées sur colonnes ouvertes, domination d'espace |
| Révolution / rébellion | Promotion de pion, pièce mineure qui bat une pièce majeure |

Ce tableau n'est pas exhaustif — il s'enrichit à chaque histoire (voir étape 8).

### Règle : la partie doit être INTÉRESSANTE en tant que partie. Si les coups ne sont pas beaux, l'histoire ne le sera pas non plus.

---

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
- **Rythme** : où sont les accélérations et les pauses ? Y a-t-il une rupture de tempo ? La partie a-t-elle deux phases distinctes ?

### Règle : pas de métaphore ici. Juste de l'analyse échiquéenne.

---

## Étape 2 : Cadre narratif

Sortie : `stories/game_XX/2_framework.md`

Objectif : choisir le genre, assigner les rôles, et poser les fondations narratives.

### 2a. Genre / ton
Le style de la partie (étape 1) suggère un genre :
- Partie tactique agressive → action, fantasy épique, thriller
- Partie positionnelle lente → drame psychologique, thriller cérébral
- Partie avec sacrifice majeur → tragédie, récit héroïque
- Partie avec comeback → récit de rédemption, underdog story
- Partie nulle → drame existentiel, compromis amer

Ce n'est pas rigide. Le genre peut aussi venir d'une envie créative. Mais la partie doit le supporter.

### 2b. Micro-audit du genre

**AVANT d'aller plus loin**, se poser la question : "est-ce que ce genre/angle est le PREMIER qui vient à l'esprit pour cette partie ?"

Si oui → **le tordre**. Garder le genre mais changer l'ANGLE.

| Premier réflexe | Torsion possible |
|-----------------|-----------------|
| Partie agressive → guerre | → procès, compétition sportive, campagne politique |
| Sacrifice → héros tragique | → lanceur d'alerte, parent qui protège, artiste qui se consume |
| Mat étouffé → assassinat | → faillite, rupture amoureuse, perte de mémoire |
| Chasse au roi → poursuite policière | → fuite d'un système (surveillance, dette, maladie) |
| Partie positionnelle → espionnage | → relation toxique, harcèlement institutionnel, procédure kafkaïenne |

Le but n'est pas d'éviter les genres classiques — c'est d'éviter le PREMIER choix paresseux. Le deuxième ou troisième choix est presque toujours meilleur.

### 2c. La question du lecteur

Écrire en UNE phrase interrogative la question qui tient le lecteur du début à la fin :

- **Faible** : "Qui est le coupable ?" (réponse binaire, le lecteur attend juste un nom)
- **Moyenne** : "L'enquêtrice réussira-t-elle à prouver le meurtre ?" (tension, mais une seule issue intéressante)
- **Forte** : "Le tueur avait-il raison de tuer ?" (deux réponses légitimes, le lecteur est DIVISÉ)

**Test** : si la question a une réponse évidente ("oui le héros va gagner"), ce n'est pas une bonne question. La vraie question est ailleurs — la trouver.

La question du lecteur doit être inscrite en tête du `2_framework.md`. Elle guide TOUT ce qui suit.

### 2d. Assignation des rôles
Pour chaque pièce **qui compte** dans cette partie :
1. Consulter `reference/pieces.md` pour ses propriétés intrinsèques
2. Choisir une transposition qui sert le genre ET le rôle de cette pièce dans CETTE partie spécifique
3. **Justifier** : pourquoi cette association ? (propriétés intrinsèques + comportement dans la partie)

### 2e. Fusils et résonances
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

Objectif : écrire le **squelette sec** de l'histoire. Actions, décisions, retournements. PAS de détails sensoriels, PAS d'ancrage (ça vient à l'étape 5).

### Contrainte de format :
- **1 à 1,5 page maximum.** Si le synopsis dépasse 1,5 page, c'est qu'il contient des détails qui appartiennent à la densification.
- Chaque phrase doit être une ACTION ou une DÉCISION. Pas de description, pas d'ambiance, pas de chiffres précis.
- Le synopsis doit tenir debout comme un PITCH — quelqu'un qui le lit en 3 minutes doit comprendre toute l'histoire.

### À faire :
1. Lister les moments clés de la partie (étape 1)
2. Transposer chaque moment en scène narrative grâce aux rôles (étape 2) et aux événements (`reference/events.md`)
3. Rédiger le synopsis : début → développement → climax → dénouement

### Tracé de suspicion :

À la fin du synopsis, ajouter un tableau qui trace ce que le LECTEUR sait vs ce que le PERSONNAGE sait à chaque acte :

```
| Acte | Le personnage sait... | Le lecteur sait... | Effet |
|------|----------------------|-------------------|-------|
| I    | Rien (mort naturelle) | Rien              | Exposition |
| II   | C'est un meurtre     | C'est un meurtre  | Alignement |
| III  | Qui (Hélène)          | Qui + le mobile   | Ironie dramatique |
| IV   | Tout                  | Tout sauf une question | Question ouverte |
```

**Types d'effets :**
- **Alignement** : lecteur et personnage savent la même chose. Tension par identification.
- **Ironie dramatique** : le lecteur sait plus que le personnage. Tension par impuissance.
- **Surprise** : le personnage sait plus que le lecteur. Tension par révélation.
- **Question ouverte** : ni le lecteur ni le personnage ne savent. Tension par mystère persistant.

Le tracé de suspicion permet de vérifier que le lecteur n'est JAMAIS dans la même position pendant tout le récit — il doit osciller entre ces 4 états.

### Test de cohérence (CRITIQUE) :
Relire le synopsis en se posant ces questions :
- [ ] Est-ce que l'histoire tient debout **sans savoir qu'elle vient d'une partie d'échecs** ?
- [ ] Les motivations des personnages sont-elles crédibles ?
- [ ] Les retournements sont-ils "earned" (préparés narrativement) ou sortent-ils de nulle part ?
- [ ] Le ton est-il cohérent du début à la fin ?
- [ ] Y a-t-il des personnages/éléments qui apparaissent et disparaissent sans raison ?
- [ ] La question du lecteur (étape 2c) est-elle maintenue sous tension jusqu'au dénouement ?

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

**7 catégories d'intéressant :**

1. **Compétence rare** — le personnage possède un savoir inhabituel qui crée des connexions que personne d'autre ne voit. (Ex : Noor + chimie oenologique. Syla + lecture des absences dans IRIS.) → Amplifier : faire travailler cette compétence PLUSIEURS FOIS, pas une seule.

2. **Déduction non-linéaire** — le personnage connecte des points que le lecteur n'aurait pas connectés. La logique est implacable mais surprenante. (Ex : maquillage en accident → art. 726 → héritier. Pic de 0,2% → brouilleur EM → accès en écriture IRIS.) → Amplifier : montrer le RAISONNEMENT, pas juste la conclusion.

3. **Sacrifice coûteux** — le personnage paie un VRAI prix pour avancer. Pas un sacrifice symbolique — un sacrifice qui change sa vie. (Ex : Noor perd son mandat. Syla perd son accès IRIS.) → Amplifier : montrer les conséquences APRÈS le sacrifice, pas juste le moment.

4. **Ironie dramatique** — le lecteur sait quelque chose que les personnages ne savent pas, ou un personnage se trahit sans le savoir. (Ex : Hélène qui ne montre aucune surprise → elle se trahit par l'ABSENCE de réaction.) → Amplifier : laisser le lecteur sentir l'ironie avant de l'expliquer.

5. **Détail technique surprenant** — un fait réel qui semble inventé. (Ex : la granulométrie fine du métabisulfite. Le ratio K+/Na+ dans l'humeur vitrée. L'article 726 du code civil.) → Amplifier : intégrer le détail dans le RAISONNEMENT du personnage, pas en note de bas de page.

6. **Inversion d'attente** — le choix narratif va CONTRE ce que le genre promet. (Ex : dans un polar, le moment clé n'est pas un interrogatoire mais un calcul sur un cahier. Le "gun" de l'histoire est un taux de SO2, pas une arme.) → Amplifier : assumer l'inversion, ne pas la compenser par un retour au cliché.

7. **Fusil transféré** — un élément posé dans un contexte A réapparaît dans un contexte B inattendu (voir `reference/techniques.md`). → Vérifier : des éléments déjà posés pourraient-ils résonner dans un deuxième contexte ? Si oui et que ce n'était pas planifié à l'étape 2, l'intégrer maintenant.

---

### Format du document :

```
### Élément N : [citation ou résumé du passage]
**Verdict :** 🔴 Banal / 🟢 Intéressant
**Catégorie :** [une des 13 catégories ci-dessus]
**Analyse :** pourquoi c'est banal/intéressant
**Action :** [si banal] comment corriger — [si intéressant] comment amplifier
```

### Règles :
- Être IMPITOYABLE. Si c'est le premier choix qui vient, c'est probablement le mauvais.
- Un élément peut être à la fois intéressant ET partiellement banal (ex : bonne idée, exécution paresseuse).
- L'audit doit être fait AVANT la densification : on corrige la structure avant de remplir les détails.
- **Après l'audit, RÉÉCRIRE le synopsis (étape 3) et si nécessaire MODIFIER le framework (étape 2)** avec les corrections identifiées, avant de passer à l'étape 5. Marquer la version.

---

## Étape 5 : Densification — Chasse au flou

Sortie : `stories/game_XX/5_densification.md`

Objectif : relire le synopsis (version post-audit) et identifier chaque zone **vague, générique ou trop facile**, puis la rendre concrète et crédible.

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
- **Si un enrichissement change la logique de l'histoire** → RÉÉCRIRE le synopsis (étape 3). Marquer la version.

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
- [ ] La question du lecteur (étape 2c) est-elle résolue de manière satisfaisante — ou délibérément laissée ouverte ?
- [ ] Le tracé de suspicion (étape 3) est-il respecté ? Le lecteur oscille-t-il entre les 4 états ?

Si tout est bon → publication dans `stories/game_XX/6_story.md` (version finale).

Si non → renvoyer à l'étape concernée. Marquer la version.

---

## Étape 8 : Rétro-injection

Sortie : modifications dans `reference/*.md` et dans le tableau de l'étape 0

Objectif : **nourrir le système avec ce que l'histoire a appris.**

### Méthode :

Relire l'histoire terminée et identifier :

1. **Nouvelles transpositions** découvertes en cours de route → les ajouter dans `reference/pieces.md`
   > *Ex : game_02 — la tour comme "preuve matérielle qui arrive tard mais verrouille tout." Game_03 — la tour comme "accès institutionnel qu'on peut sacrifier."*

2. **Nouveaux événements narratifs** → les ajouter dans `reference/events.md`
   > *Ex : game_02 — "camouflage de crime en accident = signature d'héritier (art. 726)." Game_03 — "modification de logs = le tueur est DANS le système."*

3. **Nouvelles dynamiques** → les ajouter dans `reference/dynamics.md`
   > *Ex : game_02 — "enquêteur dessaisi qui continue d'agir par canal officieux." Game_03 — "réseau parallèle (maintenance) vs réseau principal (IRIS)."*

4. **Nouvelles techniques** → les ajouter dans `reference/techniques.md`
   > *Ex : game_03 — "le silence de réaction comme preuve comportementale" a enrichi le silence éloquent.*

5. **Nouvelles associations genre ↔ propriétés échiquéennes** → les ajouter dans le tableau de l'étape 0
   > *Ex : après game_03 — "surveillance totale + faille = double sacrifice de tour + buffer local oublié."*

### Règle : chaque histoire doit laisser au moins 2-3 ajouts dans les docs de référence. Si une histoire n'a rien appris au système, c'est qu'on n'a pas assez cherché.

### Fréquence : à faire IMMÉDIATEMENT après la relecture (étape 7), tant que les découvertes sont fraîches.
