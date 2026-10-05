# Reprise de conversation : projet de jeu Steam

Ce fichier permet de reprendre le travail dans une nouvelle conversation avec Claude. Il contient tout le contexte nécessaire (partie A), puis le journal complet de la conversation d'origine, des 4 et 5 octobre 2026 (partie B).

> **Attention, dépôt public.** Ce dépôt GitHub est public et sert un site GitHub Pages. Si ce fichier est commité et poussé, il devient lisible par tout le monde, y compris les liens vers les Google Docs qu'il contient. Pour le garder privé, ne le commite pas, ou ajoute `REPRISE-CONVERSATION.md` au fichier `.gitignore`.

**Comment reprendre.** Ouvrir une nouvelle conversation Claude Code dans le dossier `C:\GitProjects\SteamMarketMapping`, puis écrire par exemple : « Lis REPRISE-CONVERSATION.md et reprends le projet là où on s'est arrêtés. » La partie A suffit pour reprendre ; la partie B sert de référence.

---

# Partie A : le contexte pour reprendre

## A1. Le projet

- **Qui.** Mathieu, game designer diplômé de Rubika. Son équipe : trois game designers qui pensent le projet, plusieurs artistes et au moins un programmeur, extensible. L'équipe est versatile et peut se scinder en deux projets si besoin. Consigne de Mathieu : ne pas se préoccuper des besoins en effectifs. Mathieu n'est **pas le seul décideur** : les documents doivent présenter son raisonnement pour convaincre les autres designers, pas annoncer une décision.
- **Historique.** Leur jeu étudiant « 12 Memory Lane » a été nominé aux Pégases, catégorie meilleur jeu étudiant.
- **Objectif.** Faire un jeu qui s'insère dans un marché, pas seulement un projet d'épanouissement créatif.
- **Cadrage décidé.** Plateforme cible : Steam (PC). Roblox, mobile et web écartés pour l'instant ; portage Epic ou autre envisageable plus tard. Sortie visée vers 2027-2028.
- **Phase actuelle.** Fin de l'étude de marché, début du cadrage de design. Le document de cadrage a été envoyé aux autres designers le 4 octobre 2026.

## A2. Les livrables et où ils se trouvent

| Livrable | Où | État |
|---|---|---|
| Site « Cartographie Steam 2026 » | https://mathieucabot.github.io/SteamMarketMapping/ (fichier `index.html` du dépôt) | En ligne via GitHub Pages, branche `main`, dossier racine. Thème sombre inspiré de finary.com. |
| Dépôt GitHub | https://github.com/MathieuCABOT/SteamMarketMapping | Public. Commits : « Publier le rapport en page GitHub Pages », « Refondre le rapport en document d'équipe », « Adopter une direction visuelle inspirée de Finary ». |
| Notes de données par famille de genres | `donnees/*.md` du dépôt | Chiffres sourcés et datés, issus de six collectes du 4 octobre 2026. |
| Extractions brutes Gamalytic | `donnees/gl_*.json` du dépôt | Cohortes 2024-2026 de six tags (tactique, horreur psychologique, farming, cozy, metroidvania, tactical RPG). |
| **Document de cadrage, version d'équipe** | Google Doc « Cadrage du projet Steam » : https://docs.google.com/document/d/1uvjEewOmD68vPNjaWXbgCSaJJKhGs6jSPLViLabZTn4/edit?usp=sharing | **Fait foi.** Exporté depuis le Claude Doc puis retouché par Mathieu. Texte complet en annexe A9. |
| Document de cadrage, version Claude | Claude Doc « Cadrage du projet Steam » : https://claude.ai/code/artifact/27523ffd-ceec-4d2e-9591-5c13cefe09f8 | Modifiable par Claude, mais **plus synchronisé** avec la version Google Docs. |
| Premier rapport publié | Artifact Claude « Cartographie Steam 2026 » : https://claude.ai/artifact/JgMttUuM3T7MM2XzFioFip | Version 1, ancienne. Remplacée par le site GitHub Pages. |
| Google Doc « design od » | https://docs.google.com/document/d/1cIbzovjsyNq7o3y3wkz5uzl7YPIaFEjTuI_VeeBJv6M/edit?usp=sharing | Quasiment vide, créé par Mathieu. Non utilisé. |
| Bandeaux d'images des jeux | `.claude/img/*.png` du dépôt (ignoré par git) | Sept bandeaux de vignettes Steam officielles, insérés dans le Claude Doc. |

## A3. La conclusion de l'étude de marché

**La proposition.** Un jeu coop systémique à concept clair, pour 2 à 8 joueurs entre amis, hébergé par un joueur, vendu entre 10 et 20 $, lancé en Early Access traité comme le vrai lancement. Ses systèmes fabriquent des histoires et chaque manche produit des moments qui se découpent en clips. Thème non-horreur, ou horreur mêlée à un autre registre. Le concept, le hook et le thème restent ouverts.

**Les cinq constats qui la fondent**, chacun écrit sous la forme constat, « Pourquoi », « Donc », « Limite » :

1. **Être découvert est le vrai goulot.** 20 282 jeux sortis en 2025, environ 24 000 attendus en 2026 ; 2,99 % dépassent 1 000 avis. Bō, 84 % d'avis positifs, a vendu 31 700 copies. Les trois canaux qui amènent des joueurs (algorithme Steam, amis, streamers) ne donnent que quelques secondes à chaque jeu.
2. **Le coop vend mieux, parce qu'un acheteur en entraîne d'autres.** Trois des cinq plus gros nouveaux indés de 2025 sont des coop à moins de 20 $ (Schedule I, R.E.P.O., Peak). Peak a converti ses wishlists 266 fois mieux que la médiane.
3. **La demande coop grandit mais change de jeu tous les 3 à 9 mois.** Records successifs de 197 000, 281 000 puis 366 000 joueurs simultanés ; un leader retombe à 10 % de l'audience en 3 à 9 mois. Rétention à 30 jours du friendslop : 3 %.
4. **La vidéo courte attire, mais c'est Steam qui fait vendre.** How Many Dudes? : deux Shorts ont apporté 769 wishlists, la démo et New & Trending 36 946.
5. **En coop, le prix se paie plusieurs fois.** Prix médian des hits passé de 19,50 $ à 15,64 $ entre 2023 et 2025. Quatre amis paient le prix quatre fois.

Sixième fait : le passage en 1.0 rapporte en médiane 40 % du premier mois d'Early Access.

**La carte.** Dix-sept familles placées sur deux axes : la place sur le marché, et la capacité à se faire découvrir et à durer sans budget marketing (clips et histoires). Quatre familles en haut à droite : friendslop, party physique, sim d'équipe coop, chaos coop systémique. Écartées : extraction, horreur asymétrique et sports compétitifs (dépendent d'inconnus en ligne) ; déduction sociale (un seul moment répété) ; colony sim, automation et tactique (histoires sans clips) ; roguelite, deckbuilder, survival, cozy et metroidvania (trop de monde) ; narratif court (pas d'histoire propre au joueur).

## A4. Le cadre de design

**Les piliers** décident du succès. Ils ne sont pas encore écrits ; le document fixe le niveau d'exigence de chacun.

- **Le hook**, la phrase qui résume le jeu et donne envie d'y jouer. Test : cinq personnes extérieures lisent le hook et décrivent une partie imaginaire ; si quatre décrivent la même chose, il tient.
- **La core experience**, ce que l'on fait concrètement pendant une partie. Test : sans explication, l'objectif est compris en moins d'une minute et le groupe relance une manche de lui-même.
- **L'identité esthétique.** Test : une image fixe prise au hasard, trois personnes nomment le jeu.

Quand un filtre entre en conflit avec un pilier, le pilier gagne.

**Filtre A, la clipabilité** (appelé « Lentille A » dans les premières versions). Onze statements testables sur un playtest filmé : unité de temps de 15 à 60 s ; lisibilité en deux secondes ; payoff net ; l'échec est le contenu ; variance ; réaction humaine amplifiée ; format vertical 9:16 ; signature en une image ; le clip est une publicité ; titrabilité en cinq mots ; capture facilitée (optionnel).

**Filtre B, l'anecdote factory** (« Lentille B »). Huit statements : causalité lisible ; attribution ; croisement d'au moins deux systèmes ; verbes polyvalents ; conséquence durable ; témoins ; longue queue ; racontable en trois phrases sans le jeu. Test central : le lendemain d'un playtest, demander à chaque joueur « raconte-moi une histoire de la partie ».

**Le protocole de validation** en cinq étapes : filmer un playtest de 30 à 45 minutes ; découper et compter les moments clipables (cible : 1 par 10 minutes, 2 pour un party) ; auditer le filtre clip (7 clips sur 10 compris par trois inconnus, 8 sur 10 titrés en cinq mots, cinq clips lisibles en vertical) ; test du lendemain (une histoire par joueur, la moitié avec deux systèmes ou plus) ; décider après deux échecs consécutifs d'un statement. Les cibles sont des hypothèses à recalibrer sur les cent clips les plus vus d'une vingtaine de hits. Une fiche d'audit interactive est sur le site, section « Valider ».

## A5. Les points ouverts

**Corrections à faire dans le Google Doc d'équipe** (Claude ne peut pas modifier le corps d'un Google Doc) :

| Passage actuel | Correction proposée |
|---|---|
| la mapping, de la mapping | le mapping, du mapping |
| un jeu de ce genre de jeu peut-il | un jeu de ce genre peut-il |
| Les jeux chaos coop systémique est le genre de jeu le plus ouvert | Le chaos coop systémique est le genre le plus ouvert |
| Des quatre genres de jeux…, c'est celle qui a le plus de place | …, c'est celui qui a le plus de place |
| Les deux filtre se recoupent…, mais elles se testent séparément : la première…, la seconde… | Les deux filtres se recoupent…, mais ils se testent séparément : le premier…, le second… |
| une étude que j'ai fait | une étude que j'ai faite |
| Je propose de passer un protocole, la fiche d'audit… en parle | Je propose de suivre un protocole, décrit dans la fiche d'audit… |
| riche en story auto généré | riche en histoires auto-générées |
| (comédie, absurde,etc) | (comédie, absurde, etc.) |

Autres points relevés dans la version d'équipe :

- Le tableau du filtre B renvoie au test du lendemain « décrit dans la section suivante », que la section 8 raccourcie ne décrit plus.
- Les liens internes (« section 2 », « constat 3 ») n'ont pas survécu à l'export ; Google Docs permet de les recréer avec Insérer un lien, puis Titres.
- La section 1 parle encore de « deux grilles de design » alors que les sections 6 et 7 s'appellent « Filtre A » et « Filtre B ».
- La légende de la carte dit « alignement clip + anecdote » ; l'axe s'appelle désormais « Se faire découvrir et durer ».
- Le test du hook a perdu son seuil de réussite (quatre sur cinq).
- « Physique based » apparaît deux fois ; à garder seulement si c'est un terme d'équipe assumé.
- Non vérifié : la présence des deux schémas et des sept bandeaux d'images dans le Google Doc (sa taille, 4,4 Mo, laisse penser qu'ils y sont).

**Décisions laissées à l'équipe** (section 11 du Claude Doc, retirée de la version Google Docs) : valider ou contester le périmètre ; choisir le registre thématique ; fixer la fenêtre de sortie et le Next Fest visé ; ouvrir une ou deux pistes de prototype ; nommer un responsable du corpus de clips ; ajuster les cibles chiffrées après le premier playtest ; trancher auto-édition ou éditeur. Questions ouvertes : budget et durée avant la première porte ; mode solo jouable ou non.

**Commentaire resté sans réponse** dans le Claude Doc : l'exclusion de l'horreur pure (seule l'horreur hybridée est gardée) est-elle confirmée, ou faut-il la garder comme piste à part entière ?

## A6. Les préférences de travail de Mathieu

- Langue : français. Ton de GD senior spécialisé marché Steam, pragmatique, fondé sur les données plutôt que les intuitions.
- **Économiser les tokens** : limiter les agents parallèles. La première collecte a coûté environ 1,3 million de tokens.
- **Définir chaque terme** à sa première apparition (friendslop, clip, Next Fest, anecdote factory…).
- **Raisonnements explicites et sans faille** : chaque argument suit le chemin constat chiffré, mécanisme, déduction, limite. Pas de saut logique, pas de chiffre mal sourcé, pas de pari présenté comme un fait.
- **Posture** : présenter un raisonnement pour convaincre ses pairs, à la première personne (« je propose »), pas une décision.
- Documents **courts**, agréables à lire, style Notion, aérés par des images (vignettes des jeux cités) et des liens cliquables entre sections.
- Distinguer partout les chiffres sourcés, estimés et les lectures d'analyste.
- Mathieu reprend lui-même les documents et a remplacé « familles » par « genres de jeux » et « lentilles » par « filtres ».

## A7. Notes techniques utiles

- **Google Drive** : le connecteur de Claude peut lire un Google Doc, en créer un nouveau, le renommer ou le déplacer, mais pas modifier le corps d'un document existant. Export Claude Doc vers Google Docs : clic sur le nom du document, puis Export, puis Google Docs ; c'est une action de l'utilisateur. Par le connecteur, l'export HTML perd les schémas.
- **Claude Doc** : liens internes créés avec une opération `format` qui ajoute un lien `#<id du titre>` ; images ajoutées en téléversant les fichiers sur l'artifact du document, puis en créant un blob et en l'insérant en markdown `![alt](blob/<id>)`.
- **GitHub Pages** : `index.html` autonome à la racine, `.nojekyll` présent, `.gitignore` ignore `.claude/`.
- **Windows** : Python échoue sur les chemins de plus de 260 caractères ; travailler les images dans un dossier au chemin court.
- **Identifiants Steam vérifiés** : Schedule I 3164500, R.E.P.O. 3241660, PEAK 3527290, Lethal Company 1966720, Meccha Chameleon 4704690, Balatro 2379780, How Many Dudes? 3934270, Bō 1614440, RimWorld 294100, Phasmophobia 739630, Abiotic Factor 427410, Chained Together 2567870, RV There Yet? 3949040, Marathon 3065800, Texas Chain Saw Massacre 1433140, Liar's Bar 3097560, Mewgenics 686060.
- **Mémoire de Claude** : la conversation d'origine tournait dans un dossier temporaire, et sa mémoire persistante y est rattachée. Une nouvelle conversation ouverte dans ce dépôt ne la retrouvera pas : ce fichier la remplace.

## A8. Sources principales de l'étude

Chris Zukowski (howtomarketagame.com), Simon Carless (newsletter GameDiscoverCo), Alinea Analytics, Naavik, Game Developer, Gamalytic, VG Insights, Steambase, SteamCharts, SullyGnome, TwitchTracker, pages Steam. Liste détaillée et datée dans `index.html` et `donnees/*.md`.

## A9. Annexe : texte de la version d'équipe du document de cadrage

Texte du Google Doc « Cadrage du projet Steam » tel que relu le 4 octobre 2026, sans les images ni les schémas. Les deux schémas sont signalés par leur légende.

---

**Cadrage du projet**

Ce document présente mon raisonnement, il part d'une étude que j'ai fait (4 octobre 2026) et arrive à une proposition de marché cible, de contraintes et de méthodes.

L'analyse : https://mathieucabot.github.io/SteamMarketMapping

**1. Le raisonnement en trois temps**

1. Sur Steam, la qualité est nécessaire mais ne suffit plus : le vrai obstacle est d'être découvert. Le marché récompense les jeux qui se comprennent en une phrase, se jouent entre amis et coûtent peu. Section 2.
2. J'ai donc classé les genres de jeux selon deux questions : reste-t-il de la place, et un jeu de ce genre de jeu peut-il se faire découvrir et durer sans budget marketing ? Quatre genres de jeux répondent oui aux deux. J'en tire un périmètre. Sections 3 et 4.
3. Pour que ce périmètre tienne, deux grilles de design, un protocole de validation, des pièges à éviter et un calendrier. Sections 5 à 10.

Chaque argument suit le même chemin : un constat chiffré, le mécanisme qui l'explique, ce que j'en déduis, et sa limite. Les sections 2 à 4 se lisent en dix minutes. Chaque chiffre vient de la mapping Steam 2026, où il est daté et sourcé.

**2. Ce que j'ai retenu du marché**

J'ai cherché ce que Steam récompense aujourd'hui, pas ce qui est à la mode. Cinq constats ressortent, et ils poussent tous dans la même direction.

*1. Être découvert est le vrai goulot*

Steam a publié 20 282 jeux en 2025 et en attend environ 24 000 en 2026, soit près de 70 par jour. Seuls 2,99 % dépassent 1 000 avis, le seuil qui correspond à environ 150 000 $ de revenus. Et ce n'est pas qu'une question de qualité : Bō, noté 84 % positif, a vendu 31 700 copies.

Pourquoi. Les trois canaux qui amènent des joueurs ne donnent que quelques secondes à chaque jeu : l'algorithme de Steam montre une vignette et un titre, un ami recommande en une phrase, et les streamers choisissent d'abord selon la tendance et ce que leur audience comprendra.

Donc. Un concept qui se comprend en une phrase n'est pas un bonus marketing : c'est la condition pour passer par ces trois canaux.

Limite. RimWorld ou Factorio ont réussi sans concept d'une phrase, mais en quatre à cinq ans d'Early Access portés par de longues vidéos YouTube. C'est une route possible, plus lente ; j'y reviens en section 3.

*2. Le coop vend mieux, parce qu'un acheteur en entraîne d'autres*

Trois des cinq plus gros nouveaux indés de 2025 sont des jeux coop à moins de 20 $ : Schedule I, R.E.P.O. et Peak. Au-delà des hits, VG Insights estime qu'un jeu coop vend de l'ordre de 40 000 unités là où un jeu solo en vend 5 000. GameDiscoverCo classe le coop en ligne parmi les catégories qui convertissent le mieux leurs wishlists en ventes : Peak 266 fois la médiane, R.E.P.O. 68 fois.

Pourquoi. Un jeu coop s'achète en groupe. Le premier joueur convainc ses amis, qui achètent sans l'avoir jamais mis en wishlist : chaque vente en déclenche plusieurs.

Donc. Pour un studio nouveau, sans communauté ni budget marketing, le coop est le format qui dépend le moins d'une longue campagne de wishlists.

Limite. L'effet de groupe joue aussi à la baisse : un joueur sans amis disponibles n'achète pas. C'est un argument de plus pour un prix bas (constat 5).

*3. La demande coop grandit, mais change de jeu tous les quelques mois*

Dans les jeux coop à physique chaotique joués entre amis, le genre de jeu que le marché appelle « friendslop » (Lethal Company, Peak, R.E.P.O.), chaque nouveau leader bat le record du précédent : 197 000 joueurs simultanés fin 2023, 281 000 en 2025, 366 000 en 2026. Puis il retombe à 10 % de l'audience du genre en 3 à 9 mois.

Pourquoi. L'audience ne se lasse pas du format, elle se lasse du jeu et cherche le suivant : 61 % des joueurs de Peak possèdent aussi R.E.P.O.

Donc. Il y a une place à prendre tous les quelques mois, auprès d'une audience qui cherche activement. Mais un jeu qui ne vit que de sa nouveauté vivra trois à neuf mois.

Limite. Je n'ai pas de chiffre qui prouve qu'un jeu riche en histoires retienne mieux ses joueurs dans ce genre de jeu. C'est un pari, que j'argumente en section 7 et que le prototype peut tester.

*4. La vidéo courte attire, mais c'est Steam qui fait vendre*

Pour How Many Dudes?, sorti en juillet 2026, deux vidéos courtes virales (des « Shorts ») ont apporté 769 wishlists ; la démo et la mise en avant « New & Trending » de la boutique Steam en ont apporté 36 946. Balatro, plus de 5 millions de copies, a été lancé par 300 petits streamers et deux démos, sans TikTok.

Pourquoi. Une vidéo donne envie d'aller voir. C'est la page Steam, la démo et les avis qui transforment cette envie en achat.

Donc. Concevoir le jeu pour qu'il produise des clips, ces extraits courts de streams, multiplie la visibilité. Mais la démo et le Next Fest, le festival de démos de Steam, restent le cœur du plan.

Limite. Le ratio de How Many Dudes? vient d'un seul cas documenté. Pour Schedule I, les compilations TikTok de streams ont clairement pesé ; aucune étude ne chiffre l'effet en général.

*5. En coop, le prix se paie plusieurs fois*

Le prix médian de lancement des 50 jeux les plus vendus chaque mois est passé de 19,50 $ en 2023 à 15,64 $ en 2025. Tous les hits coop de 2025-2026 étudiés sont vendus entre 5 et 20 $.

Pourquoi. Un groupe de quatre amis paie le prix quatre fois. À 30 $, la soirée coûte 120 $ au groupe ; à 10 $, elle coûte le prix d'un repas, et l'achat devient impulsif.

Donc. Je propose un prix entre 10 et 20 $.

Limite. Des jeux plus chers marchent : Slay the Spire 2 à 25 $, Mewgenics à 30 $, et le segment 30 à 50 $ a progressé sur PC en 2025. Mais ce sont des suites, des licences ou des jeux solo très profonds, pas notre cas.

Un sixième fait pèse sur le calendrier : quand un jeu passe de l'Early Access à sa version 1.0, il rapporte en médiane 40 % de ce qu'il avait rapporté le premier mois d'Early Access. J'y reviens en section 10.

**3. Ma lecture de la carte**

J'ai placé les dix-sept genres de jeux de l'étude sur deux axes, qui découlent de la section 2. Le premier : reste-t-il de la place, c'est-à-dire une demande que l'offre ne couvre pas ? Le second : un jeu de ce genre de jeu peut-il se faire découvrir et durer sans budget marketing ?

Pour un studio sans audience, ce second axe repose sur deux capacités. Produire des moments que les streamers et leurs spectateurs partagent, des clips : c'est ce qui fait découvrir le jeu (constat 1 et constat 4). Et produire des histoires que les joueurs se racontent, des anecdotes : c'est ce qui le fait durer (constat 3). Les positions sont ma lecture des chiffres de la mapping, pas une mesure ; si vous en contestez une, la fiche du genre y donne les chiffres.

Quatre genres de jeux sont en haut à droite : le friendslop, le party physique, la sim d'équipe coop et le chaos coop systémique, c'est-à-dire des jeux coop dont plusieurs systèmes se croisent pour produire des accidents.

[Schéma : carte des genres de jeux · place sur le marché × alignement clip + anecdote]

Le quart supérieur gauche est tentant et fermé : ces genres se partagent très bien, mais un ou deux gagnants y retiennent les joueurs. Le quart inférieur droit est viable mais lent : de la place et des histoires, mais une découverte qui passe par des années d'Early Access et de longues vidéos. Le reste cumule les deux handicaps.

Ce qui me fait viser le quart supérieur droit

- Les jeux chaos coop systémique est le genre de jeu le plus ouvert, et le plus risqué. Schedule I (un développeur, 459 000 joueurs simultanés) et Abiotic Factor (dix personnes, 1,4 million de copies) ont percé avec un concept clair et deux ou trois systèmes qui se croisent, sans concurrent direct. La contrepartie : ce sont des succès déclenchés par un streamer, donc imprévisibles.
- Le friendslop a une demande qui grandit et une offre horreur saturée. Les clones horreur plafonnent depuis fin 2024 (Murky Divers : 204 joueurs au pic) ; les hits suivants sont une escalade, une partie de pêche, un camping-car. La place est dans les variantes non-horreur.
- La sim d'équipe coop marche, la sim solo non. Sur 38 jeux « Simulator » sortis en août 2025, un seul hors Waterpark Simulator a dépassé 70 000 $ de revenus. Les succès récents se jouent à plusieurs : Schedule I, Supermarket Simulator, RV There Yet? ; Dear Passengers a pris un million de wishlists en trois jours.
- Le party game physique based vit en ligne, plus sur canapé. Chained Together, un jeu français à 4,99 $, dépasse 10 millions de copies ; sept des dix meilleurs party games locaux datent d'avant 2021.

Pourquoi j'écarte le reste

- Extraction, horreur asymétrique, sports compétitifs : il faut des inconnus en ligne pour jouer. Quand la population baisse, l'attente de partie s'allonge, les joueurs partent, et le jeu cesse de fonctionner. Marathon a perdu 96 % de ses joueurs en six mois malgré 82 sur Metacritic ; Texas Chain Saw a été abandonné en moins de deux ans. Un jeu coop entre amis n'a pas ce problème : il fonctionne à quatre, même si personne d'autre ne joue.
- Déduction sociale : un seul moment, répété. Le genre se clippe très bien, mais chaque partie produit le même moment de vérité, qui lasse vite : aucun nouveau jeu n'y a dépassé 20 000 joueurs simultanés en 2026. Nous pouvons emprunter ce moment comme mécanique, pas en faire le jeu.
- Colony sim, automation, tactique : des histoires, mais pas de clips. Leurs moments forts demandent des heures de contexte : le dernier DLC de RimWorld a battu le record de chaînes Twitch, pas celui de spectateurs. Ces genres réussissent par la rétention et les longues vidéos, sur 4 à 5 ans d'Early Access. C'est une autre stratégie que celle que je propose.
- Roguelite, deckbuilder, survival, cozy, metroidvania : trop de monde. Les deux premiers en sont à leur troisième vague de suiveurs (le développeur de Vital Shell : « presque aucune réponse des streamers ») ; le survival est passé aux mains des licences et des studios de soixante personnes ; le cozy a triplé ses sorties en 2026 et sa médiane s'est effondrée.
- Narratif court : beaucoup de succès, aucune histoire propre au joueur. C'est le genre qui produit le plus de jeux à plus d'un million de dollars. Mais tout y est scénarisé : chaque joueur vit la même histoire, et un spectateur qui l'a vue n'a plus de raison de jouer.

**4. Ce que je propose**

Je propose un jeu coop systémique à concept clair, pour 2 à 8 joueurs entre amis, vendu entre 10 et 20 $, dont les systèmes fabriquent des histoires et dont chaque manche produit des moments qui se découpent. Le concept et le thème restent ouverts.

| Contrainte | Ma proposition | D'où elle vient |
|---|---|---|
| Genre de jeu | Chaos coop systémique, en lisière du friendslop non-horreur | Des quatre genres de jeux du quart supérieur droit, c'est celle qui a le plus de place : peu de concurrents directs et des hits récents faits par de petites équipes (section 3). Sa lisière avec le friendslop lui donne accès à une audience qui cherche déjà son prochain jeu (constat 3). |
| Nb de Joueurs | 2 à 8, en ligne, entre amis, hébergé par un joueur | Le coop vend en groupe (constat 2). Hébergé par un joueur, le jeu fonctionne même s'il n'a que dix joueurs dans le monde, sans serveurs ni attente de partie : c'est ce qui a manqué à Marathon et Texas Chain Saw. |
| Prix | 10 à 20 $, lancement 20 à 35 % moins cher la première semaine | Le groupe paie le prix plusieurs fois (constat 5). La remise de lancement est une pratique courante dans ce genre de jeu, et elle déclenche l'achat groupé pendant la semaine où l'attention est maximale. |
| Lancement | Early Access, traité comme le vrai lancement | C'est la norme de ce genre de jeu (Lethal Company, R.E.P.O., Schedule I) : il permet de sortir pendant que la fenêtre est ouverte, puis d'itérer avec les joueurs. Mais quatre jeux sur cinq gagnent moins à leur 1.0 qu'à l'ouverture de l'Early Access (sixième fait) : démo, Next Fest et streamers doivent être prêts dès l'ouverture. |
| Thème | Non-horreur, ou horreur hybridée avec un autre registre (comédie, absurde,etc) | L'offre horreur du friendslop est saturée depuis fin 2024, et les hits suivants sont ailleurs (constat 3, section 3). |
| Structure | Des manches avec un objectif et une fin, pas une sandbox ouverte | Les hits de ce genre de jeu sont structurés ainsi : un quota à atteindre (Lethal Company), un sommet (Peak), une extraction (R.E.P.O.). Une manche donne un enjeu aux accidents, donc des histoires, et un début et une fin aux clips. |
| Systèmes | Deux ou trois systèmes indépendants qui se croisent, des verbes polyvalents | C'est ce qui produit des situations que personne n'a écrites, donc des histoires propres à chaque groupe (section 7). Un seul système ne produit que des variations ; deux systèmes indépendants produisent des collisions. |

Ce que je propose d'exclure, et pourquoi

- Le PvP entre inconnus, le free-to-play, le live service : ils dépendent d'une population en ligne que nous ne pouvons pas garantir (section 3).
- Une sortie collée à un mastodonte du même genre : l'audience migre en bloc vers le plus gros (constat 3). Burglin' Gnomes, deuxième du Next Fest de février 2026, a été étouffé le jour de la sortie de Meccha Chameleon. Et pas d'octobre si le jeu touche à l'horreur : c'est le mois le plus encombré et le troisième pire en revenu.

**5. Les piliers**

Trois piliers décident du succès : le hook, la phrase qui résume le jeu et donne envie d'y jouer ; la core experience, ce que l'on fait concrètement pendant une partie ; et l'identité esthétique. Voici le niveau d'exigence que je propose pour chacun de ces points

*Le hook*

Une phrase qui décrit une situation, pas un genre. « Quatre amis portent un coffre fragile dans une maison hantée » est un hook. « Un coop horreur à physique based » n'en est pas un.

- Critère. Une phrase qui décrit une situation, pas un genre, et qu'un streamer peut expliquer sans avoir joué. Peak tient en une phrase : des amis escaladent ensemble une montagne, et une chute peut coûter la partie. Lancé avec 29 000 wishlists, 15,5 M de copies.
- Test. Cinq personnes extérieures lisent le hook et décrivent une partie imaginaire.

*La core experience*

La boucle d'une manche : ce que les joueurs font minute après minute, ce qui crée la tension, ce qui la résout.

- Critère. Une manche avec un début, un objectif et une fin ; un échec plus intéressant que la réussite et qui ne coûte qu'une manche ; des joueurs dépendants les uns des autres par construction. Peak a ajouté de la friction sociale volontaire : sac inaccessible seul, guide lisible par un seul joueur, morts qui deviennent des fantômes bavards.
- Test. Un playtest sans explication : l'objectif est compris en moins d'une minute et le groupe relance une manche sans qu'on le lui demande.

*L'identité esthétique*

Ce qui rend le jeu reconnaissable en une image, sans titre ni logo.

- Critère. Une silhouette, une palette ou un son que personne d'autre n'a. Le low-fi est accepté par le marché (Lethal Company, R.E.P.O.), le générique ne l'est pas. Dans un clip de huit secondes sans contexte, c'est la seule chose qui ramène vers la page Steam.

**6. Filtre A : la clipabilité**

Un clip est une séquence de 15 à 60 secondes découpée d'un stream et rediffusée sur TikTok, Shorts ou Reels.

Mon pari : un jeu qui en produit naturellement fait le travail des streamers à leur place, et pour un studio sans audience ni budget marketing, les streamers sont le seul canal qui peut nous faire connaître à grande échelle : Peak a été lancé avec moins de 200 000 $ de budget. Les onze statements ci-dessous sont tirés des points communs des clips de ces hits. Ce sont des hypothèses à confirmer sur un corpus plus large, et elles rendent le pari vérifiable sur prototype.

Ce qui appuie ce pari

- Peak a conçu sa friction sociale pour produire des moments partageables et a converti ses wishlists 266 fois mieux que la médiane ; son co-créateur parle d'un volume soudain d'images qui a créé la perception d'un événement.
- Schedule I a des animations bouclables, un HUD minimal et un cadrage vertical anticipé ; des chaînes TikTok découpent les VOD des gros streamers, ce que son développeur appelle de la poussière d'or.

Les onze statements

| Statement | Ce que ça veut dire | Comment on le teste |
|---|---|---|
| 1. Unité de temps | Le jeu produit des séquences autonomes de 15 à 60 s avec un début et une fin : une tentative, une manche, une décision. | Découper 30 minutes de playtest : combien de segments se tiennent seuls ? |
| 2. Lisibilité en deux secondes | Un inconnu comprend l'enjeu du moment en deux secondes, par l'image et le son, jamais par le texte. | Dix clips sans explication montrés à trois personnes extérieures : elles disent l'enjeu. |
| 3. Payoff net | Chaque séquence se conclut par un événement non ambigu, visible et audible. | Chaque segment a-t-il un dernier plan évident ? |
| 4. L'échec est le contenu | Échouer est plus drôle ou plus spectaculaire que réussir, et ne coûte qu'une séquence. | Compter la part d'échecs parmi les moments découpés. |
| 5. Variance | Le même setup produit des issues différentes par la physique, l'aléatoire ou les autres joueurs. | Dix clips côte à côte : combien racontent la même chose ? |
| 6. Réaction humaine amplifiée | Le jeu ménage des temps de tension où la face cam ou la voix des joueurs devient le spectacle. | Repérer un silence avant payoff dans chaque séquence. |
| 7. Format vertical | L'information critique tient dans le tiers central et reste lisible en 9:16. Rien d'essentiel dans les coins. | Recadrer cinq clips en vertical : l'enjeu reste visible. |
| 8. Signature en une image | Une silhouette, une palette ou un son reconnaissables en une frame. | Une image fixe au hasard : trois personnes nomment le jeu. |
| 9. Le clip est une publicité | La séquence montre ce que le spectateur ferait lui-même. Pas de twist qui s'épuise en regardant. | Après le clip, la question spontanée est « c'est quoi ce jeu ? », pas « c'est quoi la fin ? ». |
| 10. Titrabilité | Chaque moment se décrit en cinq mots. Sans titre TikTok possible, ce n'est pas un clip. | Le playtesteur titre chaque segment en moins de dix secondes. |
| 11. Capture facilitée (optionnel) | Le jeu aide à sortir le moment : replay, résumé de manche, caméra intégrée. | Combien de clics entre le moment et le fichier partageable ? |

Pourquoi je ne compte pas que sur les clips

- Ils ne convertissent pas seuls et n'arrivent pas sans premier streamer. Balatro a été lancé par 300 petits et moyens streamers, CloverPit a distribué 600 clés tôt : le plan d'amorçage fait partie du design.
- Ils ne remplacent pas la rétention. Les clips font la semaine de lancement ; les histoires font les mois suivants.

**7. Filtre B : l'anecdote factory**

Une anecdote est une histoire que le joueur raconte le lendemain à quelqu'un qui n'a pas joué. C'est mon pari face à la rétention de 3 % en D30 du friendslop, et je le présente comme tel : je n'ai pas de chiffre qui prouve qu'un jeu riche en story auto généré retienne mieux dans notre genre de jeu.

Ce que les données montrent, c'est que les jeux qui en produisent continuent de se vendre par bouche-à-oreille longtemps après leur sortie, là où l'effet des clips s'arrête. Leur point commun : des systèmes indépendants qui se croisent, et un cadre qui donne un enjeu à leurs collisions. Une sandbox sans objectif produit du bruit ; une manche avec un but produit des histoires.

Ce qui appuie ce pari

- Phasmophobia, coop horreur sorti en 2020, a dépassé 22 millions de copies et continue de vendre. Hatchet attribue ces ventes durables au fait que le partage d'histoires est intégré au principe du jeu : chaque partie est différente, et les spectateurs finissent par vouloir jouer.
- RimWorld se joue 242 heures en moyenne et dépasse 300 M$ sept ans après sa sortie, sans clip viral : ses joueurs vendent le jeu en racontant leurs colonies.
- À l'inverse, le narratif court et le metroidvania produisent des succès mais un seul lancement : chaque joueur vit la même histoire, et personne n'a rien à raconter que l'autre ne sache déjà.

Les huit statements

| Statement | Ce que ça veut dire | Comment on le teste |
|---|---|---|
| 1. Causalité lisible | Chaque événement marquant a une cause que les joueurs peuvent reconstituer. Pas de hasard opaque. | Après un moment fort, les joueurs disent pourquoi c'est arrivé : « c'est parce que tu as lâché la caisse ». |
| 2. Attribution | Un acteur identifiable est responsable, en héros ou en coupable. Le jeu nomme et montre qui a fait quoi. | Les histoires racontées ont un sujet nommé. |
| 3. Croisement de systèmes | Les moments mémorables naissent d'au moins deux systèmes indépendants, jamais d'un script. | Lister les systèmes impliqués dans chaque histoire. Si un seul système : c'est un script. |
| 4. Verbes polyvalents | Chaque verbe du joueur a plusieurs usages et plusieurs interactions avec le monde. | Compter les interactions distinctes par verbe, d'un prototype à l'autre. |
| 5. Conséquence durable | L'événement change la suite de la partie. Sans conséquence, c'est un gag, pas une histoire. | L'état du jeu dix minutes après est différent de ce qu'il aurait été sans l'événement. |
| 6. Témoins | L'événement a été vu par un autre joueur, ou le jeu le rend visible par un récapitulatif. | Combien d'histoires ont deux versions concordantes ? |
| 7. Longue queue | Les événements extrêmes sont rares mais possibles. C'est la distribution qui fabrique « la fois où ». | Sur dix parties, un événement qu'aucune autre n'a produit. |
| 8. Racontable sans le jeu | L'histoire tient en trois phrases pour quelqu'un qui n'y joue pas : situation, retournement, chute. | Le test du lendemain, décrit dans la section suivante. |

Les deux filtre se recoupent sur la variance et la titrabilité, mais elles se testent séparément : la première devant des inconnus, la seconde auprès des joueurs eux-mêmes, le lendemain.

**8. Comment valider sur prototype**

Je propose de passer un protocole, la fiche d'audit interactive (https://mathieucabot.github.io/SteamMarketMapping/#valider) du mapping en parle.

**9. Les pièges à éviter**

Six erreurs ont coûté le plus cher à des équipes compétentes ces deux dernières années. Pour chacune, la preuve chiffrée et la règle que je propose que nous nous donnions. Un septième piège me concerne en tant qu'analyste : lire une estimation comme une vente. Quand je cite un chiffre, je dis s'il est sourcé ou estimé.

| Le piège | La preuve | Notre règle |
|---|---|---|
| Le jeu à regarder | Paper Dolls : 5 à 6 millions de vues, 20 000 ventes. GameDiscoverCo range les « boutique indies », qui suscitent l'intérêt sans intention d'achat, parmi les jeux qui convertissent le moins leurs wishlists en ventes. | Chaque clip montre ce que le spectateur ferait lui-même. Coop, variance, prix impulsif. Jamais de twist unique. |
| Lancer dans l'ombre d'un mastodonte | Burglin' Gnomes, top 2 du Next Fest de février 2026, sorti le jour de Meccha Chameleon : étouffé. Dear Passengers a pris 1,5 M de wishlists en cinq jours. | Surveiller les annonces de notre genre de jeu. Décaler de quelques semaines plutôt que de quelques jours. |
| La spirale de population | Marathon moins 96 % en six mois. Texas Chain Saw rebasculé en P2P puis abandonné. Omega Strikers et Superball morts en quelques mois. | Coop hébergé par les joueurs, jouable avec ses propres amis, sans matchmaking ni serveurs. |
| Compter sur le 1.0 | 80 % des jeux gagnent moins au 1.0. Médiane : 40 % du premier mois d'Early Access. Supermarket Simulator : moins 95 %. | L'Early Access est le lancement. Démo, Next Fest, streamers et prix de lancement se jouent là. |
| Le clip sans hook | Pour un Lethal Company, des centaines de jeux conçus pour le stream n'ont jamais été streamés. Le développeur de Vital Shell : « presque aucune réponse des streamers ». | Le hook d'abord, validé par le test des cinq personnes. La clipabilité multiplie, elle ne crée pas. |
| La longue campagne sans momentum | Les sous-convertisseurs ont 411 jours de pré-lancement en moyenne contre 214 pour les meilleurs. Le momentum des deux semaines avant le Next Fest prédit mieux que le total à vie. | Page Steam ouverte 6 à 12 mois avant, 70 % de l'effort sur les quatre derniers mois, un pic avant chaque Next Fest. |

**10. Calendrier et jalons marché**

Je lis le calendrier Steam ainsi : la sortie en Early Access est notre lancement, et quatre portes la précèdent. Les dates dépendent de la fenêtre que nous choisirons ; les seuils des portes, eux, sont fixés par le marché.

[Schéma : feuille de route · cinq phases (Prototype, Vertical slice, Next Fest, Early Access, Post-lancement), quatre portes (hook validé 4 sur 5 et audit des filtres passé ; page Steam ouverte 6 à 12 mois avant ; 7 000 wishlists et 20 % de conversion démo ; avis à 90 % ou plus en semaine 1)]

Chaque seuil vient des données. 7 000 wishlists, c'est le minimum observé pour apparaître dans Popular Upcoming, la liste des sorties attendues de Steam. 20 %, c'est la conversion médiane d'une démo en wishlists. 90 % d'avis positifs, c'est la moyenne des jeux qui convertissent le mieux leurs wishlists en ventes, contre 67 % pour ceux qui convertissent le moins.

Ce que le calendrier Steam impose

- Trois Next Fest par an, fin février, mi-juin, mi-octobre. J'en vise un, avec une base de wishlists et un pic dans les deux semaines précédentes : les jeux qui réunissent les deux réussissent leur Next Fest dans 82 % des cas, alors que le participant médian ne gagne que 200 wishlists.
- La page Steam ouvre 6 à 12 mois avant, et 70 % des wishlists arrivent dans les quatre derniers mois. Une campagne plus longue sous-convertit.
- Début 2027, les Daily Deals universels disparaissent au profit de recommandations personnalisées : un jeu à audience nette y gagne, un jeu générique y perd.

**Sources**

Tous les chiffres de ce document viennent de la Mapping Steam 2026 (https://mathieucabot.github.io/SteamMarketMapping/), étude faite le 4 octobre 2026, où chacun est daté, marqué comme sourcé, estimé ou lecture d'analyste. Les notes de données par genre de jeu et les extractions brutes sont dans le dépôt GitHub (https://github.com/MathieuCABOT/SteamMarketMapping/tree/main/donnees).

Les sources primaires les plus utilisées : Chris Zukowski, How to Market a Game ; Simon Carless, GameDiscoverCo ; Alinea Analytics et Naavik ; Game Developer ; pages Steam, Steambase, SteamCharts, SullyGnome et TwitchTracker, relevés le 4 octobre 2026.

---

# Partie B : le journal complet de la conversation

Les messages de Mathieu sont reproduits mot pour mot, fautes de frappe comprises. Les réponses de Claude sont reproduites dans leur forme finale. Les actions faites entre deux messages (recherches, écriture de fichiers, publications) sont résumées entre crochets.

## Échange 1 : le cadrage initial

**Mathieu :**

> J'ai un projet. Qui est euh, de faire un jeu avec des amis à moi. On a fait un jeu ensemble lors de ma dernière année d'études à Rubika qui avait plutôt bien marché, qui avait été nominé au Pégase dans la catégorie meilleur jeu étudiant (12 Memory Lane). Et on aimerait réitérer l'expérience. Sauf que maintenant, on a tous eu des expériences professionnelles chacun de notre côté. Et réaliser un jeu qui n'a pas seulement pour but d'être original et de servir d'épanouissement créatif, mais aussi de s'insérer dans un marché.
>
> Déjà, niveau cadrage, On sait à peu près mis d'accord sur le fait qu'on voulait faire un jeu Steam. s'est à peu près mis d'accord sur le fait qu'on voulait faire un jeu Steam. On a mis de côté pour le moment Roblox, le mobile et les jeux web. Bien sûr, on n'exclut pas un portage à l'avenir, que ce soit sur Epic Games ou d'autres plateformes. Mais le secteur ciblé, le marché Steam.
>
> et Pour notre approche, on aimerait avoir une approche très pragmatique. Nous sommes trois designers. Et là, nous en sommes à la phase où nous Voulons observer le marché afin de pouvoir situer quel genre de jeu serait susceptible de fonctionner ou pas. Par exemple, on sait qu'un tactical euh, top view, ça marcherait pas trop. Alors que peut-être un jeu de type friend slope est endance en ce moment. J'aimerais que tu joues le rôle d'un game designer senior spécialisé dans le marché Steam Et que tu design une approche à avoir pour avoir une idée globale sur le marché. Nous, ce qu'on s'est dit, c'est que ça serait bien de mettre en relation les tendances de jeu, de jeu sur Steam avec les tendances de vue sur Twitch en fonction du jeu ou même YouTube ou même les recherches Google. Pour avoir un peu une idée des mouvements euh, du marché, des hypes qui se créent, qui se perdent, etc. Mais c'est une vision qui est basée sur mes connaissances actuelles et non celle que j'aurai à la fin de cette étude, entre guillemets. Qu'est-ce que tu en penses ? Est-ce que tu vois ce que je veux dire et est-ce que tu comprends ?

**Claude :**

> Oui, je vois exactement ce que tu veux dire, et je comprends le projet. Je te réponds en tant que GD senior côté marché Steam, en commençant par ce qui me semble juste et ce qui me semble piégeux dans ton intuition de départ, puis je te propose une méthode.
>
> [Claude enregistre le contexte du projet dans sa mémoire persistante.]
>
> **Ce que je comprends de ta demande**
>
> Vous voulez une méthode de veille marché pour répondre à une question précise : « quel genre de jeu, faisable par trois designers, a une demande réelle sur Steam et de la place pour un nouvel entrant ? ». Et ton idée est de triangulariser les signaux Steam avec les signaux d'attention (Twitch, YouTube, Google) pour lire les cycles de hype plutôt qu'une photo figée. Le raisonnement est bon. Mais trois points méritent d'être corrigés avant de construire la méthode.
>
> **Ce qui me semble piégeux dans l'approche initiale**
>
> **Twitch est un très mauvais proxy de ventes pour la plupart des genres.** L'audience Twitch est hyper concentrée sur une poignée de titres, et beaucoup de jeux qui font des millions sur Steam n'y existent quasiment pas (deckbuilders, city builders, puzzle, narratif, automation). À l'inverse, le signal Twitch est pertinent pour une seule famille de jeux : ceux dont la boucle est « streamable » (coop horreur, party games, physique chaotique). Donc Twitch ne doit pas servir à mesurer la demande d'un genre, mais à mesurer une dimension spécifique : le potentiel de viralité par les créateurs. Ce sont deux axes différents dans la grille, pas un seul.
>
> **Une tendance observable est déjà une tendance en voie de saturation.** Entre aujourd'hui et votre sortie, il va s'écouler 18 à 30 mois. La vague « friendslop » a déjà eu plusieurs générations (Lethal Company fin 2023, Content Warning 2024, R.E.P.O. et Peak 2025). Quand un genre est visible sur Twitch, des centaines d'équipes sont déjà en production dessus. La vraie question n'est pas « qu'est-ce qui est hype », mais « quel genre a une demande structurelle supérieure à l'offre, et pourquoi ça va durer ». Il faut donc analyser la position dans le cycle, pas seulement la hauteur de la vague.
>
> **Vos intuitions de départ sont des hypothèses à tester, pas des acquis.** « Tactical top view ça marche pas » est typiquement le genre d'intuition que la donnée contredit souvent : revenu médian plus faible, oui, mais audience fidèle, peu de concurrence de qualité et des réussites régulières de petites équipes (Into the Breach, Tactical Breach Wizards). Et « friendslop est en tendance » est vrai, mais c'est un genre qui exige du netcode, du multijoueur, et une loterie de viralité, soit exactement ce qu'une équipe de trois designers sans programmeur réseau a le plus de mal à maîtriser. Le fit avec vos capacités pèse autant que le fit marché.
>
> **La méthode que je vous propose**
>
> 1. **Contraintes avant marché.** Écrire noir sur blanc : budget, durée de production cible, compétences réelles (qui code, qui fait l'art, quel moteur), temps plein ou soir et week-end. Ça élimine 60 % des genres avant même de regarder une courbe, et ça évite de tomber amoureux d'un marché inaccessible.
> 2. **Cartographie offre/demande par tag Steam.** Pour chaque genre candidat, sur les jeux sortis les 24 derniers mois : nombre de sorties, revenu médian estimé, part des jeux dépassant un seuil de reviews, concentration des revenus sur les hits. Sources : SteamDB, Gamalytic, VG Insights, les rapports par genre de Chris Zukowski (How to Market a Game) et la newsletter GameDiscoverCo de Simon Carless. On cherche les genres à médiane haute et offre faible, pas les genres à gros hits et offre pléthorique.
> 3. **Signaux d'attention, chacun pour ce qu'il mesure.** Twitch (SullyGnome, TwitchTracker) pour la streamabilité. YouTube pour la capacité à générer du contenu long et des tutos, ce qui révèle les genres à forte rejouabilité et communauté. Google Trends et Reddit pour l'intérêt latent et les demandes insatisfaites (« jeu comme X mais avec Y »). Ces trois signaux deviennent des colonnes séparées dans la grille, jamais un indice fusionné.
> 4. **Position dans le cycle de hype.** Pour chaque genre, reconstruire la chronologie sur cinq ans : le hit fondateur, les suiveurs, le moment où la médiane s'effondre. Ça permet de classer en « émergent », « mature mais sain », « saturé » et « ringard avec niche fidèle ». Les deux meilleures positions pour une petite équipe sont souvent la deuxième et la quatrième, pas la première.
> 5. **Grille de scoring croisée.** Dix à quinze genres en lignes, et en colonnes : demande, saturation, streamabilité, scope faisable à trois designers, risque technique, place pour une différenciation, et votre avantage injuste (ce que 12 Memory Lane vous a appris à faire mieux que les autres). Notation honnête, puis débat à trois.
> 6. **Validation terrain avant production.** L'étude de marché ne remplace pas un test de wishlists. Une page Steam avec un pitch et des visuels, un Next Fest avec une démo, et un objectif de wishlists mesurable. C'est le seul signal qui prédit vraiment vos ventes.
>
> **Ma recommandation sur la suite**
>
> Je peux faire les étapes 2 à 4 avec vous de façon concrète : aller chercher les données réelles sur une liste de genres candidats et vous livrer la grille remplie, avec les sources. Pour ça, il me faut deux choses de votre côté : les contraintes de l'étape 1, et une première liste de genres qui vous attirent ou vous intriguent, même si vous pensez qu'ils ne marchent pas. On les traitera tous de la même manière, intuitions comprises.

## Échange 2 : l'équipe complète et l'idée du clipping

**Mathieu :**

> Attention, il y a un pledge. Nous ne sommes pas que trois designers. Il y a des artistes, des programmeurs. C'est juste que c'est nous les designers qui pensons le projet. Je comprends ton point sur la plateforme Twitch. L'un des designers qui travaille avec moi a néanmoins proposé l'idée marketing que pour diffuser le jeu, on compte sur les streamers. Il a une approche intéressante qui consiste à designer un jeu pour qu'il soit naturellement adapté au clipping. Le clipping est une tendance que l'on peut voir sur le web qui consiste à faire des clips de live de streamers et les diffuser sur TikTok, YouTube, instagram, et plein d'autres plateformes. Autrement dit, si un jeu est naturellement pensé pour créer des moments idéaux pour le clipping, la stratégie de diffusion est en partie déjà faite. Eh bien, et bonne idée pour ta notion de la vague, savoir si on est au début, au milieu, à la fin, si c'est en expansion, si c'est stable, comme hype, c'est une bonne notion, je pense. D'un point de vue euh, compétences, il faut savoir qu'on est extrêmement versatile. On a une foulée d'artistes, trois GD, un programmeur, mais on peut en avoir plusieurs si nécessaire. Et si la team est trop grosse pour ce projet, bah, imaginons, on peut très bien se séparer en deux pour faire deux projets à la fois. Donc ne t'occupe pas de ce que le projet a besoin, on sera adapté.

**Claude :**

> Bien noté, je corrige ma mémoire du projet et je te réponds sur le clipping, qui est le vrai sujet de ce message.
>
> [Mise à jour de la mémoire du projet.]
>
> Compris pour l'équipe, j'enlève le filtre « faisabilité » de la méthode. Le filtre principal devient donc le marché et la différenciation. Passons au clipping, parce que l'idée de ton collègue est bonne, mais elle mérite d'être affûtée.
>
> **Mon avis sur « designer pour le clip »**
>
> **C'est une stratégie validée par le marché, pas une théorie.** Lethal Company et Content Warning sont les exemples évidents, mais le phénomène dépasse largement le friendslop. Buckshot Roulette, Balatro, Liar's Bar, Mouthwashing, Thank Goodness You're Here ou Schedule I ont tous explosé via des clips courts, et plusieurs sont solo. Ce qui compte n'est pas le multijoueur, c'est la structure du moment.
>
> **La vraie cible de cette stratégie, c'est le streamer, pas le spectateur.** Un streamer choisit un jeu parce qu'il lui facilite le travail : il lui fournit du contenu, des réactions et des clips sans effort. Un jeu « clip-friendly » est un cadeau fait aux créateurs. Il faut donc penser le design du point de vue de leur métier : que vont-ils pouvoir monter, titrer, et poster dans l'heure ?
>
> **Un bon clip a une grammaire assez stricte.** Quinze à soixante secondes, lisible sans aucun contexte, un enjeu compris en deux secondes, un payoff net (retournement, échec comique, surprise, réaction humaine) et souvent un visage ou une voix qui réagit. En design, ça se traduit par des leviers concrets : états lisibles d'un coup d'œil, moments à forte variance, décisions à timing court, échecs drôles plutôt que punitifs, et une UI qui reste lisible sur un recadrage vertical de téléphone. Ce dernier point est sous-estimé par presque tout le monde.
>
> **Les trois pièges à anticiper**
>
> 1. **Regarder n'est pas acheter.** Certains jeux sont excellents à regarder et mauvais à vendre, parce que le spectateur a épuisé sa curiosité en regardant. C'est le cas de beaucoup de jeux narratifs à choix et de jeux d'horreur à twist unique. Les jeux qui convertissent sont ceux où le spectateur se dit « je veux vivre ça moi-même, ou avec mes potes ». Il faut donc concevoir des moments qui donnent envie de jouer, pas seulement envie de regarder.
> 2. **Le biais du survivant.** Pour un Lethal Company, il y a des centaines de jeux conçus pour le stream que personne n'a jamais streamés. La clipabilité est un multiplicateur, pas un hook. Sans une promesse forte tenant en une phrase, il n'y a rien à multiplier.
> 3. **L'amorçage.** Il faut un premier streamer. Content Warning a eu Landfall et un lancement gratuit 24 h, Lethal Company a eu de la chance pure. Vous, vous aurez besoin d'un plan d'amorçage réaliste : petits et moyens streamers d'horreur ou de coop en manque de nouveautés, Next Fest, démo, clés distribuées tôt. Ça se planifie dès le concept.
>
> **Ce que ça change dans la méthode**
>
> J'ajoute un axe « clipabilité » séparé de l'axe « demande », avec des sous-critères : lisibilité hors contexte, fréquence des moments à payoff, dépendance aux réactions humaines, et surtout le ratio entre audience des clips et ventes réelles. Ce ratio se mesure. On peut prendre une vingtaine de hits récents, relever le volume de vues sur TikTok et Shorts, le comparer au nombre de reviews Steam, et distinguer les « jeux à regarder » des « jeux à acheter ». On peut aussi décortiquer les clips les plus vus de chaque jeu pour en extraire la grammaire : durée, déclencheur, contexte nécessaire, type de payoff. Ça donnerait à vos designers une boîte à outils très concrète plutôt qu'une intuition.
>
> Pour lancer la vraie étude, il me manque encore deux éléments de votre part : votre liste de genres candidats, y compris ceux que vous croyez perdants, et vos contraintes de calendrier et de budget, qui servent à fixer la fenêtre de sortie et donc le moment du cycle de hype que l'on vise.

## Échange 3 : la grammaire du clip en statements

**Mathieu :**

> C'est une bonne idée de définir la grammaire d'un clip et de mettre ça comme des statements de design ? en tout cas garder bien ça en tete et que ça soit bien claire, presque. Par exemple, avoir une expérience, une expérience de 15 à 60 secondes, un payoff net, le contexte du jeu compris en 2sec , echec drole plutot que punitif, UI non handicapante sur un format vericale, et plus encore.
>
> sur Les pièges à éviter, en effet. Regardez, ce n'est pas acheté. Et tu as raison. Il est nécessaire de créer la motivation chez le joueur de vivre ça lui-même plutôt que de le regarder.
>
> trouver Un hook ou une thématique forte est vraiment essentiel. C'est ça qui fera sans doute le succès du jeu. C'est toutes les décisions prises pour la clippabilité qui permettront de faire, d'aider à sa diffusion. Mais son succès dépend évidemment de la core expérience, de l'esthétique indentifiable, etc

**Claude :**

> Oui, c'est une bonne idée, à une condition de forme qui change beaucoup de choses en pratique. Je te propose la formulation ci-dessous, puis je la sauvegarde dans ma mémoire du projet.
>
> **Statements, oui, mais comme une « lentille », pas comme des piliers**
>
> Les piliers de design décrivent l'expérience que vit le joueur. La clipabilité décrit une propriété de diffusion. Si vous mettez le clipping au niveau des piliers, vous finirez par designer un jeu à regarder, ce qui est précisément le piège dont on parlait. Je recommande donc une hiérarchie en deux étages :
>
> - **Étage 1, ce qui fait le succès :** le hook en une phrase, la core experience, l'identité esthétique. Ce sont vos piliers, et chaque feature doit les servir.
> - **Étage 2, ce qui fait la diffusion :** la grammaire du clip, formulée comme une lentille transversale. Chaque feature validée par les piliers est ensuite passée au crible de cette lentille.
>
> Et chaque statement doit être **testable** sur un prototype, pas inspirant. On doit pouvoir filmer trente minutes de playtest et répondre oui ou non.
>
> **La grammaire du clip, en onze statements**
>
> 1. **Unité de temps.** Le jeu produit naturellement des séquences autonomes de 15 à 60 secondes, avec un début et une fin identifiables : une tentative, une manche, une décision.
> 2. **Lisibilité en deux secondes.** Un spectateur qui ne connaît pas le jeu comprend l'enjeu du moment en deux secondes, par l'image et le son seuls, jamais par du texte.
> 3. **Payoff net.** Chaque séquence se conclut par un événement non ambigu, visible et audible : victoire, échec, retournement, révélation.
> 4. **L'échec est le contenu.** Échouer est plus drôle ou plus spectaculaire que réussir, et l'échec ne coûte jamais plus d'une séquence.
> 5. **Variance.** Le même setup produit des issues différentes, par la physique, l'aléatoire ou les autres joueurs. Deux clips du même jeu ne doivent pas se ressembler.
> 6. **La réaction humaine est amplifiée.** Le jeu ménage des temps de tension ou d'attente où la face cam du streamer ou la voix des joueurs devient le spectacle.
> 7. **Format vertical.** Toute information critique tient dans le tiers central de l'écran et reste lisible après recadrage en 9:16. Rien d'essentiel dans les coins ni en petit texte.
> 8. **Signature en une image.** Une silhouette, une palette ou un son reconnaissables en une frame, pour que le jeu soit identifié dans un clip sans titre ni lien.
> 9. **Le clip est une publicité.** La séquence montre ce que le spectateur ferait lui-même. Pas de twist unique dont la curiosité s'épuise en regardant.
> 10. **Titrabilité.** Chaque moment peut se décrire en cinq mots. Si personne ne peut écrire le titre TikTok, ce n'est pas un clip.
> 11. **Capture facilitée.** Le jeu aide à sortir le moment : replay, résumé de fin de manche, photo ou caméra intégrée. C'est le seul statement optionnel.
>
> Le statement 8 relie directement les deux étages : votre identité esthétique est aussi ce qui empêche vos clips d'être anonymes. Et le statement 9 est la traduction en design du piège « regarder n'est pas acheter ».
>
> **Comment on s'en sert**
>
> Deux usages concrets. D'abord, **avant de figer la grammaire**, la vérifier sur le terrain : prendre une vingtaine de hits récents, regarder leurs cent clips les plus vus, et relever durée, déclencheur, contexte nécessaire et type de payoff. Si la réalité contredit un statement, c'est le statement qui bouge. Ensuite, **sur vos prototypes**, un audit de clips régulier : filmer un playtest, le découper, compter combien de moments passent la lentille, et suivre cette densité comme une métrique de production au même titre que le fun.
>
> [Enregistrement de la grammaire du clip dans la mémoire.]
>
> C'est enregistré. Pour résumer où on en est : la méthode d'étude de marché est posée en six étapes, l'équipe n'est plus un filtre, et la clipabilité est désormais une lentille de onze statements testables, subordonnée au hook, à la core experience et à l'identité esthétique.
>
> Pour passer de la méthode à l'étude elle-même, il me manque trois choses de votre côté, indépendantes les unes des autres :
>
> 1. **Votre liste de genres candidats**, y compris ceux que vous pensez perdants, pour que tout le monde soit évalué avec la même grille.
> 2. **Votre fenêtre de sortie et votre budget approximatif**, pour savoir quel moment du cycle de hype on vise.
> 3. **Vos jeux de référence**, une dizaine de titres récents que vous admirez ou qui vous intriguent, pour constituer le corpus de clips à analyser et valider la grammaire.
>
> Dès que j'ai au moins la liste de genres, je peux lancer la collecte des données Steam et des signaux d'attention, et vous livrer la grille remplie avec les sources.

## Échange 4 : la théorie du chaos systémique et le lancement de l'étude

**Mathieu :**

> concernant la liste des genres candidats, je n'en ai pas. Hormis des classiques comme le Friends Slope. Tout ce qui est jeu dont le système permet de créer un chaos systémique avec des gameplays émergents. Par exemple, la capacité à porter des choses peut servir à plein de choses. On peut les jeter, on peut les empiler, on peut... Euh, tout un tas de choses. Et ça crée un chaos systémique avec la porte ouverte pour des gameplays émergents qui permettent potentiellement d'arriver à du contenu unique de chaque partie et chaque partie aura peu, probablement tendance à devenir plus mémorable comme un, une histoire ou un souvenir. Ça, ce n'est qu'une théorie de ma part. Je n'ai pas vérifié si elle était vraie ou non. Et pour les jeux de référence, pareil, je n'en ai pas. Euh, on est très, très, très ouvert.

**Claude :**

> Pas de problème, l'absence de liste est une information en soi : c'est à moi de proposer le périmètre. Je réagis d'abord à ta théorie, puis je lance la collecte de données sur une liste de genres que je construis à partir d'elle, et je vous livre une première grille sourcée.
>
> **Sur ta théorie du chaos systémique.** Elle est largement validée par le marché, sous le nom d'« anecdote factory » : RimWorld, Dwarf Fortress, Deep Rock Galactic, Among Us et Lethal Company vendent tous des histoires que les joueurs se racontent ensuite. Et elle recoupe directement deux statements de la lentille clip, la variance et la titrabilité. Deux nuances pourtant. D'abord, l'émergence n'engendre des histoires que si une structure la cadre : un objectif, une manche, un enjeu. Une sandbox physique sans enjeu produit du bruit, pas des souvenirs. Ensuite, ton exemple précis, porter et jeter des objets avec de la physique, est exactement le cœur de R.E.P.O., Content Warning, Peak, Human Fall Flat et Moving Out. Ce n'est pas une raison de l'écarter, mais c'est la zone la plus encombrée du marché actuel, donc celle où la différenciation devra être la plus nette.
>
> Je lance maintenant la collecte sur quinze genres, répartis en cinq familles plus un lot de données macro. La liste inclut volontairement des genres « témoins » que vous croyez perdants, pour calibrer la grille.
>
> [Claude lance six agents de recherche en parallèle : (1) friendslop, party physique, déduction sociale ; (2) colony sim, sandbox systémique, automation ; (3) survival crafting, extraction, compétitif physique et horreur asymétrique ; (4) roguelite et bullet heaven, deckbuilder et Balatro-likes, job sims ; (5) genres témoins : tactique, narratif court, cozy, metroidvania ; (6) données macro Steam 2025-2026 et clipping.]
>
> Les six collectes tournent en arrière-plan. Je compile la grille dès qu'elles remontent, puis je publie le rapport pour votre équipe.

## Échange 5 : les statements de l'anecdote factory

**Mathieu :**

> C'est cool que tu valides ma théorie et que tu mettes un nom dessus. Anecdote Factory. Est-ce qu'on pourrait la faire rentrer dans les statements ? Comme ça, ça ferait qu'on aurait des statements dédiés à la clippabilité et d'autres statements dédiés à l'anecdote factory. Attention à l'utilisation de tokens, je vois que tes tâches en cours sont très gourmandes.

**Claude :**

> Compris pour les tokens : je laisse finir les six collectes déjà lancées, puisqu'elles sont la matière première de la grille, mais je n'en lance aucune autre et je compilerai le rapport moi-même sans agent supplémentaire.
>
> Oui, l'anecdote factory mérite ses propres statements, et la séparation est même saine : la lentille clip décrit ce que voit un spectateur étranger, la lentille anecdote décrit ce que le joueur raconte le lendemain. Certains critères se recoupent, comme la variance, mais chaque lentille doit rester autonome pour être auditable.
>
> **Lentille B, l'anecdote factory, en huit statements**
>
> 1. **Causalité lisible.** Chaque événement marquant a une cause que les joueurs peuvent reconstituer après coup. Pas de hasard opaque : « c'est parce que tu as lâché la caisse ».
> 2. **Attribution.** Un acteur identifiable est responsable du moment, en héros ou en coupable. Le jeu nomme et montre qui a fait quoi.
> 3. **Croisement de systèmes.** Les moments mémorables naissent de la rencontre d'au moins deux systèmes indépendants, jamais d'un script. Porter plus feu plus physique, pas une cinématique.
> 4. **Verbes polyvalents.** Chaque verbe du joueur a plusieurs usages et plusieurs interactions. Métrique : nombre d'interactions distinctes par verbe.
> 5. **Conséquence durable.** L'événement change la suite de la partie. Une anecdote sans conséquence est un gag, pas une histoire.
> 6. **Témoins.** L'événement a été vu par un autre joueur, ou le jeu le rend visible ensuite par un récapitulatif ou un replay. Une anecdote se raconte à quelqu'un qui peut confirmer.
> 7. **Longue queue.** Les événements extrêmes sont rares mais possibles. C'est la distribution qui fabrique « la fois où ».
> 8. **Racontable sans le jeu.** L'histoire tient en trois phrases pour quelqu'un qui n'y joue pas : situation, retournement, chute.
>
> Le test de terrain est simple et peu coûteux : le lendemain d'un playtest, demander à chaque joueur de raconter une histoire de la partie. On compte le nombre d'histoires distinctes, on vérifie qu'elles passent les statements, et on suit ce chiffre comme métrique de production, au même titre que la densité de clips.
>
> [Mise à jour de la mémoire.] Les deux lentilles sont enregistrées dans ma mémoire du projet. Elles figureront dans le rapport final avec la grille des genres, dès que les collectes en cours remontent.
>
> [Retour de la collecte macro, archivée dans un fichier de travail.] Collecte macro archivée. Trois enseignements qui pèsent déjà sur votre cadrage :
>
> - **Friendslop n'est pas saturé mais « affamé »** selon Chris Zukowski en juillet 2026 : l'audience saute de jeu en jeu, un hit capte la moitié de l'audience puis retombe en quelques mois. GameDiscoverCo note en parallèle que le coop non-friendslop est un marché sous-servi.
> - **Le genre le plus rentable en taux de réussite est le job simulator**, loin devant tout le reste. Les genres témoins que vous pensiez perdants ne sont pas les pires : la stratégie au tour par tour recule, mais le 2D platformer et le point-and-click sont les vrais déserts.
> - **Les clips comptent moins que l'algorithme Steam.** Sur un hit récent, deux Shorts réussis ont rapporté quelques centaines de wishlists, quand la démo et le New & Trending en ont rapporté des dizaines de milliers. La vidéo courte amorce, Steam convertit.
>
> J'attends les cinq collectes par genre pour compiler la grille.

## Échange 6 : le coût en tokens

**Mathieu :**

> Continue, mais il y en a encore pour beaucoup de tokens tu penses ?

**Claude :**

> Oui, il en reste une part significative. Pour te donner un ordre de grandeur :
>
> | Poste | Tokens |
> |---|---|
> | Collecte macro terminée | ~190 000 |
> | Cinq collectes par genre en cours, estimation | 150 000 à 200 000 chacune |
> | Compilation de la grille et du rapport | 30 000 à 50 000 |
>
> Les cinq collectes sont lancées depuis une douzaine de minutes, donc une bonne partie de ce coût est déjà engagée. Les arrêter maintenant perdrait le travail fait sans rien économiser de ce qui est consommé. Je recommande de les laisser finir, et de ne plus rien lancer ensuite : la grille se compilera à partir de ce qui remonte, sans recherche complémentaire. Si une collecte revient trop mince sur un genre, je le signalerai dans le rapport plutôt que de relancer.
>
> J'attends les retours et je compile dès qu'ils sont tous là.

## Échange 7 : ce que collectent les agents

**Mathieu :**

> Tu serais capable de m'expliquer ce que tu collectes, comment tu le collectes, sur quel, euh, plateforme, quel site etc rapidement ?

**Claude :**

> Oui, rapidement.
>
> **Ce que je collecte**, pour chacun des quinze genres : le volume de sorties récentes, le revenu médian estimé, les trois à cinq hits des 24 derniers mois avec leurs avis Steam, prix et taille de studio, la chronologie du cycle de hype sur cinq ans, les pics d'audience Twitch, les cas de clips viraux, les jeux annoncés pour 2026-2027 et les prix pratiqués. Plus un lot de données macro sur Steam : volume total, conversion wishlists vers ventes, Next Fest, évolution des prix, algorithme.
>
> **Comment** : six agents de recherche en parallèle, chacun responsable de trois genres. Ils font des recherches web, ouvrent les pages, extraient les chiffres, et me rendent un rapport structuré où chaque chiffre est daté, sourcé, et marqué « sourcé » ou « estimation ». J'archive ensuite chaque rapport en version condensée pour compiler la grille.
>
> **Sur quels sites**, par famille :
>
> - **Données Steam et estimations de ventes** : SteamDB, Gamalytic, VG Insights, Raijin, SteamPulse, Steambase, SteamCharts, Immutable, pages Steam des jeux.
> - **Analyses marché** : la newsletter GameDiscoverCo de Simon Carless, le blog How to Market a Game de Chris Zukowski, Alinea Analytics, Naavik, Newzoo, Game Developer, Edge.
> - **Audience et streaming** : SullyGnome, TwitchTracker, StreamsCharts, Hatchet, StreamHatchet.
> - **Clips et viralité** : KnowYourMeme, post-mortems GDC, presse spécialisée, Wikipédia pour les chiffres officiels de ventes.
>
> **Deux limites à connaître** : SteamDB, Gamalytic et StreamsCharts bloquent l'accès automatisé, donc les volumes de sorties par tag et par année sont incomplets. Et Google Trends n'est pas récupérable par ces outils. Les agents le signalent plutôt que d'inventer, et le rapport final indiquera les trous.
>
> Trois collectes sur six sont remontées. J'attends les deux dernières, puis je compile.
>
> [Les six collectes remontent et sont archivées. Claude compile un rapport HTML et le publie en artifact Claude.]
>
> Le rapport est publié : Cartographie Steam 2026 (https://claude.ai/artifact/JgMttUuM3T7MM2XzFioFip). Il est privé pour l'instant, vos co-designers ne pourront l'ouvrir qu'une fois partagé depuis le menu Share de la page.
>
> **Ce qu'il contient.** Dix-sept familles de jeux notées sur cinq axes (demande, place, clip, anecdote, risque), triables en cliquant les en-têtes. Une fiche par genre avec les chiffres qui ont pesé, le verdict de position dans le cycle et l'angle qui reste ouvert. Trois zones de conclusion, les deux lentilles de design, la liste de ce qui n'a pas pu être mesuré, et une quarantaine de sources datées.
>
> **Les trois conclusions qui comptent pour vous.**
>
> - **La zone alignée avec vos deux lentilles est le chaos coop systémique à hook lisible**, 2 à 8 joueurs, 10 à 20 $, non-horreur ou horreur hybridée. C'est aussi la zone la plus encombrée, donc la différenciation doit venir du hook, de la structure de manche et du thème, pas du verbe « porter ».
> - **Vos deux intuitions de départ étaient à moitié vraies.** Le tactique a la pire médiane de l'étude mais produit 25 à 33 jeux à plus d'un million par an. Friendslop a une demande affamée qui migre tous les 3 à 9 mois, mais son offre horreur est saturée depuis fin 2024.
> - **Les clips amorcent, Steam convertit.** Aucun des grands hits étudiés n'a été lancé par TikTok seul. Balatro, c'est 300 petits streamers et deux démos ; Schedule I et Peak, ce sont des streamers dont les VOD ont été découpées ensuite. La démo et le Next Fest pèsent dix à cinquante fois plus qu'un Short réussi.
>
> **Deux limites à garder en tête.** Les volumes de sorties par tag et par année manquent pour les genres non témoins, parce que SteamDB et Gamalytic bloquent l'accès automatisé. En revanche l'API publique de Gamalytic a répondu, et le rapport indique comment la réutiliser. Les estimations de ventes fondées sur les avis sous-estiment les hits à bas prix et surestiment les hits chers.
>
> **Coût total de l'étude.** Les six collectes ont consommé environ 1,3 million de tokens, la compilation une fraction de cela. Aucune recherche supplémentaire n'a été lancée après ta remarque.

## Échange 8 : le dépôt Git

**Mathieu :**

> j'ai creer un git ( C:\GitProjects\SteamMarketMapping) tu tu déplacer ce que tu as fait dedans ? ça sera plus facile à partager

**Claude :**

> Oui. Je déplace la session vers ce dossier, l'application y copiera les fichiers à la fin de ce tour.
>
> [La session est rattachée au dossier. Claude copie les notes de données dans `donnees/` et rédige un README.]
>
> C'est fait. La session est maintenant rattachée à `C:\GitProjects\SteamMarketMapping`, et l'application y copie les fichiers de ce tour dès qu'il se termine.
>
> Ce qui sera copié :
>
> - `etude-marche-steam-2026.html`, le rapport complet, qui s'ouvre dans n'importe quel navigateur.
> - `donnees/`, cinq fichiers Markdown avec les notes de données condensées par famille de genres et leurs sources, utiles si vous voulez vérifier ou prolonger un chiffre.
> - `README.md`, qui décrit le contenu, les conventions « sourcé / estimation », les trous de l'étude et les deux lentilles.
>
> Rien n'est encore commité : je ne touche pas à git sans que vous le demandiez. Quand vous voudrez, je peux faire le premier commit, ou vous pouvez le faire vous-même.
>
> Le lien de l'artefact reste dans le README, mais il faudra le partager depuis le menu Share de la page pour que vos co-designers y accèdent. Le fichier HTML dans le dépôt, lui, s'ouvre sans aucun accès.

## Échange 9 : un lien GitHub Pages

**Mathieu :**

> sans le faire pour le moment, est-ce que tu pourrais faire un lien partageable hébergé sur ce Git pour que cela fasse comme une page web si le Git est en public ? Comme ça, j'ai juste à envoyer le lien de mon Git et les gens ont accès aux données. Est-ce que ça pourrait être fait rapidement ? un peut comme ce lien par exemple (https://mathieucabot.github.io/trendwatch/fr/index.html)

**Claude :**

> Oui, et vite : c'est exactement le mécanisme de ton lien trendwatch, GitHub Pages. Le dépôt est déjà poussé sur GitHub sous MathieuCABOT, donc l'adresse serait https://mathieucabot.github.io/SteamMarketMapping/
>
> Ce qu'il faudrait faire, environ cinq minutes de travail de mon côté :
>
> 1. **Rendre le rapport autonome.** Le fichier HTML actuel a été écrit pour l'artefact Claude, qui ajoute lui-même l'enveloppe de page. Pour GitHub Pages il lui faut son doctype, son head avec encodage et viewport, et son body. Je le renomme en `index.html` à la racine pour que l'URL du dépôt suffise.
> 2. **Ajouter un fichier `.nojekyll`** pour que GitHub serve les fichiers tels quels, sans passer par son moteur Jekyll qui transformerait les Markdown de façon imprévisible.
> 3. **Rendre les notes de données lisibles depuis la page.** Deux options : soit un lien vers chaque fichier Markdown sur github.com, qui les affiche proprement, soit une petite page HTML par note. La première est immédiate, la seconde plus jolie.
> 4. **Ranger les fichiers `gl_*.json`.** Ils sont déjà commités à la racine : ce sont les extractions brutes de l'API Gamalytic pour les six genres témoins, 1,8 Mo au total. Je les déplacerais dans `donnees/` et je les décrirais dans le README.
> 5. **Commit et push.**
>
> Une seule étape te revient : activer Pages dans les réglages du dépôt, Settings, Pages, source « Deploy from a branch », branche main, dossier racine. La page est en ligne une à deux minutes après. Sur un compte GitHub gratuit, le dépôt doit être public pour que Pages fonctionne, ce qui correspond à ton intention.
>
> Dis-moi quand tu veux que je lance les cinq étapes.

## Échange 10 : mise en place de GitHub Pages

**Mathieu :**

> Ok, go, vas-y.

**Claude :**

> [Création de `index.html` autonome, `.nojekyll`, déplacement des JSON dans `donnees/`, liens vers les notes, README mis à jour, commit « Publier le rapport en page GitHub Pages » et push.]
>
> Les cinq étapes sont faites et poussées sur `main`. Ce qui a changé dans le dépôt :
>
> - `index.html` remplace l'ancien fichier HTML, avec son enveloppe de page complète, et contient maintenant des liens vers les notes de données.
> - `.nojekyll` est ajouté.
> - Les sept fichiers `gl_*.json` sont rangés dans `donnees/` et décrits dans le README.
> - Le README donne l'adresse de la future page et une note de publication.
>
> Il reste les deux réglages qui sont de ton ressort, sur GitHub :
>
> 1. **Rendre le dépôt public.** Il est privé pour l'instant : l'API publique de GitHub répond 404 dessus.
> 2. **Activer Pages.** Settings, Pages, Source « Deploy from a branch », branche `main`, dossier `/ (root)`, Save.
>
> Une à deux minutes après, le rapport sera en ligne à l'adresse https://mathieucabot.github.io/SteamMarketMapping/

## Échange 11 : refonte du site (premier message, interrompu)

**Mathieu :**

> C'est bon, tout est set up et ça fonctionne. Est-ce que tu pourrais... Déjà remanier le site pour qu'il ne fasse pas écho à des réflexions que je t'ai dites et plutôt qu'il expose les données de manière utile. Mais toi, en tant que designer UX de ce rapport, réfléchis à comment communiquer l'information pour qu'elle soit pertinente, claire et pratique. Attention aussi au biais de motivation. Quand un utilisateur lit quelque chose, il y a des astuces pour le maintenir engagé. Essaye de réfléchir à ça.
> [Message interrompu]

**Claude :**

> Message bien reçu, et tu m'as interrompu, donc je m'arrête avant de toucher au site. Voici comment je lis le brief, dis-moi si tu veux compléter.
>
> **Ce que je changerais, en tant que designer du rapport :**
>
> - **Retirer tout ce qui est le reflet de notre conversation** : les « vos intuitions », les « zone alignée avec vos lentilles », les mentions de l'équipe. Le site devient une ressource neutre que n'importe quel designer ou studio peut lire, où la grille et les données parlent d'elles-mêmes.
> - **Inverser la hiérarchie** : aujourd'hui le texte précède les chiffres. Je mettrais la grille en premier, avec un tri actif et des filtres par position dans le cycle, puis chaque genre dépliable sur place plutôt qu'en fiches à défiler. Le lecteur choisit sa profondeur.
> - **Rendre chaque chiffre actionnable** : une donnée ne vaut que si elle répond à une question. Je reformulerais les fiches autour de questions concrètes (combien ça vend, combien de place, combien ça se regarde, combien ça coûte en temps et en infra) plutôt qu'autour de la méthode.
> - **Sur l'engagement** : un seul grand fait par écran, de la progression visible (sommaire ancré, compteur de genres explorés), des comparaisons côte à côte plutôt que des listes, et un fil conducteur qui pose une question au début et y répond à la fin. Pas de gadgets, mais un rythme.
> - **Sur le biais** : séparer visuellement « chiffre sourcé », « estimation » et « jugement d'analyste », en trois traitements distincts, pour que le lecteur voie d'un coup d'œil ce qui est solide et ce qui est une lecture.
>
> Deux questions courtes avant de commencer, parce qu'elles changent le résultat : le site s'adresse-t-il à votre équipe seulement, ou à un public plus large de développeurs ? Et veux-tu garder les deux lentilles de design dans le site, ou les sortir dans un document interne ?

## Échange 12 : refonte du site (brief complet)

**Mathieu :**

> C'est bon, tout est set up et ça fonctionne. Est-ce que tu pourrais... Déjà remanier le site pour qu'il ne fasse pas écho à des réflexions que je t'ai dites et plutôt qu'il expose les données de manière utile. Mais toi, en tant que designer UX de ce rapport, réfléchis à comment communiquer l'information pour qu'elle soit pertinente, claire et pratique. Attention aussi au biais de motivation. Quand un utilisateur lit quelque chose, il y a des astuces pour le maintenir engagé. Essaye de réfléchir à ça. Le but est, est que je puisse partager ce lien pour que les informations que j'ai je puisse les transmettre aux autres membres de la team. Faire une partie sur les pièges à éviter. Faire toute une partie également sur la clippabilité. les statements, etc. comment ocnfirmer qu'on prototype les valide ou non. Essaye d'être assez clair sur un peu tout. Pense bien l'architecture et la manière dont tu présentes les choses pour que cela soit clair, intuitif, agréable à suivre et à lire. Et pertinent.

**Claude :**

> [Réécriture complète de `index.html`, vérification dans le navigateur intégré, commit « Refondre le rapport en document d'équipe » et push.]
>
> Le site est refondu et poussé. GitHub Pages le redéploie en une à deux minutes à la même adresse.
>
> **L'architecture, en neuf sections.** Le rapport s'ouvre sur une question, « où un jeu Steam premium a-t-il de la place en 2027-2028, et comment le concevoir pour qu'il se diffuse ? », et chaque section y répond à un niveau de profondeur croissant :
>
> 1. **La réponse en une page.** Six faits chiffrés et la carte des trois zones. Un lecteur pressé s'arrête là.
> 2. **Le marché en 2026.** Dix indicateurs avec, pour chacun, ce qu'il implique concrètement, puis les trois mécanismes de visibilité qui changent d'ici 2027.
> 3. **Dix-sept familles de jeux.** La grille se construit à partir des fiches, se trie, se filtre par position dans le cycle, et chaque ligne ouvre une fiche dépliable : repères chiffrés, cycle, ce qui marche, ce qui échoue, angle ouvert.
> 4. **Idées reçues et données.** Sept phrases que l'on entend partout, confrontées aux chiffres en trois lignes, sans référence à qui les a dites.
> 5. **Dix pièges documentés.** Chacun avec son signal, un échec récent chiffré et sa parade.
> 6. **Clipabilité.** Ce que les hits ont fait concrètement, l'anatomie d'un clip selon le genre, puis les onze statements avec pour chacun un test et un exemple.
> 7. **Anecdote factory.** Même structure, huit statements.
> 8. **Valider sur prototype.** Un protocole en cinq étapes avec des cibles chiffrées, et une fiche d'audit interactive qui se mémorise dans le navigateur et copie un bilan texte.
> 9. **Méthode, limites, sources.** Replié par défaut.
>
> **Les choix pour tenir le lecteur.** Une barre de progression et une navigation collante donnent une position à tout moment. Chaque section se termine par un « À retenir » de trois lignes. Les chiffres sont isolés en gros caractères avec leur explication dessous, jamais noyés dans une phrase. Les fiches de genre sont fermées par défaut, donc la page reste courte au premier regard et s'approfondit à la demande. Les idées reçues sont présentées en face-à-face, ce qui crée une petite tension à résoudre à chaque ligne.
>
> **Contre le biais de lecture.** Chaque chiffre porte un marqueur visible : S pour sourcé, E pour estimation, J pour lecture d'analyste. La légende est en tête de page, et la section Méthode rappelle que les estimateurs sous-estiment les jeux à bas prix et surestiment les jeux chers. Les notes de la grille sont explicitement présentées comme une aide de lecture, pas un classement.
>
> **Vérifié avant de pousser.** Rendu en sombre sans erreur console, grille construite avec ses dix-sept lignes, filtres et fiches fonctionnels. Je n'ai pas pu vérifier le mode clair ni le format téléphone dans l'aperçu, donc un coup d'œil sur mobile de votre côté vaut la peine.

## Échange 13 : l'esthétique « Finari »

**Mathieu :**

> Est-ce que tu pourrais donner l'esthétique du site Finari à ce là ?

**Claude :**

> Je ne trouve pas de site qui s'appelle « Finari » tel quel. Le plus proche est Finary, la fintech française (finary.com), dont l'esthétique est reconnaissable : fond sombre profond, accents dorés, typographie fine, cartes aux bords subtils, aspect « premium ».
>
> Avant de refaire toute la direction artistique, j'ai besoin de savoir de quoi tu parles exactement :
>
> - **Finary**, finary.com ?
> - Un autre site ou projet qui s'appelle Finari ? Dans ce cas colle-moi le lien, ou une capture, et je m'en inspire directement.
>
> Dès que j'ai la référence, je refais le système de couleurs, la typographie et le traitement des cartes pour coller à cette esthétique, sans toucher au contenu ni à l'architecture.

## Échange 14 : style Finary appliqué

**Mathieu :**

> Oui, Finary, finary.com

**Claude :**

> [Claude relève les couleurs et polices de finary.com dans le navigateur, réécrit la feuille de style, vérifie le rendu, commit « Adopter une direction visuelle inspirée de Finary » et push.]
>
> C'est poussé. La page se redéploie en une à deux minutes à la même adresse.
>
> **Ce que j'ai repris de Finary**, relevé directement sur leur site :
>
> - **Un thème sombre unique.** Fond quasi noir, texte blanc, texte secondaire gris acier, plus de mode clair : la page assume une seule ambiance, comme la référence.
> - **L'or comme seul accent.** Points de la grille, marqueurs de section, filtres actifs, boutons et la phrase clé de l'en-tête en dégradé doré. Un halo lumineux doré derrière le titre et derrière la fiche d'audit, le motif le plus reconnaissable de leur page d'accueil.
> - **Les cartes.** Bords translucides à 8 % de blanc, coins arrondis à 16 px, léger éclaircissement au survol et à l'ouverture.
> - **Les pilules.** Chips de position, filtres, boutons d'audit et marqueurs de fiabilité sont tous en capsule.
> - **La typographie.** Finary utilise PP Telegraf et PP Neue Montreal, deux polices payantes absentes de Google Fonts. J'ai pris Space Grotesk pour les titres, la plus proche géométriquement, et Inter pour le corps, que Finary utilise aussi. Les grands chiffres sont en graisse légère, comme leurs montants de patrimoine.
>
> Les couleurs sémantiques ont bougé pour ne pas se confondre avec l'or : le vert reste pour « émergent » et les chiffres sourcés, le rouge pour « saturé », le lavande pour « niche », et « mixte » passe en bleu acier.
>
> Contenu, architecture et interactions sont inchangés. Vérifié en local sans erreur console, grille et fiches fonctionnelles.

## Échange 15 : modifier un Google Doc ?

**Mathieu :**

> est-ce que tu as la possibilité écrire et medifier ce document ? https://docs.google.com/document/d/1cIbzovjsyNq7o3y3wkz5uzl7YPIaFEjTuI_VeeBJv6M/edit?usp=sharing

**Claude :**

> Oui pour lire, non pour écrire dedans. J'ai bien accès au document : il s'appelle « design od », il est quasiment vide (créé aujourd'hui, 1 Ko) et appartient à ton compte Gmail perso.
>
> Ce que le connecteur Google Drive de cette session me permet :
>
> - **Lire** le contenu complet d'un Google Doc, commentaires compris.
> - **Créer** un nouveau Google Doc avec le contenu que je rédige, dans le dossier de ton choix.
> - **Renommer ou déplacer** un fichier existant.
>
> Ce qu'il ne permet pas : **modifier le corps d'un document existant**. Je ne peux donc pas écrire directement dans « design od ».
>
> Deux façons de contourner, selon ce que tu veux mettre dedans :
>
> 1. **Je crée un nouveau Google Doc** avec le contenu, par exemple le cadre de design du projet (piliers, les deux lentilles, le protocole de validation, la synthèse des zones). Tu le partages ou tu copies son contenu dans « design od » en un copier-coller.
> 2. **Je te rédige le contenu en Markdown dans le dépôt**, et tu le colles dans le Doc toi-même.
>
> Dis-moi ce que tu voulais y mettre, et laquelle des deux voies tu préfères.

## Échange 16 : modifier un document après création ?

**Mathieu :**

> Si tu crées un document Google Doc, est-ce que tu es capable d'écrire dedans ? D'après ce que tu me dis, oui. Mais est-ce que tu es capable de le modifier ensuite ?

**Claude :**

> Non. Un document que je crée se retrouve dans la même situation qu'un document existant : je peux le lire, le renommer ou le déplacer, mais pas en modifier le contenu une fois créé. L'écriture ne se fait qu'au moment de la création, en un seul envoi.
>
> Concrètement, si tu veux itérer sur un texte avec moi dans Google Docs, chaque version serait un nouveau document, ce qui devient vite pénible.
>
> Trois alternatives selon ton besoin :
>
> - **Un document Claude.** Je peux créer un document éditable et partageable chez Claude, que je modifie autant de fois que nécessaire par la suite, et que tu peux exporter en Google Docs, Word ou PDF quand il est stabilisé.
> - **Un fichier Markdown dans le dépôt GitHub.** Je le modifie à volonté, chaque version est commitée, et GitHub l'affiche proprement. C'est cohérent avec le reste du projet, et tes co-designers y ont déjà accès.
> - **Google Docs en lecture seule pour moi.** Tu écris dans le Doc, je le lis quand tu veux un retour, et je te réponds ici. Ça marche si c'est toi qui tiens la plume.
>
> Si l'objectif est le document de design du projet, je recommande le fichier Markdown dans le dépôt : même lien à partager, historique des versions, et je peux le relire face aux données du rapport à chaque modification.

## Échange 17 : option 1 (premier message, interrompu)

**Mathieu :**

> faisont l'option 1.
> [Message interrompu]

**Claude :**

> Tu m'as interrompu, donc j'attends avant de créer le document. Pour partir sur de bonnes bases, dis-moi ce qu'il doit contenir au départ.
>
> Ma proposition, si c'est le document de design du projet : le hook et les piliers à remplir, la synthèse des zones de marché, les deux lentilles avec leurs statements, le protocole de validation, et un journal des audits de prototypes. Je peux aussi partir d'un plan vide avec les titres seulement, que l'on remplit ensemble ensuite.

## Échange 18 : le document de cadrage

**Mathieu :**

> faisont l'option 1.
>
> Ok, maintenant, ça serait bien d'écrire un document synthétique qui permette un peu de cadrer la production au vu de l'analyse que l'on a faite du marché, des piliers euh, de design, des statements, etc. Cadrer un petit peu quel secteur est une opportunité, lesquels ne le sont pas. Point de vue analyse de la clipabilité. et de l'anecdote factory. En gros, faire un document un petit peu que l'on pourrait tous lire en design pour un peu cadrer ce que l'on va faire avec des arguments pour chaque point presque. Le but, c'est d'être clair, que ça soit bien écrit, que ça donne envie de continuer de lire, agréable à lire.
>
> hessiter pas a me questionner si tu as la moidre questino. fait un documment destiner à google docs dans le style de notion

**Claude :**

> Compris : option 1, un document Claude que je pourrai modifier ensuite et que tu exporteras vers Google Docs. Je crée d'abord le squelette, puis je remplis section par section. Je pars sur quelques choix que je te signale : voix « nous », une recommandation argumentée plutôt qu'un menu d'options, et les décisions qui restent à prendre listées en fin de document.
>
> [Création du Claude Doc « Cadrage du projet Steam » en douze sections, avec deux schémas dessinés (carte des familles sur deux axes, feuille de route à quatre portes), et un commentaire laissé sur le choix du thème : « J'ai exclu l'horreur pure du périmètre et gardé seulement l'horreur hybridée : vous confirmez, ou vous préférez la garder comme piste à part entière ? »]
>
> Cadrage du projet Steam (https://claude.ai/code/artifact/27523ffd-ceec-4d2e-9591-5c13cefe09f8) est prêt : relis-le, modifie-le en place, ou laisse des commentaires et je révise.

## Échange 19 : les termes non définis

**Mathieu :**

> attiention des fois tu utlise des terme qui ne sont pas introduit avant comme "L'anecdote factory est notre réponse à la rétention."  "coop à physique" etc

**Claude :**

> Bien vu. Je corrige les termes utilisés avant d'être définis : friendslop, anecdote factory, clip, Shorts, New & Trending, Next Fest, Popular Upcoming et le chaos coop systémique reçoivent une définition à leur première apparition.
>
> [Neuf remplacements dans le document.]
>
> Corrigé dans le document : huit passages définissent désormais leur terme à la première apparition. Friendslop est présenté dès le tableau de la section 2, l'anecdote factory n'est plus citée avant la section 7, et clip, Shorts, New & Trending, Next Fest, Popular Upcoming et chaos coop systémique ont chacun une glose en quelques mots.
>
> Si tu en repères d'autres en relisant, signale-les en commentaire au fil du texte et je les traiterai de la même façon.

## Échange 20 : trop long, et une posture à revoir

**Mathieu :**

> ok. bon c'est un poile trop long à lire quand meme. et au niveau de la posture, le document dit "On fait ça car c'est mieux", il faudrait qu'il plutot qu'il présent un résonnement pour convaincre les lecteurs que c'est ça qu'il faut faire. je ne suis pas le désideur seul pour ce projet, la le but est de présenter mon raisonnement

**Claude :**

> Compris : moins long, et une posture d'argumentation à la première personne plutôt qu'une décision annoncée.
>
> [Réécriture section par section.]
>
> Le document est resserré et reformulé. Ce qui a changé :
>
> - **La posture.** Un chapeau sous le titre annonce un raisonnement à discuter, pas une décision. Les titres de section suivent : « Ce que j'ai retenu du marché », « Ma lecture de la carte », « Ce que je propose », « Ce que je vous demande de trancher ». Le texte dit « je propose », « mon pari », « ce qui me fait viser », et signale à chaque étape où l'argument peut être attaqué.
> - **La longueur.** L'ancienne première section est remplacée par trois temps du raisonnement en six lignes. Les listes « où nous allons » et « où nous n'allons pas » passent de huit à six puces regroupées, les exclusions de cinq à trois, les piliers perdent leur paragraphe redondant et une puce sur trois, les deux grilles gardent leurs tableaux mais perdent un tiers du texte autour, le protocole tient en cinq items compacts, le calendrier en trois puces.
> - **Ce qui n'a pas bougé.** Les deux schémas, les tableaux des statements, le tableau des pièges et la liste de décisions, qui sont la substance.
>
> Le commentaire sur le choix du thème reste en place dans la section « Ce que je propose ». Relis quand tu veux et annote directement dans le document.

## Échange 21 : des raisonnements à expliciter

**Mathieu :** (avec une capture de la première ligne du tableau des constats : « Le volume écrase | 20 282 sorties en 2025, 66 à 70 par jour en 2026. 2,99 % dépassent 1 000 avis. | La visibilité est la ressource rare. Un hook compréhensible en une phrase n'est pas un plus, c'est le ticket d'entrée. »)

> t'es raisonnement logique sous pas evidement, atttention àa ce que tes raisonnement soit expliquer, convainquant et avec pas ou peu de faille

**Claude :**

> Tu as raison, plusieurs déductions sautent une étape. Exemple sur cette ligne : rien n'explique *pourquoi* le volume de sorties rend un concept d'une phrase indispensable. Il manque le mécanisme : les canaux qui amènent les joueurs ne donnent que quelques secondes à chaque jeu.
>
> J'ai relu tout le document avec ce regard. J'y trouve des sauts du même genre, et aussi de vraies failles :
>
> - **Un raisonnement circulaire.** La carte classe les genres selon nos propres grilles, puis conclut qu'il faut aller là où elles sont satisfaites.
> - **Une contradiction.** Le document cite le taux de 34,7 % des job sims alors que la cartographie classe ce chiffre parmi les pièges.
> - **Un seuil d'avis mal sourcé**, et une baisse de joueurs simultanés présentée comme un échec commercial. Liar's Bar est pourtant rentable.
>
> Je réécris chaque argument sur le même modèle : constat chiffré, mécanisme, déduction, limite.
>
> [Réécriture des sections 1 à 4, des piliers, des deux grilles et du calendrier ; mise à jour du titre et de l'axe vertical de la carte.]
>
> J'ai réécrit les arguments du document pour que chaque déduction soit expliquée, et j'ai corrigé les failles que j'ai trouvées en le relisant.
>
> **La méthode.** Chaque constat de la section 2 suit maintenant le même chemin, annoncé dès la section 1 :
>
> - **Le constat**, avec son chiffre.
> - **Pourquoi**, le mécanisme qui explique le chiffre.
> - **Donc**, ce que j'en déduis.
> - **Limite**, l'endroit où l'argument peut céder.
>
> **La ligne de ta capture.** Elle explique maintenant le lien entre le volume de sorties et le concept d'une phrase. L'algorithme de Steam, un ami ou un streamer ne donnent que quelques secondes à chaque jeu. Bō le prouve : 84 % d'avis positifs, 31 700 copies. La limite est assumée : RimWorld a réussi sans concept d'une phrase, mais par une route plus lente.
>
> **Les failles corrigées :**
>
> - **Le raisonnement circulaire de la carte.** L'axe vertical ne mesure plus « l'alignement avec nos grilles ». Il mesure la capacité d'un jeu à se faire découvrir et à durer sans budget marketing, ce qui découle des constats de la section 2.
> - **La contradiction sur les job sims.** Le taux de 34,7 % a disparu. L'argument repose maintenant sur une autre donnée : un seul jeu « Simulator » solo sur 38 a dépassé 70 000 $ en août 2025.
> - **Un critère de rejet faux.** Une baisse de joueurs n'est pas un échec commercial : Liar's Bar est rentable. Le vrai critère contre l'extraction ou l'horreur asymétrique est qu'il faut des inconnus en ligne pour y jouer.
> - **Le prix.** Le seul chiffre du « segment sans top-seller » ne tenait pas. L'argument devient le mécanisme du coop : quatre amis paient le prix quatre fois.
> - **Le seuil d'avis à 90 %.** Il était mal sourcé. Il est maintenant ancré sur une donnée vérifiable : les jeux qui convertissent le mieux leurs wishlists ont 91 % d'avis positifs en moyenne, contre 67 % pour les moins bons.
> - **Les paris présentés comme des faits.** Deux affirmations sont désormais présentées comme des paris, avec la limite de leurs preuves. Les histoires améliorent-elles la rétention ? Les clips pèsent-ils vraiment ?
> - **Un slogan inventé.** Une phrase entre guillemets attribuée à Peak a été retirée.
>
> Ton commentaire sur le choix du thème est toujours ouvert dans la section « Ce que je propose ».

## Échange 22 : export vers Google Docs

**Mathieu :**

> exporte-le en Google Docs

**Claude :**

> [Essai d'export HTML par le connecteur : les schémas sont remplacés par leur légende.]
>
> Je ne peux pas faire cette copie proprement moi-même. La voie fiable est un clic de ton côté.
>
> **Le chemin dans l'app :**
>
> 1. Ouvre le document.
> 2. Clique sur son nom, en haut de la page.
> 3. Choisis **Export**, puis **Google Docs**.
>
> L'app crée alors une copie dans ton Google Drive. Sur mobile, Export se trouve sous Share.
>
> **Pourquoi je ne le fais pas moi-même.** J'ai essayé par mon connecteur Google Drive en exportant le document en HTML, et le résultat est dégradé :
>
> - Les deux schémas, la carte des familles et la feuille de route, sont remplacés par leur seule légende.
> - Ta mention d'auteur sous le titre apparaît comme un identifiant technique.
>
> Une fois dans Google Docs, la copie vit sa vie et je ne pourrai plus la modifier. Pour itérer encore, mieux vaut continuer dans le document Claude et réexporter quand il est stabilisé. Si tu préfères malgré tout une version texte sans les schémas déposée directement dans ton Drive, je peux la créer.

## Échange 23 : des liens cliquables

**Mathieu :**

> tu dis constament section 2, constat 3, etc mais tu pourrais faire des liens clicable pour que ça soit plus claire ? je sais pas si tu vois ce que je veux dire

**Claude :**

> Oui, je vois très bien : chaque renvoi devient un lien qui saute directement à la bonne partie du document. Il y a aussi un problème en amont : les titres ne portent pas de numéro, donc « section 7 » ne correspond à rien de visible. Je numérote les titres, puis je transforme chaque renvoi en lien.
>
> [Numérotation des onze titres, puis 27 liens internes.]
>
> Tous les renvois du document sont maintenant des liens cliquables : 27 au total. Un clic sur « constat 3 » ou « section 7 » fait défiler la page jusqu'au bon endroit.
>
> **Ce que j'ai modifié :**
>
> - **Les onze titres de section sont numérotés.** Avant, « section 7 » ne correspondait à aucun numéro visible. Les sous-titres des cinq constats étaient déjà numérotés.
> - **Tous les renvois pointent vers leur cible** : sections, constats, et le « sixième fait » sur le passage à la version 1.0. Les formules « sections suivantes » et « section suivante » sont aussi liées.
> - **J'ai ajusté deux titres au passage**, pour qu'ils suivent la posture « je propose » : la section 8 devient « Comment valider sur prototype », la section 9 « Les pièges à éviter ».
>
> Je n'ai pas pu vérifier que ces liens survivent à l'export vers Google Docs. Ils pointent vers des endroits précis de la page Claude, et Google Docs pourrait ne pas les reconnaître. Teste un ou deux liens dans la copie après l'export.

## Échange 24 : des images des jeux

**Mathieu :**

> et est ce que tu pourrais ajouter des imagepar mooment ?  de contexte par Example quand tu parle de jeu existant mettre leur icone ou une image leurs ocrrespondant etc. pour aéré la lecteur et aider à voire de quoi on parle à chaque fois

**Claude :**

> [Vérification de seize identifiants Steam, téléchargement des vignettes officielles, composition de sept bandeaux, téléversement et insertion dans le document.]
>
> J'ai ajouté sept bandeaux d'images dans le document, aux endroits où le texte cite plusieurs jeux à la fois. Je n'ai pas pu afficher le rendu final de mon côté : jette un œil pour vérifier la mise en page.
>
> | Emplacement | Jeux montrés |
> |---|---|
> | Constat 1, être découvert | Bō, RimWorld |
> | Constat 2, le coop vend en groupe | Schedule I, R.E.P.O., PEAK |
> | Constat 3, la demande migre | Lethal Company, R.E.P.O., Meccha Chameleon |
> | Constat 4, la vidéo courte | Balatro, How Many Dudes? |
> | Section 3, ce que je vise | Schedule I, Abiotic Factor, Chained Together, RV There Yet? |
> | Section 3, ce que j'écarte | Marathon, Texas Chain Saw, Liar's Bar |
> | Lentille B, les histoires | Phasmophobia, RimWorld |
>
> **Comment ils sont faits :**
>
> - **Les images sont les vignettes officielles des pages Steam.** J'ai vérifié chaque identifiant auprès de la boutique Steam pour que l'image corresponde bien au jeu nommé.
> - **Le nom du jeu est écrit sur chaque vignette**, dans une bande sombre lisible en thème clair comme sombre.
> - **Pour Lethal Company, R.E.P.O. et Meccha Chameleon, l'année figure aussi** : le bandeau montre ainsi la succession des leaders.
> - **J'ai choisi des bandeaux plutôt qu'une image à chaque nom** pour aérer sans encombrer. Les mentions isolées, comme Factorio ou Slay the Spire 2, restent en texte.
>
> Ces visuels appartiennent aux éditeurs des jeux. Ils conviennent à un document interne d'équipe, mais il vaudrait mieux les retirer si le document devenait public.

## Échange 25 : la version envoyée à l'équipe

**Mathieu :**

> voici le document que j'ai envoyer aux autres designer https://docs.google.com/document/d/1uvjEewOmD68vPNjaWXbgCSaJJKhGs6jSPLViLabZTn4/edit?usp=sharing

> Réessayer

**Claude :**

> [Lecture du Google Doc par le connecteur.]
>
> J'ai relu la version que tu as envoyée à l'équipe. Le contenu est complet et tes retouches tiennent. Deux points sont à corriger en priorité :
>
> - **Un renvoi est cassé.** Le tableau de la section 7 dit que le test du lendemain est « décrit dans la section suivante ». Or ta section 8 ne le décrit plus.
> - **Les liens internes n'ont pas survécu à l'export.** « Section 2 », « constat 3 », etc. sont redevenus du texte simple. Google Docs sait faire ces liens nativement : sélectionne le mot, puis Insérer un lien, puis Titres. Les liens vers le site et vers GitHub, eux, fonctionnent.
>
> Je n'ai lu le document qu'en texte, donc je ne vois pas les images. Sa taille, 4,4 Mo, laisse penser que les vignettes sont bien présentes. Vérifie surtout les deux schémas, la carte et la feuille de route.
>
> **Coquilles introduites par les retouches.** La plupart viennent du remplacement de « familles » par « genres de jeux », et de « lentilles » par « filtres ». [Tableau des corrections reproduit en partie A5.]
>
> **Incohérences plus légères :**
>
> - La section 1 parle encore de « deux grilles de design », alors que les sections 6 et 7 s'appellent maintenant « Filtre A » et « Filtre B ».
> - La légende de la carte dit toujours « alignement clip + anecdote ». L'axe vertical s'appelle désormais « Se faire découvrir et durer ».
> - Le test du hook n'a plus de seuil de réussite. La phrase « si quatre personnes sur cinq décrivent la même chose, il tient » a disparu.
> - « Physique based » apparaît deux fois. Si ce n'est pas un terme d'équipe assumé, « à physique » suffit.
>
> Pour les corrections du tableau, la fonction Rechercher et remplacer de Google Docs, avec Ctrl + H, règle les cas répétés en une fois.
>
> Je ne peux pas modifier un Google Doc avec mon connecteur. Le document Claude, lui, n'intègre pas tes retouches. Désormais, c'est la version Google Docs qui fait foi.

## Échange 26 : ce fichier

**Mathieu :**

> Dans le repository, crée-moi un fichier avec l'intégralité de cette conversation écrite dedans et tout le contexte nécessaire pour que cela puisse être repris dans une nouvelle conversation.

**Claude :**

> [Création de ce fichier, `REPRISE-CONVERSATION.md`, à la racine du dépôt, sans commit.]
