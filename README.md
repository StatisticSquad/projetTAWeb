projetTAWeb
===========

Projet Technologies Avancées du Web



API STEAM

Methode d'accès :
The Steamworks Web API is accessed by making HTTP/HTTPS requests to api.steampowered.com. Similiar to the Steamworks C++ API, the Web API has been divided into multiple interfaces that contain related methods. The URI forResponse Format

Steam supports returning Web API responses in multiple formats. By default, all responses are returned JSON encoded. However, each request can optionally contain a format parameter to specify the desired response format. The following values can be passed for this parameter: xml, json, and vdf.

A flexible solution should be used to parse Web API results as each method may return results in an arbitrary order.
API Keysed.com/<interface>/<method>/<method_version>/

Faire défiler de vraie stats en bandeau


Il faut une clef pour consulter cette api
Peu de données exploitables en fait




Data.un.org
Des centaines de données chiffrées qui se récupères par l'api
https://www.undata-api.org/wiki/filteredquery
On requète par une simple query paramètrée. On recupère du XML.


Le site theesa.com fournit de nombreuses données rafinées (non exploitables automatiquement) sur le monde du jeu video.


Le site de l'OCDE, une api simple et efficace avec des requetes directes
http://stats.oecd.org/OpenDataAPI/OData.html
La sortie se fait en JSon

Le site data.gouv n'a pas encore d'api, on récupère les donnée en XSL

En rdf On a le world factbook de la CIA

http://datahub.io/dataset/cia-world-factbook


Un tuto RDF/Jena
http://web-semantique.developpez.com/tutoriels/jena/introduction-rdf/



Pour afficher les graphes

JQPlot
ou mieux
FusionCharts.com


RDF tuto W3C
http://www.w3schools.com/rdf/rdf_intro.asp



Rajouter un flux rss


Objectif pour le TP 10/10/13
Ensemble. Récupérer et formater dans un fichier json,les données des API : au moins Un.data 
En attendant : trouver le plus de statistiques statiques possibles, les formater Json et trouver une ontologie

On a décidé d'utiliser Play avec un plugin RDF (empire), plutot que Jena pour se faciliter la vie au moment de developper l'interface web en Java


10/10/13
Une ontologie eurostat

17/10/13
http://ontologycentral.com/2009/01/eurostat/
http://wifo5-04.informatik.uni-mannheim.de/eurostat/

dvl: l'utilisateur donne du sens aux données qui lui sont proposées. Interaction entre les utilisateurs. Analyses des actions des utilisateurs.
Regarder les fonctionnalités de commentaires et d'administration offertes par play ou utiliser un framework php et le faire fonctionner avec Java.

24/10/13 :


http://www.thefigtrees.net/lee/blog/2008/03/modeling_statistics_in_rdf_a_s.html
On va stocker une partie des données récupérées sur le serveur. probablement les plus consultées.
Une autre partie sera requétée en live.



A FAIRE : une fonction qui renvoie toutes les stats suivant leur indice (ex : 70 %) ce qui permettrait de générer des statistiques puisque l'on trouverait des stats qui iraient ensemble.



