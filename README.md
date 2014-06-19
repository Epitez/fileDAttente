File D'Attente
==============

# Aperçu du système #

Fournir un système permet de délivrer des tickets pour organiser l'accès à des guichets.
Ce système doit permettre :

* accepter plusieurs guichets.
* accepter plusieurs types de guichets, fournissant différents services. Les fils d'attente étant gérée par type.
* fournir des tickets aux clients via :
	- des bornes fournissant des tickets papier
	- des appareils Android délivrant des tickets au format numérique
* permettre de fournir des rapports de statistique :
	- par ticket : durée d'attente
	- en moyenne durée d'attente, durée d'intervention, % d'abandon ... :
		+ par ticket
		+ par guichet
		+ par type de guichet

# Guichet #

## Pour un guichet non identifié ##

À partir d'un guichet il est possible de :

* s'identifier dans le système :
	- un code d'authentification (unique par guichet)
	- un type de guichet

## Pour un guichet identifié ##

À partir d'un guichet il est possible de :

* appeler le prochain client
* rappeler le prochain client (appel sur écran)
* abandonner un client
* prendre en compte un client
* fermer le guichet
* éventuellement, transférer un client sur un autre type de guichet

# Distributeur de ticket papier #

## Non enregistré sur le système ##

Un distributeur peut :

* s'authentifier sur le système (pas de code d'authentification)
* afficher des statistiques d'utilisation via un code d'accès :
* récupérer l'historique d’utilisation (connexion, délivrance de ticket)
moyenne temps d'utilisation (du 1er clic à la délivrance d'un ticket)
nombre d'abandons
  
##Enregistré sur le système##

Un distributeur peut :

* récupérer la liste des types de file d'attente (assurer qu'une mise à jour sur le système soit prise en compte pour toute demande de ticket après un maximum d'un délai de 5 minutes)
* proposer des tickets pour chaque type de file d'attente disponible dans le système ;
(éventuellement) fournir au système, sur demande, des statistiques d'utilisation :
* récupérer l'historique d’utilisation (connexion, délivrance de ticket)
moyenne temps d'utilisation (du 1er clic à la délivrance d'un ticket)
nombre d'abandons

# Afficheur du système #
  
Un afficher peut :

* se connecter au système
* récupérer pour chaque guichet :
	- le type du guichet
	- le ticket attendu

# Distributeur de e-ticket sur des smart-phone android #

Un distributeur peut :

* récupérer la liste des types de file d'attente du système
* prendre un ticket d'un type de file d'attente disponible dans le système ;
* abandonner un ticket (non obligatoire, mais automatique si demande de nouveau ticket).

   

