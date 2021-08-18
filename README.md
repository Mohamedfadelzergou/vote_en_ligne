# vote_en_ligne
Enoncé du projet : Dans une entreprise multinationale, son PDG (président-directeur général) désire organiser un vote à distance électronique entre ces personnelles pour élire un nouveau responsable dans son siège. Pour cela, un ensemble de n correspondant ou personnels désirent voter un représentant parmi m candidats en utilisant la messagerie électronique sécurisée (OpenPGP). Chaque votant Vi sera identifié par son nom, son prénom et sa date de naissance. On affecte à chaque votant un numéro de vote I. Vi possède une clé publique KpVi connue de tout le monde et une clé privée KprVi . Un votant envoie deux messages chiffrés contenant son bulletin de vote B et son numéro d’identification I à deux centres. 1. Un centre de comptage CO : Ce centre reçoit un message chiffré d’un votant Vi, contenant les informations (I, B chiffré et destiné à DE) avec les restrictions suivantes : CO pourra lire I et ne doit pas accéder au bulletin de vote B. CO possède une liste contenant nom, prénom, date de naissance et I de tous les votants. Son rôle est de vérifier l’identité de Vi à partir de I et la clé publique de Vi. Ensuite, CO marque Vi sur la liste pour éviter un second vote de I. Enfin, CO chiffre (I, B chiffré et destiné à DE) et l’envoie au centre DE. Les clés privée et publique de CO sont KprCO et KpCO . 2. Un centre de dépouillement DE : Ce centre reçoit le message de CO et le message chiffré de Vi contenant (I, B). Sa tâche consiste à déchiffrer les deux messages sans possibilité d’identifier Vi. Si après déchiffrement les deux messages sont égaux à (I, B) alors le vote de Vi sera validé. Les clés privée et publique de DE sont KprDE et KpDE
