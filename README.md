# Modele-de-transcription-pour-ecriture-manuscrite-XVe
Modèle de transcription pour ecriture manuscrite XVe issu du projet TMD (Tours municipal Data, 2026). 
I. Description du corpus

Extraits des délibérations du corps de ville de Tours, pour la période 1511- 1520:

-	Archives municipales de Tours, BB, reg. 14 (FRAC037261_BBR_014), f.  (images) ;

Le corpus sélectionné entre dans la catégorie des documents d’archives antérieurs a 1600, c’est-à-dire avec une écriture très peu normalisée, avec de nombreuses abréviations polysémiques, et une paléographie ancienne, parfois complexe (gothique cursive). 
Il s’agit plus particulièrement ici des délibérations du corps de ville de Tours, ensemble de textes qui présentent, pour une succession de dates rapprochées (1511-1512), les noms des personnes présentes aux assemblées, les sujets  de discussion, les débats et les décisions qui sont prises. 
Construit par séance d’assemblées municipales, le document n’est pas plus précisément structuré de manière uniforme, même si se met en place progressivement une sorte de présentation (date, direction et lieu/ noms des présents suivant un certain ordre (religieux puis laïcs), puis ordre du jour, présentation des avis de tous les présents et relevé de décision) . 
La série documentaire va  dans son ensemble de 1407 à 1789, est construite en volumes qui peuvent avoir une ou plusieurs mains.  
Le sous corpus choisi ici relève d’une même main, celui d’un des clercs de la municipalité de Tours. On peut penser qu’il s’agit d’une remise au propre de notes prises en conseil municipal, même si les quelques rayures et corrections, si l’énumération linéaire des avis montrent que leur enregistrement a pu se faire directement au cours du conseil municipal. 
La main est assez stable sur la centaine de pages sélectionnée. Les pages d’une autre main ont été enlevé du corpus pour réaliser l’entrainement automatique.

II. Projet TMD 

Le projet Tours Municipal Data (TMD) — Transcrire l’écrit délibératif municipal vise à réaliser la transcription et la publication numérique en XML-TEI des manuscrits d’archives liés à la délibération municipale de la ville de Tours pour les XVe et XVIe siècles. L’édition de ce riche corpus de registres de délibérations et de pièces associées (6000 folios manuscrits environ) permet d’en faciliter l’exploration par les chercheurs (recherches plein texte, index nominun, index locorum, index rerum). Leur analyse met en relief les grandes évolutions de l’écrit municipal, des modalités de la prise de décision à différentes périodes institutionnelles de la cité (assemblée d’habitants avant 1462, municipalité ensuite, période de conflits religieux enfin), alors que celle-ci est au cœur du royaume de France. 
C’est dans le cadre de celui-ci, et dans la perspective de mener des campagnes supplémentaires de transcription/édition, que ce  corpus de documents a été sélectionné pour mener à bien des opérations HTR (plateforme eScriptorium) et au développement d’un modèle de transcription. Ces travaux sont très liés au cluster 3 de Biblissima+.
L’objectif de TMD reste cependant l’édition diplomatique de ces documents, et dépasse donc la simple mise en ligne de transcriptions issues d’un modèle de HTR. 

III. Vérité de terrain

Toutes les transcriptions ont été corrigées manuellement afin d’établir la vérité de terrain (ground truth).

IV. Modèles de transcription

La transcription des registres de délibérations du corps de ville de Tours a été réalisée en deux étapes. Une première transcription automatique a été produite à l’aide de CATMuS Medieval 1.6.0 (https://zenodo.org/records/15030337), puis corrigée manuellement afin de constituer une vérité de terrain (ground truth), laquelle a ensuite été utilisée pour entrainer un nouveau modèle de transcription, intitulé : TMD_XVI_14.mlmodel.

V. Logiciel utilisé

La logiciel libre eScriptorium (https://escriptorium.inria.fr), en interface avec le moteur de reconnaissance automatique des écritures manuscrites Kraken, a été utilisé pour l’établissement de la vérité de terrain.
 
VI. Guide de transcription (normes d’établissement de la vérité de terrain)

L’entraînement d’un modèle HTR repose sur l’établissement préalable d’une vérité de terrain, constituée à partir de la transcription d’un témoin selon des normes strictes. À cet égard, TMD adopte une approche dite graphémique, consistant à représenter la valeur de chaque signe au sein de son système d’écriture, au détriment de ses réalisations allographiques.

La transcription est établie de manière ultra-diplomatique, en respectant la graphie et la ponctuation historiques. La capitalisation des lettres majuscules suit l’usage historique, mais peut toutefois être normalisée en cas d’ambiguïté. Les chiffres romains sont normalisés et capitalisés, et les signes de renvois tels que les astérisques « * », croisillons « # » ou obèles « † », sont conservés et restitués à leur place dans le texte.

Les ambiguïtés allographiques contextuelles sont résolues afin de restituer la valeur graphémique des signes. En revanche, les lettres ramistes « u/v » et « i/j » ne sont pas normalisées et sont systématiquement transcrites par « u » et « i » respectivement.

Les signes de ponctuation historiques autorisés sont le point bas « . », employé sans espace avant le signe, le point médian « · », employé avec une espace avant et après le signe, et la virgula ou diastole « / », employée avec une espace avant et après le signe.

Les abréviations ne sont pas développées. Chaque signe d’abréviation est représenté par un caractère Unicode conventionnel défini par une table de correspondance en annexe.

La segmentation moderne des mots est rétablie : les formes agglutinées sont séparées conformément à l’usage actuel ; les élisions relevant de l’apostrophe dans l’usage moderne sont en revanche conservées sous leur forme agglutinée.

Les noms propres sont transcrits selon une orthographe diplomatique, avec une normalisation minimale. Lorsque les particules de, des ou du sont agglutinées au nom, elles sont dissociées si cette séparation correspond manifestement à la forme du nom (établie d’après les index de : Chevalier, 1978). Les formes relevant d’une élision restent agglutinées.

Les corrections manuscrites, rayures ou biffures, sont signalées entre des doubles crochets mathématiques « ⟦ ⟧ » lorsqu’elles sont lisibles. Les passages illisibles sont signalés par une espace entre doubles crochets.

Les caractères spéciaux mobilisés dans le cadre du projet sont saisis à l’aide d’un clavier numérique importé dans l’interface d’encodage eScriptorium. Ce clavier est évolutif et susceptible de s’adapter aux besoins du corpus. Tout signe non prévu par le clavier, mais rencontré de manière récurrente, doit être signalé et une correspondance établie avec un caractère Unicode.

VII. Clavier numérique associé

Fichier : TMD_Keyboard_Superscript_v8.4b.JSON
