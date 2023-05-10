# studi-api
Création API pour exercice

Endpoints principaux :

Publier une photo :

Endpoint : POST /photos
Description : Permet à un utilisateur de publier une nouvelle photo.
Paramètres : L'image (fichier), la légende (texte), les hashtags (tableau de chaînes), la localisation (latitude et longitude).
Réponse : ID de la photo publiée et statut de réussite.
Obtenir une photo :

Endpoint : GET /photos/{photo_id}
Description : Récupère les détails d'une photo spécifique.
Paramètres : ID de la photo.
Réponse : Détails de la photo (y compris l'image, la légende, les hashtags, la localisation, le nombre de likes, etc.).
Modifier une légende de photo :

Endpoint : PUT /photos/{photo_id}/caption
Description : Permet à l'utilisateur de modifier la légende d'une photo.
Paramètres : ID de la photo.
Données de requête : Nouvelle légende (texte).
Réponse : Statut de réussite de la modification.
Supprimer une photo :

Endpoint : DELETE /photos/{photo_id}
Description : Permet à l'utilisateur de supprimer une photo.
Paramètres : ID de la photo.
Réponse : Statut de réussite de la suppression.
Commenter une photo :

Endpoint : POST /photos/{photo_id}/comments
Description : Permet à un utilisateur de commenter une photo.
Paramètres : ID de la photo.
Données de requête : Contenu du commentaire (texte).
Réponse : ID du commentaire ajouté et statut de réussite.
Rechercher des photos par localisation :

Endpoint : GET /photos/search
Description : Permet de rechercher des photos en fonction de la localisation.
Paramètres : Latitude et longitude.
Réponse : Liste des photos correspondantes avec leurs détails.
Créer un hashtag :

Endpoint : POST /hashtags
Description : Permet à un utilisateur de créer un nouveau hashtag.
Paramètres : Nom du hashtag.
Réponse : ID du hashtag créé et statut de réussite.
Rechercher des photos par hashtag :

Endpoint : GET /hashtags/{hashtag_id}/photos
Description : Récupère les photos associées à un hashtag spécifique.
Paramètres : ID du hashtag.
Réponse : Liste des photos correspondantes avec leurs détails.
