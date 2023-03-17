# Développez un chatbot pour réserver des vacances

## Objectifs
FlyMe est une agence qui propose des offres de voyage clé en main pour les particuliers et les professionnels.
L'objectif de ce projet est de développer un chatbot qui aidera les utilisateurs à choisir une offre de voyage. La première étape consiste à construire un MVP qui permettra aux employés de FlyMe de réserver facilement un billet d'avion pour leurs vacances. Le MVP devra être capable d'identifier les cinq éléments suivants dans la demande de l'utilisateur :

- Ville de départ
- Ville de destination
- Date de départ
- Date de retour
- Budget maximal pour le prix total du billet
Si l'un de ces éléments est manquant, le chatbot devra être capable de poser des questions pertinentes en anglais à l'utilisateur pour comprendre pleinement sa demande. Une fois que le chatbot pense avoir compris tous les éléments de la demande de l'utilisateur, il devra reformuler la demande et demander à l'utilisateur de valider sa compréhension.

## Dataset
Pour ce projet, j'ai utilisé un dataset contenant des histoires d'échanges entre un chatbot et un utilisateur. Le dataset est plus étendu que ce qui est requis pour le MVP, mais cela me permet de garder le même dataset pour les étapes futures du projet et ainsi gagner du temps.

## Méthodologie
J'ai automatisé l'intégration et le développement dès le début du projet, et de procédé par itérations plutôt que de travailler de manière séquentielle.

## Stack technique
Le stack technique pour ce projet comprend :

- Le kit de développement Microsoft Bot Framework SDK v4 pour Python
- Le service cognitif Azure LUIS pour l'analyse sémantique d'un message entré par l'utilisateur et sa structuration pour le traitement par - le chatbot (il devrait permettre d'identifier les cinq éléments demandés)
- Le service Azure Web App pour exécuter une application web sur Azure Cloud
- L'émulateur Bot Framework pour tester le chatbot localement et en production. C'est une interface qui permet à un utilisateur d'interagir avec le chatbot.

## Points d'attention
Il est essentiel de surveiller les performances du chatbot lorsqu'il est en production pour éviter qu'il ne fournisse des réponses incorrectes. À cet effet, j'ai utilisé le service d'application insight Azure, qui permet de suivre et d'analyser l'activité du chatbot en production. De plus, cet outil permet de déclencher une alerte lorsque le chatbot donne plusieurs mauvaises réponses aux utilisateurs.

Pour assurer la pertinence du chatbot, il est nécessaire d'évaluer les performances du modèle LUIS sous-jacent hors ligne. Par conséquent, j'ai développé des scripts qui permettent l'entraînement et l'évaluation du modèle, en plus de ceux qui permettent l'exécution du pipeline complet pour générer l'application de chatbot web.

## Compétences mises en oeuvre
1. Intégrer la sortie du modèle dans un produit informatique fini:
- Mettre en place une réponse automatique à partir d'un message utilisateur
- Vérifier la qualité des dialogues avec l'utilisateur
- Créer une interface de conversation avec le chatbot en anglais
2. Intégrer une chaîne de traitement IA dans un outil informatique via Git:
- Développer et tester le code d'une chaîne de traitement IA
- Exécuter automatiquement des tests unitaires lors du déploiement du code (CI/CD)
- Organiser le code en fonctions ou classes
- Utiliser un outil de gestion de version Git et stocker le code sur un repository Github
1. Piloter la performance du modèle en production:
- Définir les critères d'évaluation de la performance du modèle
- Calculer automatiquement les critères d'évaluation de la performance à partir des dialogues enregistrés et labellisés
- Mettre en place un seuil d'alerte pour détecter les erreurs du chatbot
- Utiliser l'outil de suivi Azure Application Insight pour suivre les performances du chatbot
- Définir une méthodologie de mise à jour du modèle en production (métriques d'évaluation, fréquence de calcul de la performance, etc.)

## Mots-clés
#chatbot #voyages #MicrosoftBotFramework #AzureLUIS #AzureWebApp #NLP #analysesemantique #python #MVP #automatisation #performance #monitoring #dataset #appinsight #evaluation #CI/CD #integrationcontinue

## Autres repositories liés au projet

- [FlyMeBot_App](https://github.com/AnodeGrindYo/FlyMeBot_App/actions)
- [FlyMeBot_WepPage](https://github.com/AnodeGrindYo/FlyMe_WebPage/actions)

