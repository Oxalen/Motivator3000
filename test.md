# En quoi ces tests sont-ils utiles ?

Ces tests ont pour objectif de tester et d'optimiser le **system prompt** afin d’offrir un service **optimal** aux utilisateurs. Pour ces tests, nous avons utilisé différents LLM tels que Gemma, Qwen, et Mistral. Plusieurs expérimentations ont déjà été réalisées, telles que : 
- L’utilisation de trois personnages fictifs pour observer les différences dans la création des documents.
- La comparaison des résultats produits par deux LLM pour analyser leurs formats et différences.
- Des discussions avec le LLM afin de détecter des erreurs et optimiser le **system prompt**.

## Test avec le CV de Kevin

Dans le but d'observer les différences de résultats, nous allons soumettre la même requête à Motivator 3000, avec et sans notre **system prompt**.

---

### Avec le System Prompt

[Ton Adresse]  
[Ton Numéro de Téléphone]  
[Ton Adresse Email]  

[Date]  

[Nom de l’Entreprise]  
[Adresse de l’Entreprise]  

Objet : Candidature PFMP – Élève Bac Pro MELEC  

Madame, Monsieur,

Actuellement en deuxième année de Bac Pro Métiers de l'Électricité et de ses Environnements Connectés au Lycée Technique [Nom du Lycée], je suis à la recherche d'une Période de Formation en Milieu Professionnel (PFMP) afin de renforcer mes acquis et d’acquérir une expérience pratique dans le domaine de l’électricité.

Bien que mon parcours puisse sembler modeste, j'ai eu l'occasion de découvrir les bases du métier lors de mon stage en troisième chez "Electricité Toto", où j'ai appris à manipuler une échelle et à préparer le terrain pour les professionnels. Mon stage en première année de MELEC m’a également permis d’observer directement les défis et l’importance de la sécurité sur un chantier.

Je suis particulièrement motivé par l’idée de contribuer activement à des projets concrets, même si cela implique de commencer par des tâches simples. Je suis déterminé à apprendre et possède une bonne capacité d'adaptation. Bien que mes compétences techniques soient encore en développement, je suis capable de brancher une multiprise sans incident et je sais où se situe la terre dans une prise !

Je reste à votre entière disposition pour un entretien afin de vous exposer plus en détail ma motivation et mon potentiel.

Dans l'attente de vos nouvelles, je vous prie d’agréer, Madame, Monsieur, l’expression de mes salutations distinguées.

[Ta Signature (si tu imprimes)]  
Kevin Dupuis

---

### Sans le System Prompt

[Date]

[Nom du destinataire ou nom de l’entreprise (si disponible)]  
[Adresse de l'entreprise (si disponible)]  

Objet : Candidature Spontanée (Peut-être)  

Cher Monsieur/Madame,

Je vous écris pour proposer mes services… enfin, peut-être. Je m'appelle Kevin Dupuis, j'ai 18 ans, et mon objectif est simple : trouver un travail où je ne m’ennuie pas trop et qui paye bien. Un truc genre électricien à la mairie, vous voyez ?

Je suis actuellement en Bac Pro MELEC (2022-2025). Bon, je ne vais pas vous mentir, le lycée technique c’est un peu chiant, mais j’y vais principalement quand il y a un bus pour me conduire. J’ai aussi réussi mon brevet des collèges, même si ce n’était pas de tout repos.

J’ai déjà effectué quelques stages. Chez "Electricité Toto", j'ai surtout tenu une échelle et préparé des cafés. Lors d'un autre stage MELEC, j'ai vu un collègue se prendre une châtaigne – c’était mémorable.

Je sais brancher une multiprise sans cramer l’immeuble (enfin, presque), et je suis à peu près sûr de savoir où se trouve la terre dans une prise. Je suis assez agile quand il s’agit d’éviter les tâches trop compliquées, mais si nécessaire, je peux même dénuder des fils avec les dents.

Je parle français (quand je veux) et un peu d’anglais ("Yes we can", "Wesh bro"). J’aime dormir, TikTok, bricoler (mais pas trop), et regarder des tutos que je ne finis jamais.

Si vous pensez que mon profil correspond à un poste tranquille, n’hésitez pas à contacter mon pote Dédé ou mon prof d’élec, si vous arrivez à le joindre.

Cordialement (enfin, peut-être),

Kevin Dupuis
