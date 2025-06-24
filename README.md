# Motivator3000

*L’assistant IA local et libre pour aider les lycéens à briller dans l’écosystème des stages professionnels.*

!(./pictures/Motivator3000-Logo1.png)

(c) 2025 Lycée Louis de Cormontaigne. Responsable de projet Matthieu Farcot. Motivator3000 est un projet du *Cormont Computer Club*. 
 
# Pourquoi ce nom ?
Motivator3000 est un clin d’œil assumé à l’esthétique rétro-futuriste des films de science-fiction de série B et des jeux vidéo vintage des années 80-90. Ce nom a été choisi pour plusieurs raisons stratégiques :
- Le rétro-gaming et l’univers néo-vintage sont très populaires chez les jeunes générations, en particulier chez les lycéens intéressés par les filières techniques ou numériques. Cela crée un lien culturel immédiat avec l’univers visuel et affectif des publics cibles.
- C’est aussi un clin d’œil ludique aux générations plus âgées, encadrants pédagogiques et développeurs, qui y verront une référence ironique aux titres comme RoboCop, Mototron, ou Megatron 3000.
- Ce côté kitsch et second degré a un fort pouvoir d’attractivité dans l’univers open source, souvent sensible à la culture geek, aux blagues techniques et aux projets qui assument leur identité avec humour tout en servant une cause utile.


En résumé, Motivator3000, c’est un nom qui :
- donne envie de contribuer à un outil libre sympa et utile,
- crée de la curiosité et du capital sympathie,
- affirme une identité décomplexée et accessible, tout en assumant la puissance technique de l’IA embarquée.
 
# Objectif du projet
Développer un assistant logiciel local et libre, capable d’aider les lycéens de la voie professionnelle à :
- rédiger des CV valorisants et bien structurés,
- produire des lettres de motivation personnalisées à partir d’annonces de stage ou d’alternance,
- mettre en avant les compétences issues de leurs référentiels de formation.
 
## Un assistant boosté à l’IA (mais en local)
Le cœur de Motivator3000 repose sur une IA embarquée, renforcée par une architecture RAG (Retrieval-Augmented Generation).


Le système permet à l’IA de générer des textes contextualisés à partir :
- des référentiels officiels des filières professionnelles,
- des annonces fournies par les élèves (PDF, copier/coller, etc.),
- de modèles de CV/lettres adaptés aux standards professionnels.
 
## RGPD et souveraineté numérique : priorité absolue
Motivator3000 fonctionne 100% en local, sans traitement distant, afin de garantir :
- le respect du RGPD, en particulier pour les élèves mineurs (moins de 16 ans),
- la maîtrise complète des données, sans cloud, sans inscription, sans tracking,
- la possibilité de déploiement même sans connexion internet (réseau local ou poste unique).
 
## Open Source et licence libre
Tous les développements sont publiés sous AGPL v3, pour permettre :
- aux autres lycées et structures de déployer librement l’outil,
- aux enseignants, responsables de BDE ou DDFPT et développeurs de l’adapter et l’enrichir,
- à la communauté de partager les améliorations en toute liberté.

# Motivator3000, le point sur le projet :
Ce qui a été fait pour l’instant, ou est en cours de réalisation
 
## Exploration des modèles IA open source adaptés à un usage local
Objectif : identifier des modèles de langage suffisamment puissants pour générer des contenus personnalisés (CV, lettres de motivation), mais légers et respectueux des contraintes locales (pas de cloud, pas de dépendance à des API commerciales).


Modèles testés :
- Gemma (gemma-2-27b et gemma-2-9b)
- Mistral (mistral-small-3.2)
- LLaMA (llama-3.3-70b)
- DeepSeek (deepseek-r1-0528-qwen3-8b)
- Qwen (qwen3-8b)


Critères évalués :
- Qualité de génération (fluidité, structure)
- Capacité à tourner en local (sur CPU ou GPU)
- Volume mémoire et performance sur machine (très) modeste
 
Constat :  Malgré des performances linguistiques solides, les réponses produites par les modèles testés sont trop déterministes et génériques. Les lettres générées manquent de variabilité, d’originalité et surtout de prise en compte réelle du contexte scolaire et professionnel des lycéens. On observe que, quelle que soit l’annonce ou le profil fourni, les lettres finissent par se ressembler fortement, avec des tournures stéréotypées et un contenu creux. Toutefois, vu les perfromances et les résultats obtenus, le choix pour l'instant porte du Gemma-2-9b de google.


Globalement, ce comportement souligne les limites d’un modèle généraliste non enrichi, incapable d’ajuster sa réponse en fonction de référentiels métier ou de parcours spécifiques.  
Cela justifie pleinement l’adoption d’une architecture RAG (Retrieval-Augmented Generation), permettant de connecter l’IA à une base documentaire métier, adaptée aux formations professionnelles suivies par les élèves.
 
## Conception d’un système de prompt structuré
Objectif : formuler des instructions claires et précises pour guider les modèles dans leurs productions (system prompt).
Actions menées :
- Définition de plusieurs types de prompts : création de CV, lettre pour une alternance, lettre pour un stage, mise en valeur d’un projet scolaire, etc.
- Création de gabarits de prompt intégrant les données contextuelles (niveau d’étude, spécialité, type de poste ciblé, référentiel).
- Tests manuels pour évaluer la réactivité des modèles à ces instructions.


Résultat : Les prompts bien structurés améliorent la pertinence, mais ne suffisent pas en l’absence de connaissance métier spécifique au contexte du lycée professionnel. D’où la nécessité d’implémenter un système RAG avec accès aux référentiels.

