# Densification — Chasse au flou

Relecture du synopsis v3. Identification des zones vagues, enrichissement par imagination ou faits réels mélangés.

---

### Zone 1 : Comment Marc a obtenu l'email

**Citation :** "Sur le siège passager, une clé USB. Dessus, un email."
**Catégorie :** Mécanisme non expliqué
**Problème :** C'est le pivot de toute l'histoire et on ne sait pas comment il l'a trouvé. Ça ressemble à un deus ex machina.

**Enrichissement :**
Marc prépare le PSUR n°6. Pour ça, il a besoin des tableaux de pharmacovigilance de RENEW-3, stockés sur le serveur interne SharePoint d'Helix (\\helix-lyon\clinical\RENEW\PV). Son accès normal couvre RENEW-1 et 2. Mais l'extension RENEW-3 est dans un sous-dossier verrouillé. Il demande l'accès à l'IT via un ticket ServiceNow — procédure standard pour un responsable PV qui compile un PSUR. L'IT lui ouvre l'accès au dossier RENEW-3, sans réaliser que ça inclut aussi le répertoire \\correspondence\internal\ où sont archivés les échanges email entre le management scientifique. C'est une erreur de permission, pas un hack. Marc tombe sur l'email en cherchant le rapport statistique de l'extension. Il ne le cherchait pas. Il est dans un dossier nommé "VD_AW_mars2019_reanalysis". Il le lit. Il le relit. Il le copie sur une clé USB Kingston de 16 Go qu'il garde dans son tiroir depuis 2018 — celle qu'il utilise pour les présentations en salle de réunion. Il efface le log de copie dans son historique récent, mais le serveur SharePoint garde un journal d'audit automatique (ce qu'il ne sait pas, et ce qu'Helix n'ira vérifier que trop tard).

**Source d'inspiration :** Antoine Deltour (LuxLeaks) — employé PwC qui a copié des documents internes auxquels il avait accès dans le cadre de son travail, pas par effraction. Frances Haugen (Facebook Papers) — a téléchargé des recherches internes via son accès standard d'employée. Le point commun : ce n'est jamais un hack spectaculaire, c'est un accès légitime utilisé pour copier ce qu'on n'était pas censé voir.

---

### Zone 2 : "Son directeur, embarrassé"

**Citation :** "Marc remonte le signal à sa hiérarchie. Son directeur, embarrassé, lui dit que ces données 'nécessitent une contextualisation statistique'"
**Catégorie :** Personnage carton
**Problème :** Ce directeur apparaît une fois, dit une phrase, et disparaît. Qui est-il ? Pourquoi cette réaction ?

**Enrichissement :**
Philippe Morand, 48 ans, directeur de la pharmacovigilance chez Helix. Le supérieur direct de Marc. Un ancien du CRPV (Centre Régional de Pharmacovigilance) de Bordeaux, recruté par Helix en 2015 avec un salaire x3. Il sait lire des données. Il sait exactement ce que le signal signifie. Mais il a signé, en 2019 justement, le rapport de synthèse du PSUR n°4 où il écrivait "aucun signal de néphrotoxicité identifié à ce jour". Si le signal de RENEW-3 est réel, alors son propre rapport au PSUR n°4 est un faux — il l'a signé alors que Deshayes avait déjà envoyé l'email à Weil. Morand n'est pas méchant. Il est piégé. S'il valide le signal de Marc, il s'incrimine lui-même.

Quand Marc entre dans son bureau avec les courbes de RENEW-3, Morand regarde les données 30 secondes, se pince l'arête du nez, et dit textuellement : "Marc, les cohortes de RENEW-3 avaient un profil rénal de base plus dégradé. Avant de tirer des conclusions, il faut contextualiser. Ce n'est pas ton périmètre direct. Laisse les biostatisticiens faire leur travail." C'est mot pour mot l'argument que Weil a donné à Deshayes dans l'email de mars 2019. La phrase circule chez Helix comme un mot de passe. Morand la répète sans même savoir qu'il cite Weil.

**Source d'inspiration :** Structure hiérarchique de Servier dans l'affaire Mediator — les cadres intermédiaires qui signaient des rapports de pharmacovigilance "propres" alors que les signaux existaient. Le Dr Aquilino Morelle, rapporteur de l'IGAS, a documenté comment la chaîne de commandement transformait des scientifiques honnêtes en complices passifs.

---

### Zone 3 : Comment Marc contacte Thomas Kerjean

**Citation :** "Thomas Kerjean, avocat en droit de la santé, 31 ans, accepte de le défendre pro bono"
**Catégorie :** Personnage carton + Mécanisme non expliqué
**Problème :** Pourquoi Thomas accepte ? Comment Marc le trouve ? C'est trop commode.

**Enrichissement :**
Marc ne trouve pas Thomas. C'est Thomas qui le trouve. Après le licenciement de Marc, l'ANSM accuse réception de son signalement (formulaire Cerfa n°10011, déclaration d'effet indésirable par un professionnel de santé). L'accusé de réception est un document standard — pas une validation, juste un "on a bien reçu". Mais le signalement est indexé dans la base EudraVigilance, accessible aux professionnels. Thomas Kerjean, qui prépare une thèse à l'Université Lyon 3 sur la responsabilité pénale des laboratoires en cas de pharmacovigilance défaillante, tombe sur le signalement en faisant une veille de routine. Il contacte Marc par LinkedIn — un message de 4 lignes, envoyé à 23h40 un mardi.

Thomas accepte parce que c'est exactement son sujet de thèse. Littéralement. Sa thèse s'intitule "L'obligation de signalement des signaux de sécurité en phase IV : de la passivité réglementaire à la responsabilité pénale". Marc est son cas d'étude vivant. Ce n'est pas de l'idéalisme pur — c'est aussi de l'ambition académique. Thomas sait que s'il gagne ce procès, sa carrière est faite. Il le dit à Marc au deuxième café : "Je vais pas te mentir. Si on gagne, ma thèse devient un bouquin, et le bouquin me lance. On a tous les deux quelque chose à y gagner." Marc apprécie l'honnêteté.

Thomas travaille depuis un bureau de 11m² au troisième étage d'un immeuble de la rue Mercière, au-dessus d'un restaurant libanais. Il partage le bail avec une avocate en droit du travail qui fait du divorce le reste du temps. Il n'a pas de secrétaire. Son imprimante est une HP LaserJet de 2014 qui bourre une fois sur trois.

**Source d'inspiration :** Irène Frachon et ses alliés dans l'affaire Mediator — des jeunes médecins, des internes, des chercheurs qui l'ont rejointe parce que le dossier croisait leurs propres travaux. L'alliance naît du hasard professionnel, pas d'un casting de film.

---

### Zone 4 : Claire — personnage carton

**Citation :** "Claire ne veut pas nuire à Marc, mais elle veut protéger Léa et Hugo"
**Catégorie :** Personnage carton + Raccourci émotionnel
**Problème :** Claire n'est qu'une fonction narrative ("la femme qui part"). On ne sait rien d'elle. C'est condescendant et plat.

**Enrichissement :**
Claire Vasseur, née Renaud, 39 ans, infirmière de bloc opératoire au centre hospitalier Lyon-Sud (Pierre-Bénite). Elle travaille en chirurgie viscérale, bloc B2, planning en 12 heures. Elle gagne 2 100€ nets. Elle sait ce que c'est, un patient en insuffisance rénale — elle en voit les conséquences sur la table d'opération (fistules artérioveineuses pour la dialyse, transplantations rénales ratées).

Claire ne part pas parce qu'elle ne comprend pas. Elle part parce qu'elle comprend TROP BIEN. Elle sait que Marc a probablement raison. Elle a lu l'article dans *Pharmacoepidemiology*. Elle a même vérifié sur UpToDate — les SGLT2i et la néphroprotection, elle connaît le sujet mieux que la plupart des avocats. Ce qui la brise, ce n'est pas l'enjeu. C'est le calcul. Marc a choisi de sauver 15 000 patients anonymes plutôt que de protéger deux enfants qui portent son nom. Elle ne lui reproche pas d'avoir raison. Elle lui reproche d'avoir choisi.

Le moment de la rupture n'est pas une scène de cris. C'est un mardi soir. Marc est chez son ami depuis trois semaines, il est passé récupérer des affaires. Hugo, 4 ans, est assis sur le canapé avec un cahier de coloriage. Il lève la tête et dit : "Tu dors ici ce soir ?" Marc hésite. Claire, depuis la cuisine, dit sans se retourner : "Dis-lui la vérité." Marc dit "Non, bonhomme, pas ce soir." Hugo retourne à son coloriage. Claire ferme le robinet et dit, toujours sans se retourner : "Les papiers du divorce sont sur la table de l'entrée. J'ai mis des post-it là où tu dois signer."

Claire part à Annecy parce que ses parents ont une maison avec un jardin et que Léa peut aller à l'école de Seynod à pied. Pas parce que les avocats d'Helix l'y ont poussée. Les avocats d'Helix n'ont fait qu'accélérer ce qui était déjà en cours — en faisant fuiter l'article de presse sur "l'ex-employé aigri", ils ont donné à l'avocate de Claire un argument pour la résidence principale. Mais Claire serait partie quand même.

**Source d'inspiration :** Témoignages de familles de lanceurs d'alerte dans le documentaire *The Insider* (1999, sur Jeffrey Wigand vs Brown & Williamson), et dans les interviews de Lindsay Mills (compagne d'Edward Snowden). Le point commun : le conjoint n'est pas l'ennemi, il est la victime collatérale lucide.

---

### Zone 5 : Arthur Weil — personnage carton

**Citation :** "Il ne quitte jamais son bureau... Il a toujours délégué."
**Catégorie :** Personnage carton
**Problème :** Weil est un méchant de carton. "PDG arrogant qui ne sort pas de son bureau." On peut faire mieux.

**Enrichissement :**
Arthur Weil, 62 ans. Diplômé de la faculté de pharmacie de Strasbourg (1986), thèse sur les transporteurs rénaux du glucose — ironie : c'est sa thèse qui a posé les bases théoriques de ce qui deviendra les SGLT2i, vingt ans plus tard. Il a cofondé Helix en 1994 avec un collègue de fac et 200 000 francs empruntés à son père, dentiste à Colmar. Pendant quinze ans, Helix était un petit CRO (Contract Research Organization) qui sous-traitait des essais cliniques pour les gros labos. Weil dormait au bureau, mangeait des sandwiches, embauchait des stagiaires qu'il payait au lance-pierre.

En 2011, le déclic : une de ses équipes de recherche tombe sur la molécule HX-4127, un inhibiteur dual SGLT1/SGLT2. Weil reconnaît immédiatement le potentiel — c'est son sujet de thèse, vingt-cinq ans plus tard. Il mise tout dessus. Il hypothèque le siège d'Helix. Il lève 80 millions auprès de fonds de capital-risque. RENEW-1 est lancé en 2015. Les résultats à 18 mois sont spectaculaires. Le Nexaril est approuvé par l'EMA en 2018. En trois ans, Helix passe de 200 à 15 000 employés. Weil est en couverture des *Échos* ("Le pharmacien qui défie les géants").

Weil ne cache pas les données de RENEW-3 par cupidité. Il les cache parce que le Nexaril est sa thèse, son pari, son héritage. C'est son oeuvre scientifique autant que commerciale. Admettre que le SGLT1 est toxique, c'est admettre que son intuition fondatrice — la dual inhibition — était une erreur. Ce n'est pas 3,1 milliards qu'il protège. C'est 35 ans de sa vie.

C'est pour ça qu'il ne sort pas de son bureau. Ce n'est pas de l'arrogance. C'est de la peur. Dehors, il y a la réalité. Dans son bureau du 12ème étage, avec ses écrans Bloomberg, ses rapports filtrés par trois niveaux de management, ses visioconférences où tout le monde acquiesce — là, le Nexaril est toujours le médicament miracle. Weil ne ment pas au monde. Il se ment à lui-même.

**Source d'inspiration :** Jacques Servier — fondateur des Laboratoires Servier, pharmacien de formation, qui avait bâti son entreprise sur une molécule (le benfluorex/Mediator) et qui a refusé jusqu'à sa mort de reconnaître sa toxicité. Arthur Sackler (Purdue Pharma) — visionnaire du marketing pharmaceutique qui a transformé un opioïde en blockbuster. Le point commun : des fondateurs-scientifiques qui finissent par confondre leur ego avec leur molécule.

---

### Zone 6 : Le licenciement — comment ça se passe concrètement

**Citation :** "Marc est convoqué aux RH à 14h. Licencié pour faute grave à 14h30. Badge désactivé à 14h32."
**Catégorie :** Mécanisme non expliqué
**Problème :** C'est cinématographique mais pas réaliste. En droit français, on ne licencie pas quelqu'un en 30 minutes.

**Enrichissement :**
En réalité, c'est plus sournois. Marc est d'abord convoqué à un "entretien préalable au licenciement" par lettre recommandée — délai légal de 5 jours ouvrables. Pendant ces 5 jours, il est mis à pied à titre conservatoire : badge désactivé, accès aux serveurs coupé, email professionnel suspendu. Il doit rendre son ordinateur portable et son téléphone de fonction. On lui laisse 20 minutes pour vider son bureau sous la supervision d'un agent de sécurité (un intérimaire de Securitas, pas un employé Helix — pour éviter la gêne). Marc met ses affaires dans un carton Bankers Box : une photo de Léa et Hugo à la mer, un mug "World's Okayest Pharmacologist" offert par un collègue, trois classeurs de notes, et un exemplaire annoté du *Goodman & Gilman's Pharmacological Basis of Therapeutics*, 13ème édition.

L'entretien a lieu le vendredi suivant. Salle Pasteur, RH, 2ème étage. La DRH, Nathalie Combe, est accompagnée d'un avocat de Bresson-Hartmann (déjà). Marc est venu seul — il a le droit à un conseiller du salarié mais il n'a pas eu le temps d'en trouver un. La DRH lit le motif : "violation grave et délibérée de l'obligation de confidentialité prévue à l'article 12.3 de votre contrat de travail et à l'article L. 1227-1 du Code du travail, ayant consisté en la transmission d'informations confidentielles relatives aux essais cliniques du programme RENEW à une autorité extérieure sans autorisation préalable de la direction." Marc demande s'il peut répondre. L'avocat dit "Tout ce que vous direz pourra être utilisé dans la procédure pénale en cours." Marc ne dit rien.

La lettre de licenciement arrive 4 jours plus tard par recommandé. Faute grave : pas de préavis, pas d'indemnité de licenciement. Solde de tout compte : 847,22€ (congés payés restants).

**Source d'inspiration :** Procédure de licenciement d'Antoine Deltour chez PwC Luxembourg (LuxLeaks). Procédure utilisée contre des lanceurs d'alerte dans l'affaire UBS France (Stéphanie Gibaud). Le schéma est toujours le même : mise à pied conservatoire immédiate, coupure des accès, puis procédure formelle.

---

### Zone 7 : "Marc tient, mais il maigrit" — raccourci émotionnel

**Citation :** "Chaque semaine un nouvel angle. Marc tient, mais il maigrit."
**Catégorie :** Raccourci émotionnel
**Problème :** On ne sent pas concrètement ce que vivent ces mois. C'est un résumé, pas une scène.

**Enrichissement :**
Le quotidien de Marc pendant les mois d'érosion : il vit chez Karim Bouyahia, un ancien collègue d'Helix (technicien de labo, parti en 2020 pour un poste chez bioMérieux). Karim a un deux-pièces à Villeurbanne, rue du 4-Août. Marc dort sur un clic-clac dans le salon. Il se lève à 6h quand Karim part au labo. Il passe les matins sur PubMed et ClinicalTrials.gov, en caleçon, avec le laptop personnel qu'il a acheté d'occasion sur Leboncoin (un ThinkPad T480, 180€). Il mange des pâtes Panzani et des boîtes de thon Petit Navire. Il a perdu 7 kilos en quatre mois. Pas de régime — il oublie de manger.

L'après-midi, il va à la bibliothèque municipale de la Part-Dieu (3ème étage, espace Civilisation, table 14 — celle qui est contre la vitre, avec une prise électrique). Il y travaille jusqu'à la fermeture à 19h. Les bibliothécaires le connaissent. L'une d'elles, Mme Joubert, lui apporte parfois un café du distributeur sans rien dire.

Le plus dur, c'est les dimanches. Karim sort avec sa copine. Marc est seul dans le deux-pièces. Il appelle Léa sur le téléphone de Claire. Léa raconte l'école. Hugo veut pas parler, il fait la gueule. Claire dit "cinq minutes" au bout de trois minutes. Marc raccroche et reste assis sur le clic-clac pendant une heure, le téléphone à la main, sans rien faire.

Les procédures de Bresson-Hartmann arrivent par courrier. Toujours des recommandés. Karim, en rentrant du labo, trouve les avis de passage dans la boîte aux lettres. Il ne dit rien, mais Marc voit bien qu'il commence à regretter d'avoir proposé le clic-clac.

---

### Zone 8 : La procédure d'expulsion

**Citation :** "Helix, via un fonds d'investissement filiale (Helix Capital Partners), rachète la créance à la banque et lance la procédure d'expulsion"
**Catégorie :** Fait technique vague
**Problème :** Est-ce que c'est juridiquement plausible ? Comment ça marche concrètement ?

**Enrichissement :**
Helix ne peut pas racheter directement la créance immobilière de Marc — ce serait trop visible et constituerait un abus de droit caractérisé. En réalité, c'est plus subtil. Le prêt immobilier de Marc est chez LCL, agence de Villeurbanne-Gratte-Ciel. Après 6 mois d'impayés, LCL déclenche la déchéance du terme (clause de l'article 1184 du Code civil) : tout le capital restant dû — 142 000€ — devient exigible immédiatement. LCL met le prêt en recouvrement contentieux et cède la créance à un fonds de titrisation, comme c'est la norme. Le fonds qui rachète le lot de créances douteuses s'appelle Themis Recovery Partners. C'est un véhicule luxembourgeois dont les investisseurs sont opaques — mais l'un des limited partners est Helix Ventures, la branche capital-risque d'Helix Corp. Helix ne "rachète" pas la créance de Marc spécifiquement. Mais Themis, une fois en possession du lot, fait preuve d'un zèle particulier sur le dossier Vasseur : commandement de payer signifié par huissier sous 8 jours, assignation devant le juge de l'exécution du TJ de Lyon, demande d'expulsion sans délai. La procédure standard prendrait 18 mois. Celle de Marc en prend 5. L'avocate de Themis, au téléphone avec Thomas Kerjean, dit : "On ne fait aucun traitement de faveur, maître. Le dossier est traité comme tous les autres." Thomas sait que c'est faux. Mais le prouver exigerait une enquête sur la structure capitalistique de Themis que ni lui ni Marc n'ont les moyens de financer.

**Source d'inspiration :** Mécanismes de titrisation de créances douteuses (NPL — Non-Performing Loans) utilisés par les banques européennes depuis 2015 (directive BCE). Le rachat indirect de créances pour exercer une pression est documenté dans plusieurs affaires de harcèlement judiciaire (Strategic Lawsuit Against Public Participation — procédures SLAPP). L'opacité des fonds luxembourgeois est un classique du montage.

---

### Zone 9 : L'offre de NDA

**Citation :** "Helix lui a fait passer le message via un intermédiaire. 400 000 euros et un NDA."
**Catégorie :** Mécanisme non expliqué
**Problème :** "Un intermédiaire" — qui ? comment ?

**Enrichissement :**
L'offre ne vient pas d'Helix directement. Elle arrive par un ancien professeur de Marc à la fac de pharmacie de Lyon — le Pr. Jean-François Martel, aujourd'hui retraité, qui fait du conseil pour l'industrie à travers un cabinet de consulting (Martel & Associates, société unipersonnelle). Martel invite Marc à déjeuner au Café du Soleil, place Bellecour. Ton paternel. "Marc, je te parle en ami. J'ai des gens qui m'ont contacté. Pas Helix directement, un intermédiaire. Ils proposent 400 000 euros, une clause de non-dénigrement, et le retrait de la plainte pénale pour vol de données. Tu retrouves ta vie. Tu peux racheter un appartement. Claire et les enfants reviennent peut-être. Tu republies dans deux ans sous un autre angle. Personne n'a besoin de savoir."

Marc regarde les lardons dans sa salade lyonnaise. Il demande : "Et les 15 000 patients sous Nexaril qui vont perdre leurs reins, Jean-François ?" Martel pose sa fourchette. Long silence. "Marc, tu n'es pas en position de sauver le monde." Marc demande l'addition.

Le chiffre de 400 000€ n'est pas arbitraire. C'est à peu près ce qu'il faudrait à Marc pour rembourser sa dette LCL (142 000€), payer les frais d'avocat de Claire (18 000€), et avoir de quoi vivre deux ans sans salaire. Quelqu'un chez Helix a fait le calcul précis de ce que vaut la vie de Marc en euros. Le message est clair : on sait exactement ce que tu dois, et on peut faire disparaître le problème.

**Source d'inspiration :** Les transactions confidentielles proposées par Merck aux plaignants dans l'affaire Vioxx (4,85 milliards de dollars de fonds de settlement). L'utilisation d'intermédiaires "neutres" — souvent des universitaires consultants — pour transmettre les offres, documentée dans l'affaire Mediator (Servier utilisait des professeurs de médecine comme relais).

---

### Zone 10 : La fuite des données aux médias

**Citation :** "il transmet les données brutes de RENEW-3 — les fichiers .csv des 14 000 patients, non anonymisés — à Mediapart, au BMJ, et au Monde simultanément"
**Catégorie :** Mécanisme non expliqué
**Problème :** Comment Marc transmet des données sensibles à trois médias en même temps ? C'est un acte grave et complexe, pas un email.

**Enrichissement :**
Marc ne contacte pas les trois médias le même jour. Il prépare ça depuis des semaines.

Mediapart d'abord. Thomas connaît une journaliste de la cellule investigation de Mediapart — Émilie Sardou, qui a couvert l'affaire Dépakine (Sanofi, valproate et malformations foetales). Thomas l'appelle. Sardou est intéressée mais prudente. Elle demande à voir les données avant de s'engager. Marc lui transmet un échantillon anonymisé (500 patients, pas les 14 000) via SecureDrop — le système de transmission sécurisée de Mediapart, basé sur Tor. Sardou fait vérifier l'échantillon par un biostatisticien indépendant (un maître de conférences à l'ISPED de Bordeaux qui travaille régulièrement avec Prescrire). Le biostatisticien confirme : le signal est réel. Sardou donne le feu vert.

Le *BMJ* : Marc contacte l'éditeur de la section "Research Integrity" directement par email, en joignant son article publié dans *Pharmacoepidemiology* et une lettre de 3 pages expliquant ce qu'il a. Le *BMJ* a une politique de protection des sources depuis l'affaire Andrew Wakefield. Ils acceptent de recevoir les données via un serveur sécurisé.

*Le Monde* : c'est Sardou de Mediapart qui fait le lien avec un journaliste du service Santé du Monde. Accord entre les deux rédactions pour une publication simultanée — pratique courante dans le journalisme d'investigation (cf. Panama Papers, LuxLeaks).

Le jour J, Marc envoie les fichiers complets (.csv, 14 000 patients, non anonymisés) aux trois rédactions. Il le fait depuis le ThinkPad de Leboncoin, connecté au WiFi de la bibliothèque de la Part-Dieu. Il sait que c'est traçable. Il s'en fout. C'est le sacrifice de la dame — après ça, sa carrière est morte.

Le fait que les données soient non anonymisées est un choix délibéré. Des données anonymisées, Helix pourrait arguer qu'elles sont fabriquées. Avec les numéros de patients, les dates de visite, les noms des centres investigateurs — les données sont vérifiables. Et c'est aussi ce qui rend l'acte de Marc illégal : transmettre des données de santé à caractère personnel non anonymisées est une violation du RGPD et de la loi Informatique et Libertés. Marc le sait. C'est le prix.

**Source d'inspiration :** Transmission des Facebook Papers par Frances Haugen au Wall Street Journal (SecureDrop). Coordination inter-rédactions des Panama Papers (ICIJ). Méthode de transmission des LuxLeaks (Antoine Deltour → journaliste Édouard Perrin → ICIJ).

---

### Zone 11 : Moreau — le fantôme

**Citation :** "Demandez à Moreau de réajuster le modèle statistique"
**Catégorie :** Personnage carton
**Problème :** Moreau est mentionné dans l'email de Weil mais n'existe jamais dans l'histoire. Qui est-il ? Est-il complice ?

**Enrichissement :**
Dr. Stéphane Moreau, 44 ans, directeur biostatistique chez Helix. Normalien (ENS Lyon, promotion 2002), agrégé de mathématiques, thèse en biostatistique à l'ISPED de Bordeaux. C'est le meilleur statisticien d'Helix et il le sait. Quand Weil lui demande de "réajuster le modèle en intégrant l'hétérogénéité des cohortes en baseline", Moreau comprend immédiatement ce qu'on lui demande : stratifier les patients de sorte à diluer le signal. Techniquement, ce n'est pas falsifier des données — c'est choisir un modèle statistique qui produit le résultat souhaité. En biostatistique, c'est ce qu'on appelle le p-hacking ou le "garden of forking paths" : avec assez de variables, on peut toujours trouver un sous-groupe où le signal disparaît.

Moreau le fait. Il exclut les patients avec un DFG de base <60 mL/min (environ 22% de la cohorte — les plus malades, ceux chez qui l'effet est le plus visible). Le signal passe de p=0.003 à p=0.08. Plus significatif. Il archive le modèle original dans un sous-dossier nommé "deprecated_models" et envoie le nouveau rapport à Deshayes. Le rapport porte la mention "V2 — adjusted for baseline heterogeneity."

Moreau ne témoignera jamais au procès. Il a quitté Helix en 2021 pour un poste chez Roche, à Bâle. Mais son modèle V2 — et surtout l'existence du V1 dans le dossier "deprecated_models" — sera retrouvé par les experts judiciaires mandatés par le juge après le versement de l'email. C'est une bombe à retardement qui explosera dans la procédure d'appel.

**Source d'inspiration :** Le p-hacking est un problème documenté et massif dans la recherche pharmaceutique (voir : John Ioannidis, "Why Most Published Research Findings Are False", 2005). Dans l'affaire Vioxx, Merck avait demandé à ses statisticiens de présenter les données cardiovasculaires sous un angle spécifique (argument du "naproxen cardioprotecteur" plutôt que "Vioxx cardiotoxique") — même données, deux histoires différentes.

---

### Zone 12 : L'article dans *Pharmacoepidemiology and Drug Safety*

**Citation :** "Il publie un article dans Pharmacoepidemiology and Drug Safety"
**Catégorie :** Mécanisme non expliqué
**Problème :** Comment un pharmacologue licencié, sans affiliation, publie dans une revue à comité de lecture ?

**Enrichissement :**
C'est le point le plus difficile de l'Acte II, et Marc a failli ne pas y arriver. Sans affiliation institutionnelle, un auteur est suspect. Marc soumet l'article en tant que "chercheur indépendant" — adresse personnelle, aucun conflit d'intérêts déclaré (puisqu'il n'a plus de lien avec Helix). Le premier reviewer recommande le rejet : "L'auteur ne fournit pas de données primaires et son hypothèse repose sur une extrapolation de données animales à des données humaines qu'il ne cite pas en source." Le deuxième reviewer, en revanche, est un pharmacologue clinicien qui travaille sur les SGLT2i — il reconnaît immédiatement la pertinence du signal et recommande une révision majeure.

L'éditeur de la revue, le Pr. Rachel Goldstein (Université de Pennsylvanie), est sensible au sujet. Elle a publié un éditorial en 2018 sur les angles morts de la pharmacovigilance post-marketing. Elle accorde à Marc une révision. Marc retravaille l'article pendant 6 semaines. Il ne peut pas citer les données de RENEW-3 (il ne les a pas officiellement). Mais il construit un argument indirect : la littérature sur SGLT1 + les données publiques de pharmacovigilance (base EudraVigilance, données agrégées) + l'étude de Tohoku. C'est un article d'hypothèse, pas une preuve. Mais l'hypothèse est solide et l'article est publié 4 mois après soumission.

L'article a 3 pages, pas 20. Mais Prescrire le reprend dans sa revue mensuelle avec un encadré : "Signal à surveiller." C'est ça qui met le feu aux poudres — Prescrire est lu par tous les généralistes de France.

**Source d'inspiration :** Publication des premières alertes sur le Mediator par Irène Frachon — d'abord des articles d'hypothèse dans des revues spécialisées, ignorés, puis repris par Prescrire qui a servi de caisse de résonance. La difficulté de publier sans affiliation est un problème réel documenté par les lanceurs d'alerte scientifiques.

---

### Zone 13 : Le tribunal — procédure

**Citation :** "18 mars. Tribunal judiciaire de Lyon. Salle 2.14."
**Catégorie :** Fait technique vague
**Problème :** Quelle procédure exactement ? Pénal ? Civil ? Instruction ? Audience ?

**Enrichissement :**
La procédure est pénale. Thomas a déposé une plainte avec constitution de partie civile pour mise en danger de la vie d'autrui (article 223-1 du Code pénal : "le fait d'exposer directement autrui à un risque immédiat de mort ou de blessures de nature à entraîner une mutilation ou une infirmité permanente par la violation manifestement délibérée d'une obligation particulière de prudence ou de sécurité imposée par la loi ou le règlement"). L'obligation violée : l'article R. 5121-166 du Code de la santé publique, qui impose au titulaire de l'AMM de notifier immédiatement tout fait nouveau de nature à modifier l'évaluation du rapport bénéfice-risque.

La plainte a d'abord été instruite par un juge d'instruction du pôle de santé publique du TJ de Paris (le pôle compétent pour les affaires sanitaires complexes — celui qui a instruit Mediator, Dépakine, prothèses PIP). Mais Thomas a demandé un dépaysement vers Lyon, juridiction du siège d'Helix. Le juge d'instruction de Lyon, Mme Catherine Vernier, a instruit pendant 8 mois avant de renvoyer Weil et Helix Corp devant le tribunal correctionnel.

Le 18 mars, c'est l'audience de jugement devant la 14ème chambre correctionnelle du TJ de Lyon. Salle 2.14, couloir B, deuxième étage. Trois juges. Un procureur. La salle fait 40 places. Il y en a 80 qui essaient d'entrer — une dizaine de journalistes, des représentants d'associations de patients diabétiques (AFD, Fédération Française des Diabétiques), et six personnes qui ne disent rien et prennent des notes : les observateurs envoyés par l'EMA.

**Source d'inspiration :** Procédure du procès Mediator au tribunal correctionnel de Paris (2019-2021, 6 mois d'audience, salle 2.13 du TJ de Paris). Procédure du procès Dépakine. Constitution de partie civile par des lanceurs d'alerte, mécanisme utilisé par Irène Frachon.

---

### Zone 14 : L'épilogue — trop rapide

**Citation :** "Helix Corp est condamné pour mise en danger de la vie d'autrui et tromperie aggravée."
**Catégorie :** Fait technique vague + Raccourci émotionnel
**Problème :** On résume le dénouement en 3 lignes. Quelles peines ? Que deviennent les patients ? Et Victor ?

**Enrichissement :**
La 14ème chambre correctionnelle rend son jugement six semaines après l'audience. Helix Corp (personne morale) : coupable de mise en danger de la vie d'autrui et de tromperie aggravée sur les qualités substantielles d'un produit. Amende de 2,7 millions d'euros (le maximum légal pour une personne morale à l'époque — dérisoire comparé aux 3,1 milliards de CA). Arthur Weil (personne physique) : 4 ans d'emprisonnement dont 2 avec sursis, et interdiction de gérer une entreprise pharmaceutique pendant 10 ans. Il fait appel.

Victor Deshayes n'est pas poursuivi pénalement — il est couvert par la prescription sur la période 2019-2021, et son témoignage au tribunal, bien que mensonger, n'a pas été qualifié de faux témoignage car il portait sur des "interprétations scientifiques" et non sur des faits matériels. Mais Deshayes démissionne d'Helix trois jours après le verdict. Il retrouve un poste de directeur médical chez un petit CRO à Strasbourg, à 60% de son ancien salaire. Sa femme reprend un emploi.

Le Nexaril est suspendu par l'EMA le jour du verdict ("décision de suspension d'AMM en urgence, article 20 du règlement CE 726/2004"). L'ANSM publie un point d'information pour les professionnels de santé : les patients sous Nexaril doivent être switchés vers un SGLT2i classique (dapagliflozine, empagliflozine) avec un contrôle de l'eGFR et des biomarqueurs tubulaires à M1, M3 et M6. Les associations de patients déposent une action de groupe devant le TJ de Paris — 3 400 patients inscrits dans les deux premiers mois. Le coût estimé des indemnisations : entre 800 millions et 1,2 milliard d'euros. Helix provisionne 900 millions dans ses comptes. Le cours de l'action chute de 74% en une semaine. Les fonds de capital-risque qui avaient misé sur le Nexaril en 2011 perdent tout.

Marc reçoit le statut de lanceur d'alerte au titre de la loi Sapin II (loi n°2016-1691), ce qui lui accorde une protection juridique rétroactive — la procédure pénale pour vol de données est abandonnée. Mais la radiation de l'Ordre des pharmaciens est maintenue pour la violation du RGPD (transmission de données non anonymisées). Marc ne peut plus exercer comme pharmacien. Il peut encore publier.

**Source d'inspiration :** Verdict du procès Mediator (Servier condamné à 2,7M€ d'amende — le maximum légal, absurdement bas). Suspension de l'AMM du Mediator par l'AFSSAPS (devenue ANSM). Loi Sapin II et statut de lanceur d'alerte appliqué rétroactivement. Action de groupe santé (loi de modernisation du système de santé, 2016).
