# tp3
J'ai débuté mon projet en créant un nouveau projet Maven dans mon environnement de développement, puis j'ai ajouté les dépendances nécessaires dans le fichier pom.xml pour Spring MVC, Thymeleaf et Spring Data JPA.

Ensuite, j'ai conçu une entité JPA nommée Patient, comprenant les attributs essentiels tels que l'identifiant, le nom, le prénom, etc., et je l'ai annotée avec les annotations JPA appropriées telles que @Entity, @Table, etc.

Pour la manipulation de l'entité Patient, j'ai élaboré une interface PatientRepository étendant JpaRepository<Patient, Long>, qui fournit des méthodes pour effectuer les opérations CRUD de base sur cette entité.

Pour gérer les requêtes HTTP associées aux patients, j'ai développé un contrôleur nommé PatientController, qui offre des méthodes pour afficher les patients, gérer la pagination, effectuer des recherches et supprimer des patients.

Pour une interface utilisateur conviviale, j'ai créé des pages HTML avec Thymeleaf pour afficher la liste des patients, les résultats de recherche, etc., en utilisant des expressions Thymeleaf pour intégrer les données dynamiques fournies par le contrôleur.

Pour faciliter la navigation à travers les données, j'ai configuré la pagination en utilisant les fonctionnalités fournies par Spring Data JPA.

Pour permettre une recherche efficace, j'ai implémenté la fonctionnalité de recherche des patients par leur nom, prénom, etc.

En ce qui concerne la gestion des données, j'ai mis en œuvre la logique de suppression des patients en utilisant les méthodes disponibles dans le PatientRepository, et j'ai ajouté une fonctionnalité d'édition pour mettre à jour les informations des patients.

Pour garantir l'intégrité des données, j'ai ajouté des validations côté serveur et une couche de sécurité pour restreindre l'accès à certaines fonctionnalités aux utilisateurs authentifiés.

Enfin, j'ai inclus des fonctionnalités de tri pour permettre aux utilisateurs de trier les patients selon différents critères.
