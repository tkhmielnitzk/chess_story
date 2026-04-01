# Synopsis — Les Angles Morts

## Résumé en une phrase

Dans une mégapole sous surveillance totale, une analyste qui lit les absences dans les données traque un ingénieur-système qui a tué son directeur en exploitant les failles du réseau qu'il a lui-même construit — et sacrifie ses deux accès institutionnels pour le forcer à fuir dans la lumière.

---

## Acte I — Le système parfait (coups 1-18)

14 mars 2071, 6h12. Tour Helix, strate 7 d'Éos. L'assistant personnel d'Arno Schäfer, directeur de la division Données du Consortium, trouve son patron effondré dans son fauteuil ergonomique, face aux 6 écrans de son bureau. Pupilles fixes, mâchoire relâchée, main gauche encore sur le trackpad. IRIS — le réseau de surveillance intégrée d'Éos — enregistre la mort à 6h12m07s. Cause : arrêt cardiaque. Le système médical d'Éos génère automatiquement un certificat de décès numérique. Cortisol chronique élevé, antécédents de fibrillation auriculaire, 61 ans. Mort naturelle. Dossier clos en 47 minutes.

Syla Nkomo, 34 ans, analyste de schémas au Bureau de Sûreté Intérieure, n'est pas concernée. Elle travaille à la strate 4 — département d'analyse prédictive, bureau 1107, un open space de 40 analystes qui lisent les flux d'IRIS huit heures par jour. Son travail : repérer des anomalies statistiques dans les données de surveillance — un flux de personnes inhabituel dans un corridor de strate 3, une variation de consommation énergétique dans un entrepôt, un pic de transactions dans un quartier calme. Elle ne traite pas les décès. Elle ne traite pas les strates supérieures. (**Les Blancs se développent calmement — e4, d4, Nc3, Be3**)

Mais Syla a une habitude. Chaque matin, avant de commencer ses analyses assignées, elle lit le **digest IRIS** — le résumé automatique des événements nocturnes sur les 7 strates. C'est de la curiosité, pas du travail. La plupart des analystes ne le lisent plus depuis des années — c'est un flux de données brut, 200 pages par nuit, non filtré.

Ce matin-là, dans le digest, Syla voit la mort de Schäfer. Et elle voit autre chose. Pas dans les données. Dans les **métadonnées**.

**Première déduction.** Les logs IRIS du couloir de la Tour Helix entre 23h00 et 6h12 montrent 4 caméras actives, 2 capteurs biométriques d'ambiance, et 1 porte à empreinte palmaire. Tout est nominal. Aucune intrusion. Mais Syla remarque que la caméra C3 — celle qui couvre l'angle nord-est du couloir, à 12 mètres de la porte du bureau de Schäfer — a enregistré un **micro-décalage de luminosité** de 0,2% à 23h51. Un pic de 0,2%, pendant 1,4 seconde, puis retour à la normale.

0,2% de luminosité. 1,4 seconde. N'importe quel analyste classerait ça comme du bruit — une fluctuation de l'éclairage du couloir, un reflet, un passage nuageux sur les panneaux solaires extérieurs. Mais Syla connaît les caméras IRIS. Elle a passé 12 ans à lire leurs flux. Et elle sait que les caméras de strate 7 sont des modèles Helos-K9, à compensation automatique d'exposition. Un Helos-K9 compense une fluctuation de luminosité en 0,3 seconde. Si le pic dure 1,4 seconde, ce n'est pas une fluctuation DE la lumière — c'est une fluctuation de la CAMÉRA. Quelque chose a perturbé le capteur pendant 1,4 seconde. (**Bh6 — échange stratégique, Syla identifie l'anomalie dans le système**)

Syla ne signale rien. Pas encore. Elle télécharge les logs bruts de la caméra C3 sur son poste — elle a le droit, c'est dans son périmètre d'analyste. Elle analyse le signal.

**Deuxième déduction.** Le pic de 0,2% n'est pas une perturbation optique. C'est une perturbation ÉLECTROMAGNÉTIQUE. La signature correspond à un pulse EM de courte portée — le type de signal émis par un brouilleur directionnel. Quelqu'un a utilisé un brouilleur EM pendant 1,4 seconde à proximité de la caméra C3 à 23h51. Pas pour éteindre la caméra — ça déclencherait une alerte. Pour la DÉSYNCHRONISER pendant 1,4 seconde. Pendant ce laps de temps, la caméra continue d'enregistrer — mais le flux est en décalage de 1,4 seconde avec le temps réel. Assez pour qu'une personne traverse les 12 mètres du couloir sans apparaître sur l'image synchrone.

Quelqu'un est entré dans le bureau de Schäfer. IRIS ne l'a pas vu — mais le fantôme de son passage est là, dans un pic de 0,2%. (**Na5 — le cavalier s'infiltre**)

**Troisième déduction.** Si le brouilleur a désynchronisé la caméra C3 pendant 1,4 seconde, les 3 autres caméras du couloir auraient dû capter le passage. Syla vérifie. Les 3 autres caméras ne montrent RIEN à 23h51. Conclusion : soit les 4 caméras ont été brouillées simultanément (improbable — 4 brouilleurs directionnels synchronisés, c'est un équipement militaire), soit quelqu'un a modifié les LOGS des 3 autres caméras APRÈS coup. Effacé 1,4 seconde sur chaque flux. Mais il a oublié — ou n'a pas pu — modifier les logs de C3. Pourquoi ? Parce que C3 est le seul Helos-K9 du couloir. Les 3 autres sont des modèles Pallas-M2, une génération plus récente, dont les logs sont stockés en cloud IRIS central. C3, plus ancien, a un buffer local de 72 heures avant upload. Celui qui a effacé les logs a modifié le cloud central — mais pas le buffer local de C3. Il ne savait pas que C3 avait un buffer local. Ou il le savait mais n'y avait pas accès.

**Le tueur a accès aux logs centraux d'IRIS.** Pas un accès de consultation — un accès d'ÉCRITURE. Il peut modifier les données de surveillance. C'est quelqu'un d'IRIS. (**Nd5 — le cavalier contrôle le centre, Syla comprend que le tueur est DANS le système**)

---

## Acte II — Les sacrifices (coups 19-27)

Syla a maintenant une hypothèse : Schäfer a été tué par quelqu'un qui a accès en écriture aux logs centraux d'IRIS. Elle doit vérifier. Pour vérifier, elle a besoin d'accéder au **journal d'audit d'IRIS** — le log qui enregistre QUI a modifié QUOI dans les données de surveillance. C'est un niveau d'accès qu'elle n'a pas. Les analystes du BSI ont un accès en lecture seule aux flux. Le journal d'audit est réservé aux ingénieurs-système d'IRIS et aux directeurs de division.

**Premier sacrifice (Rxd4!! — coup 24).** Syla utilise son accès standard pour lancer une requête transversale : elle demande à IRIS la liste des comptes ayant effectué des modifications sur les flux de la Tour Helix entre le 13 mars 22h00 et le 14 mars 6h00. C'est une requête légitime en apparence — elle pourrait faire partie d'un audit de routine. Mais le système de sécurité interne d'IRIS détecte que la requête cible les logs d'une strate 7 depuis un poste de strate 4. Alerte de niveau 2. Le superviseur de Syla, Commandant Ehrlich, reçoit la notification en 11 minutes.

Mais Syla a eu le temps de voir la réponse. Un seul compte a modifié les logs de la Tour Helix cette nuit-là : **V.LENZ — Ingénieur-système senior, Division Infrastructure IRIS.**

Viktor Lenz. 44 ans. L'homme qui maintient IRIS. Celui qui connaît chaque capteur, chaque algorithme, chaque buffer local de chaque modèle de caméra. Sauf, apparemment, le buffer local du Helos-K9 de la caméra C3.

L'accès de Syla est suspendu dans l'heure. Ehrlich la convoque : "Nkomo, pourquoi est-ce que tu fais une requête sur les logs de la strate 7 ? Tu travailles sur la strate 3, secteur logistique." Syla : "Il y a une anomalie sur un Helos-K9 dans le couloir de Schäfer." Ehrlich : "Schäfer est mort d'un arrêt cardiaque. C'est clos. Et tu n'as pas l'habilitation pour les logs de strate 7. Ton accès est suspendu en attendant un examen disciplinaire." (**La première tour est sacrifiée — Syla a perdu son accès IRIS**)

Syla sait maintenant QUI. Mais elle n'a aucune preuve recevable — son accès a été révoqué, sa requête sera classée comme non autorisée, et Viktor Lenz est toujours en poste, avec un accès complet au système.

**Syla déduit ce qu'elle ne peut plus lire dans les données.**

**Déduction 4 — le comment.** Si Lenz a traversé le couloir en 1,4 seconde de désynchronisation, il a eu accès au bureau de Schäfer. Mais Schäfer est mort d'un "arrêt cardiaque." Comment tue-t-on quelqu'un en mimant un arrêt cardiaque sans que le système médical ne détecte rien ?

Syla appelle sa mère. Marta Nkomo, 63 ans, infirmière en résidence surveillée de strate 3 pour dette médicale (120 000 crédits de soins après l'accident de son mari en 2051). Syla ne lui parle pas de l'enquête. Elle lui demande : "Maman, quand tu étais en soins intensifs, est-ce qu'il y avait un produit qu'on vous interdisait d'administrer par erreur ? Un truc qui pouvait tuer si mal dosé ?" Marta : "Le potassium. Le KCl. En perfusion, c'est courant — on corrige les hypokaliémies. Mais en bolus intraveineux, 40 milliéquivalents, c'est un arrêt cardiaque en 2 minutes. C'est la molécule des exécutions aux États-Unis, tu le savais ? Et le pire : le potassium est naturellement dans le sang. Après la mort, les cellules libèrent leur potassium intracellulaire. L'autopsie standard ne distingue pas le KCl injecté du potassium post-mortem." (**Le KCl est posé — contexte A : mémoire familiale**)

Syla : "Et il n'y a aucun moyen de le détecter ?"

Marta : "Si. Le potassium met plus de temps à migrer dans l'humeur vitrée — le liquide de l'oeil. Si tu compares le taux de K+ dans le sang et dans l'humeur vitrée dans les 12 heures, un écart anormal indique une injection. Mais il faut le chercher. Et il faut le chercher vite."

Syla regarde l'heure. Il est 19h40 le 14 mars. Schäfer est mort depuis 13 heures et 28 minutes. La fenêtre de 12 heures est dépassée. Trop tard pour l'humeur vitrée ? Peut-être pas — le corps est en chambre froide à la morgue automatisée de la strate 5. Le froid ralentit la migration du potassium. Il y a peut-être encore une chance.

**Deuxième sacrifice (Re7+ — coup 25).** Syla n'a plus accès à IRIS. Elle ne peut pas demander une autopsie — elle n'a pas l'autorité. Elle contacte la seule personne qui peut : **Dr. Youna Breit**, médecin légiste à la morgue automatisée, strate 5. Breit est une vieille connaissance — elles étaient au même concours de cybersécurité à 19 ans, avant que Breit bifurque vers la médecine. Syla lui demande de pratiquer un prélèvement d'humeur vitrée sur le corps de Schäfer et de faire un dosage K+/Na+. Sans ordre de réquisition. Sans autorisation du BSI.

Breit hésite. Puis accepte. Elle fait le prélèvement à 22h17 le 14 mars — 16 heures post-mortem. Le froid a ralenti la migration. Le rapport K+ vitreux / K+ sanguin est de 0,6. Normal post-mortem : 0,8-1,2. Un ratio de 0,6 signifie qu'il y avait BEAUCOUP plus de potassium dans le sang que dans l'oeil au moment de la mort. Injection exogène de KCl. Schäfer a été assassiné. (**La deuxième tour entre en jeu — Re7+. Syla a activé une ressource hors système**)

---

## Acte III — La chasse (coups 26-35)

Syla a maintenant : le QUI (Lenz), le COMMENT (KCl), la preuve de l'intrusion (C3, 0,2%, 1,4s), et la preuve du meurtre (ratio K+ vitreux). Mais elle n'a plus d'accès institutionnel. Elle est suspendue. Et Lenz est toujours en poste.

**Lenz sait qu'on le cherche.** L'alerte déclenchée par la requête de Syla a été logguée — et Lenz, en tant qu'ingénieur-système, a accès aux alertes de sécurité. Il a vu la requête. Il a vu que quelqu'un a cherché les modifications de logs de la Tour Helix. Il ne sait pas encore qui — la requête est anonymisée au niveau de l'analyste. Mais il sait que quelqu'un a tiré le fil.

Lenz prend une décision : fuir. Pas Éos — on ne quitte pas Éos. Mais descendre dans les strates. Passer de la strate 7 (où il est visible, connu, logué) vers les strates basses (où IRIS a des trous). Il connaît les zones grises — c'est lui qui les a cartographiées lors des audits techniques. (**Le roi noir commence sa traversée — Kb6, Kxa5, Ka4**)

**Syla anticipe.** Elle ne peut plus lire IRIS, mais elle peut PENSER comme IRIS. Elle connaît l'architecture du réseau — pas au niveau ingénieur, mais au niveau analyste. Elle sait où sont les zones grises. Et elle sait quelque chose que Lenz ne sait pas : elle a grandi dans les zones grises. Son père travaillait en strate 2, dans les infrastructures de maintenance — les couloirs techniques, les conduits de ventilation, les noeuds de données physiques. Syla y allait enfant, après l'école, en attendant que son père finisse son service. Elle connaît la strate 2 par le CORPS, pas par les données.

**Déduction 5 — la fuite de Lenz.** Si Lenz descend dans les strates, il va utiliser les zones grises qu'il connaît — celles des audits techniques. Mais les audits techniques d'IRIS sont faits depuis les logs, pas depuis le terrain. Lenz connaît les zones grises THÉORIQUES — celles qui apparaissent comme des trous dans les données. Syla connaît les zones grises RÉELLES — celles qu'on ne peut connaître qu'en y ayant marché. Et les deux ne coïncident pas toujours. Certaines zones grises théoriques ont été comblées par des capteurs non documentés (installés par la maintenance, hors procédure). Et certaines zones réellement aveugles n'apparaissent pas dans les audits.

Lenz croit être invisible. Syla sait où il sera visible. (**Qxd4+ — la dame entre avec échec. Syla anticipe les mouvements de Lenz**)

**La traque.**

Syla n'agit pas seule. Elle transmet ses conclusions au Commandant Ehrlich — non pas comme une requête officielle, mais comme une note manuscrite. Papier, pas numérique. Parce que tout ce qui est numérique passe par IRIS, et Lenz a accès à IRIS. Ehrlich lit la note. Il regarde Syla. Il dit : "Si tu te trompes, on coule tous les deux." Puis il déverrouille le protocole d'intervention.

**Lenz descend.** Strate 7 → strate 5 (transports publics, caméras standard — il porte un brouilleur personnel, un modèle civil légal qu'il a modifié pour émettre un pulse directionnel). Strate 5 → strate 3 (corridor de fret, zone grise théorique — mais Syla sait qu'un capteur de maintenance y a été installé en 2069). Strate 3 → strate 2 (conduits techniques, l'ancien territoire du père de Syla).

**b4+ — le pion donne échec.** Un détail matériel coince Lenz. Les conduits de strate 2 exigent un badge de maintenance pour passer les sas de ventilation. Lenz a un badge cloné — mais le badge est un modèle 2068. Les sas ont été mis à jour en 2070. Le badge ouvre le sas... mais génère une alerte de compatibilité dans le système de maintenance (pas IRIS — un système séparé, local, que Lenz n'a pas pensé à vérifier). Syla avait prévenu Ehrlich : "Surveillez les alertes de maintenance de strate 2, pas IRIS."

**Qc3 — la dame repositionne.** Syla déduit la destination de Lenz. S'il descend en strate 2, il cherche un noeud de données physique — un point d'accès matériel au réseau IRIS. S'il atteint un noeud, il peut effacer les preuves à la source : le buffer local de C3, les logs d'audit, tout. Lenz ne fuit pas — il va détruire les preuves. Syla identifie les 3 noeuds physiques de strate 2 accessibles depuis les conduits techniques. Elle envoie des équipes sur deux. Elle va sur le troisième elle-même — le noeud 7-B, dans le couloir de ventilation du secteur Minerva. Le secteur où son père travaillait.

---

## Acte IV — Le couloir (coups 36-44)

Noeud 7-B. Strate 2, secteur Minerva. Un couloir de 3 mètres de large, 2,10 de haut, éclairé par des néons industriels dont un sur trois fonctionne. Au fond, une porte métallique grise avec un panneau : "IRIS — Noeud physique 7-B — Accès restreint." L'air sent le métal chaud et le lubrifiant de ventilation.

Lenz est déjà là. Syla le voit de dos — il est devant le terminal du noeud, un câble branché dans le port physique. Il est en train d'effacer.

Syla n'a pas d'arme. Elle n'est pas formée à l'intervention. Elle est analyste. Mais elle n'a pas besoin d'intervenir physiquement.

**Bf1 — le fou verrouille.** Syla active son terminal personnel. Elle se connecte au noeud 7-B par le réseau local — pas IRIS, le réseau de maintenance de strate 2. Le même réseau que son père utilisait pour diagnostiquer les pannes de ventilation. Un réseau que Lenz ne surveille pas parce qu'il n'est pas dans le périmètre d'IRIS. Syla envoie une commande de verrouillage du terminal. Le terminal de Lenz se fige.

Lenz se retourne. Il voit Syla. (**Le fusil transféré tire — contexte B.** La connaissance des réseaux de strate 2, posée comme un élément biographique au début, devient l'outil qui neutralise Lenz. Ce n'est pas IRIS qui l'arrête. C'est le réseau de maintenance du père de Syla.)

Lenz : "Vous êtes l'analyste. La requête sur les logs de Helix."
Syla : "Vous avez oublié le buffer local du Helos-K9."
Lenz : "Je n'ai pas oublié. Je n'avais pas l'accès. Le buffer local de C3 est sur le réseau de maintenance, pas sur IRIS. Je n'ai jamais eu accès au réseau de maintenance."
Syla : "Moi si."

Ehrlich et l'équipe d'intervention arrivent 4 minutes plus tard. Lenz ne résiste pas. Le terminal est saisi. L'effacement est incomplet — Lenz a supprimé 60% des logs d'audit, mais le buffer de C3 est intact, et le prélèvement d'humeur vitrée est déjà entre les mains du Dr. Breit.

**Qa7 — abandon.** Lenz est placé en détention. Il ne parle pas pendant 3 jours. Puis il demande à voir Syla. Pas un avocat. Syla.

---

## Le mobile (le fou libéré)

Lenz parle. Pas pour se défendre — pour expliquer.

Schäfer n'était pas seulement le directeur de la division Données. Schäfer avait lancé, en secret, le **Projet Parallaxe** : une extension d'IRIS qui ne se contente plus de SURVEILLER les comportements mais de les PRÉDIRE et de les MODIFIER. Parallaxe utilise les données d'IRIS pour identifier les individus susceptibles de commettre des crimes, des fraudes, ou des "déstabilisations sociales" — et les NEUTRALISER préventivement. Pas par arrestation. Par modification de leur environnement : un emploi supprimé, un crédit refusé, un trajet dévié, une alerte médicale fabriquée. Schäfer avait commencé les tests en strate 1 et 2 — les populations non-enregistrées, celles que personne ne surveille parce que personne ne s'en soucie.

Lenz avait découvert Parallaxe en auditant les flux de données internes. Il avait vu les logs : 3 400 interventions préventives en 8 mois. 3 400 vies modifiées sans procès, sans alerte, sans recours. Il avait demandé à Schäfer d'arrêter. Schäfer avait refusé. Lenz avait menacé de rendre public. Schäfer avait répondu : "Viktor, tu es SUR le système. Si Parallaxe tombe, tu tombes avec."

Lenz avait tué Schäfer pour arrêter Parallaxe. Pas par vengeance. Par calcul : Schäfer était le seul à avoir les codes d'activation de Parallaxe. Sans Schäfer, Parallaxe s'arrête. Et en maquillant le meurtre en mort naturelle, Lenz s'assurait que personne ne chercherait les codes.

Syla écoute. Elle ne dit rien. (**Silence éloquent.**)

Puis elle pose une seule question : "Parallaxe s'est arrêté ?"

Lenz : "Oui. Depuis le 14 mars."

Syla : "Combien de personnes en strate 1 et 2 ont été affectées ?"

Lenz : "3 412."

Syla : "Ma mère est en résidence surveillée pour dette médicale. 120 000 crédits. La dette a été recalculée en janvier par le système."

Silence.

Lenz : "Je ne sais pas."

---

## Épilogue

Viktor Lenz est jugé pour meurtre. Le Projet Parallaxe est révélé au procès — mais le Consortium fait pression pour que les détails soient classifiés. Le mot "Parallaxe" n'apparaît pas dans le jugement public. Lenz est condamné à 30 ans de détention en strate 1.

Syla Nkomo est réintégrée au BSI. Pas promue — réintégrée. Ehrlich a couvert sa requête non autorisée en la requalifiant comme "test de pénétration interne initié dans le cadre d'un audit de fiabilité." C'est faux. Tout le monde le sait. Personne ne dit rien.

Le Dr. Breit reçoit un avertissement administratif pour avoir pratiqué un prélèvement sans réquisition. L'avertissement est inscrit dans son dossier pendant 2 ans.

Le buffer local du Helos-K9 — la caméra C3 — est mis à jour. Tous les Helos-K9 restants dans Éos sont remplacés par des Pallas-M2 en cloud pur. Plus de buffer local. Plus de faille. Plus de 0,2%.

Syla rentre chez elle, strate 3. Elle appelle sa mère. Elle ne parle pas de l'affaire. Elle lui demande comment elle va. Marta dit : "Ils ont annulé une partie de ma dette médicale la semaine dernière. Je ne sais pas pourquoi. Un recalcul automatique, apparemment." Syla ne dit rien. (**Contrepoint émotionnel + question ouverte.** Parallaxe a-t-il fabriqué la dette de Marta ? Lenz a-t-il arrêté Parallaxe à temps ? On ne saura pas. Syla non plus.)

Elle raccroche. Elle ouvre le digest IRIS du soir. 200 pages de données brutes. Elle commence à lire.

---

## Thèmes

- **L'absence comme preuve** — Syla résout l'affaire en lisant ce qui MANQUE, pas ce qui est là. 0,2% de luminosité. 1,4 seconde. Un buffer oublié. Le système parfait a des trous — et les trous parlent.
- **Le système ne protège pas — il aveugle** — IRIS couvre 99,7% de l'espace. Les 0,3% restants sont les seuls endroits où la vérité existe. La surveillance totale ne rend pas les gens plus sûrs — elle rend les crimes plus sophistiqués et les enquêteurs plus dépendants.
- **Le sacrifice institutionnel** — Syla sacrifie ses deux accès (IRIS + son poste) pour forcer la vérité. Comme Kasparov sacrifie ses deux tours : chaque sacrifice ouvre une ligne d'attaque.
- **Le tueur moral** — Lenz a tué pour arrêter Parallaxe. L'histoire ne juge pas. Syla non plus. Le lecteur doit décider seul.
- **Les strates** — la justice ne descend pas en dessous de la strate 4. 3 412 vies modifiées en strate 1 et 2, et personne ne le saura jamais.

---

## Test de cohérence

- [x] L'histoire tient sans connaître les échecs ? → C'est un polar futuriste sur la surveillance de masse. Aucune référence aux échecs.
- [x] Techniquement crédible ? → Le KCl et l'humeur vitrée sont réels. Le brouilleur EM est plausible. L'architecture réseau à strates est cohérente.
- [x] Motivations crédibles ? → Lenz : arrêter un programme de contrôle social. Syla : voir ce que les autres ne voient pas. Ehrlich : survivre dans le système. Schäfer : le pouvoir par les données.
- [x] Retournements earned ? → Le 0,2% est posé dès l'Acte I. Le KCl est introduit via la mère (pas un deus ex machina). Le réseau de maintenance est posé biographiquement. Chaque élément paie plus tard dans un contexte différent.
- [x] Enquêtrice atypique ? → Syla lit les absences, pas les présences. Elle pense à l'envers d'IRIS.
- [x] Fusils transférés ? → (1) Compétence de lecture d'absence : enquête → survie/traque. (2) Réseau de strate 2 : biographie paternelle → outil de neutralisation. (3) KCl : mémoire familiale → preuve chimique.
- [x] Question ouverte ? → La dette de Marta. Parallaxe. Les 3 412.
