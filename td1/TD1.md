# TD1  

**1)** La méthode GET peut être utilisé pour la personnalisation d'une page WEB (favoris, etc), elle sert aussi pour stocker les données qui permettent à un utilisateur de les retrouver quand il a besoin, mais par contre elle ne chiffre pas les données donc les données dans l'URL sont rendus visibles. La méthode est souvent utilisé pour recevoir les réponses serveur.
   La méthode POST est utilisé pour la confidentialité des données et sont donc invisibles dans l'URL (les données personnelles sont envoyés par des formulaires ou autres). Cette méthode est utilisé pour envoyé les données vers un serveur.

**2)** Voir le fichier PNG

**3)** Le protocole HTTP est extensible car il transite par TCP ou TLS et permet de récupérer en réponse beaucoup de sorte de données comme des images, vidéos, documents, renvois de formulaires HTML vers serveurs.
   Le protocole HTTP est extensible car il permet aussi d'intégrer des en-têtes qui offrent différentes transmissions comme des en-têtes général, en-têtes des requêtes, en-têtes des réponses, en-têtes d'entités.

**4)** Le protocole HTTP est qualifié de sans état car il ne permet pas le lien entre plusieurs requêtes, plusieurs solutions sont possibles pour contrer ce problème par le biais de cookies et de l'extensibilité des en-têtes.

**5)** L'URL se décompose en plusieurs parties. L'URL commence toujours par un protocole (http:// (non sécurisé) ou https:// (sécurisé)), suivi d'un sous-domaine (très souvent www.), suivi d'un nom de domaine qui est le nom du site et qui devra être acheté , le nom de domaine se termine toujours par (.com ou autre selon l'origine du site) ce qui suivra dans l'URL sera séparé du reste par un / et indiquera le chemin en requête vers le serveur.

**6)** Il existe 5 familles de codes de réponse HTTP : 

   - Réponses informatives qui ont pour but d'informer l'utilisateur d'une réponse à venir du serveur, de répondre aux en-têtes upgrade afin d'informer du protocole sur le serveur, permet aussi de répondre aux en-         êtes link qui permettent de précharger en attendant la réponse serveur, exemple: 100 Continue
   - Réponses de succès qui permet d'indiquer que la requête a été traitée avec succès, la réussite de la requête variant en fonction de la méthode HTTP employé (GET, POST...), exemple: 200 OK
   - Réponses de redirection qui indiquent que le client doit effectuer une action supplémentaire pour compléter la requête, exemple 301 Moved Permanently.
   - Réponses d'erreur - qui indique qu'il y a une erreur dans la requête client ou qu'il n'a pas les permissions, ce qui empêche le serveur de la traiter avec succès, exemple 404 Not Found
   - Réponses d'erreur côté serveur qui dans le cas d'une situation qu'il ne peut pas traiter, exemple 500 Internal Server Error

**7)** Le principe de la négociation entre le client et le serveur est de convenir de la meilleure représentation des ressources comme une version HTML ou XML et autres en fonction de ce que le client apprécie mais aussi des capacités du serveur. Le serveur utilise ensuite l'URL pour choisir parmi les différentes représentations, et la renvoie vers le client avec une URL.
   Il existe deux mécanismes pour choisir la représentation : 
   - Les en-têtes HTTP spécifiques qui sont envoyés par les clients.
   - Les codes de réponse HTTP (comme Unsupported Media Type) qui sont envoyés par le serveur et utilisés comme mécanisme de recours.

