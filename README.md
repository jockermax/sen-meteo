# sen-meteo

TITRE :  Application Web Météo utilisant HTML, CSS et Javascript

APERÇU:

Il s'agit d'une simple application Web d'une seule page construite en utilisant HTML, CSS et JavaScript.

Permet aux utilisateurs d'afficher les données météorologiques actuelles pour leur emplacement ou pour toute ville recherchée.

Récupère les données météorologiques en temps réel à partir de l'API OpenWeatherMap.

UI/UX :

Interface utilisateur propre et réactive construite en utilisant HTML et CSS.

Navigation par onglets pour basculer entre la météo locale et la météo de recherche.

Chargeurs animés et conteneurs modulaires pour une UX fluide.

Les icônes visuelles, les noms de villes et les statistiques météorologiques sont affichés dans une présentation organisée.

CARACTÉRISTIQUES:

Obtenez automatiquement la météo de l'emplacement actuel à l'aide de l'API de géolocalisation.

Recherchez la météo par nom de ville via le champ de saisie de texte.

Affichez les données météorologiques telles que la température, le vent, l'humidité, les nuages, etc.

Icônes dynamiques pour représenter les conditions météorologiques et les drapeaux des pays.

Éléments interactifs tels que des onglets, des boutons et des soumissions de formulaires.

TECHNIQUE : HTML pour la structure et la sémantique du contenu.

CSS personnalisé pour styliser l'interface visuelle.

JavaScript Vanilla pour la logique côté client et la manipulation du DOM.

JS asynchrone pour des appels d'API et une récupération de données transparents

Intégration avec l'API OpenWeatherMap pour obtenir des données météorologiques.

API de géolocalisation pour accéder aux coordonnées des utilisateurs.

Stockage local pour mettre en cache l'emplacement de l'utilisateur.

Structure de code modulaire pour la lisibilité et la maintenabilité.

ÉTAPES POUR RÉCUPÉRER LES API : 

RÉCUPÉRATION DE L'API MÉTÉO LOCALE :

1. Lorsque l'utilisateur clique sur l'onglet « Météo locale », l'API de géolocalisation est appelée pour obtenir les coordonnées de latitude et de longitude.

2. Les coordonnées sont stockées dans le stockage de session pour mettre en cache l'emplacement de l'utilisateur.

3. Afficher les indicateurs de chargement pendant que l'appel API est en cours.

4. Construisez l'URL de l'API avec :

    Coordonnées Lat, Lon

    Ouvrez la clé API WeatherMap

    Format des unités en métrique.

5. Effectuez une requête GET asynchrone vers l'URL de l'API à l'aide de la méthode fetch().

6. Gérez la promesse renvoyée par fetch() pour obtenir les données JSON de réponse.

7. Retirez l'indicateur de chargement une fois la réponse reçue.

8. Extrayez les données météorologiques requises des objets JSON tels que :

 Nom de Ville

 Description météo

 Température

 Vitesse du vent

  Humidité

 Nébulosité

9. Remplissez les valeurs extraites dans les éléments d'interface utilisateur respectifs pour afficher les données météorologiques.

RÉCUPÉRATION DE L'API DE RECHERCHE MÉTÉO :

1. Obtenez la chaîne du nom de la ville dans le champ de saisie de recherche du formulaire soumis.

2. Affichez l'indicateur de chargement pendant l'appel d'API.

3. Coconstruisez l'URL de l'API avec :

  Nom de Ville

  clé API

  Unités métriques

4. Effectuez une requête GET asynchrone vers l'URL de l'API à l'aide de fetch().

5. Gérez la promesse d'obtenir une réponse aux données météorologiques JSON.

6. Masquez l'indicateur de chargement après la réponse.

7. Extrayez et affichez les données météorologiques sur l'interface utilisateur comme pour la météo locale.

FONCTIONNEMENT: 

Onglets pour basculer entre les vues météo locales et de recherche

API de géolocalisation appelée sur le chargement d'onglets locaux pour obtenir les coordonnées de l'utilisateur.

API appelée avec des coordonnées pour récupérer des données météorologiques locales.

L'onglet de recherche permet de rechercher la météo par saisie du nom de la ville.

Appels API avec le nom de la ville pour obtenir des données météorologiques.

 Réponses JSON analysées et affichées sur l'interface utilisateur modulaire.

Icônes, animations et transitions pour un retour visuel.

CONCLUSION:

En résumé, ce projet démontre le développement d'une application météorologique Web simple mais fonctionnelle utilisant des technologies frontales de base. Il implémente une interface utilisateur propre et intuitive avec HTML et CSS tandis que JavaScript gère la logique côté client. La récupération de données de manière asynchrone à partir d'une API météo et la mise à jour du DOM créent une expérience transparente sans actualisation de page.
