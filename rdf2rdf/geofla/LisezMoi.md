Ces fichier SPARQL permettent de nettoyer les données de la base Geofla une fois celles-ci converties en RDF avec la plateforme Datalift. Le « nettoyage » se fait en plusieurs étapes car la plateforme supporte mal le traitement simultané de trop grandes quantités de données.
Les données sont remises en forme (identifiants convertis en URIs, valeurs converties en littéraux, etc.) et typées à l'aide des ontologies geofla et geometrie.
Il faut appliquer ces requêtes dans l'ordre suivant:
  - sur le jeu de données RDF des régions: renommage_region.sparql
  - sur le jeu de données RDF des départements: renommage_departement_etape1.sparql 
  - sur le jeu de données RDF departement-rdf-1: renommage_departement_etape2.sparql
  - sur le jeu de données RDF des arrondissements: renommage_arrondissement_etape1.sparql 
  - sur le jeu de données RDF arrondissement-rdf-1: renommage_ arrondissement _etape2.sparql
  - sur le jeu de données RDF des cantons: renommage_canton_etape1.sparql 
  - sur le jeu de données RDF canton-rdf-1: renommage_ canton _etape2.sparql
  - sur le jeu de données RDF des communes: renommage_commune_etape1.sparql 
  - sur le jeu de données RDF commune-rdf-1: renommage_ commune _etape2.sparql
  - sur le jeu de données RDF commune-rdf-2: renommage_ commune _etape3.sparql

Les données sont alors prêtes pour la publication.
