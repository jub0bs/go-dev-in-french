---
title: La version 1 de Go est sortie
date: 2012-03-28
by:
- Andrew Gerrand
tags:
- version
- go1
summary: "Une étape majeure : l'annonce de Go 1, la première version stable de Go."
translated-by:
- Julien Cretel
original-post: https://go.dev/blog/go1
---


![un dessin du Gopher parlant dans un mégaphone](go1/gophermega.jpg)

Ce jour marque une étape importante dans le développement du langage de
programmation Go.
Nous annonçons la version 1 de Go, ou Go 1 tout court,
qui définit un langage et un ensemble de bibliothèques standards
afin de fournir une base stable pour créer des produits, projets,
et publications fiables.

Go 1 est la première version de Go à être disponible pour les
distributions binaires supportées.
Celles-ci sont disponibles pour Linux, FreeBSD, Mac OS X et,
nous sommes ravis de l'annoncer, Windows.

La motivation principale derrière Go 1 est la stabilité pour ses
utilisateurs·rices.
Les gens qui écrivent des programmes en Go 1 peuvent être assurés que ces
programmes resteront compilables et exécutables sans nécessiter de changements,
dans de nombreux environnements, et sur une échelle de temps qui se compte en
années.
De même, les auteurs·rices de livres portant sur Go 1 peuvent être assuré·e·s
que leurs exemples et explications seront utiles aux lecteurs·rices aussi bien
maintenant qu'à l'avenir.

La compatibilité ascendante est une facette de la stabilité.
Du code compilable avec Go 1 devrait, à peu d'exceptions près,
rester compilable et exécutable pendant toute la durée de vie de cette version,
malgré les mises à jour et corrections de bogues que nous apporteront à
l'occasion des versions 1.1, 1.2, etc. de Go.
Le [document de compatibilité de Go 1](https://go.dev/doc/go1compat) comprend
des recommandations plus détaillées au sujet de la compatibilité.

Go 1 représente Go tel qu'il est utilisé aujourd'hui
plutôt qu'une refonte majeure.
Lors de sa planification, nous nous sommes attelé·e·s en priorité à faire le
ménage parmi les problèmes et les incohérences et à améliorer la portabilité.
Depuis longtemps s'accumulaient de nombreux changements à apporter à Go
que nous avions conçus et prototypés mais que nous n'étions pas en mesure de
publier car ceux-ci enfreignaient la compatibilité descendante.
Go 1 incorpore ces changements, qui permettent des améliorations marquées
au langage et aux bibliothèques mais qui sont parfois sources
d'incompatibilités pour des vieux programmes.
Heureusement, l'utilitaire
[go fix](https://pkg.go.dev/cmd/go#hdr-Update_packages_to_use_new_APIs)
est capable d'automatiser une bonne partie de l'adaptation des programmes au
standard Go 1.

Go 1 apporte des changements au langage (entre autres, l'ajout de types
représentant les [caractères Unicode](https://go.dev/doc/go1#rune) et les
[erreurs](https://go.dev/doc/go1#errors)) et à la bibliothèque standard
(entre autres, l'ajout d'un [paquet time](https://go.dev/doc/go1#time) et des
renommages au sein du [paquet strconv](https://go.dev/doc/go1#strconv).
De plus, l'organisation hiérarchique des paquets a été repensée afin de
regrouper les éléments étroitement liés, comme l'illustre le déplacement des
fonctionnalités de communication avec le réseau, le
[paquet rpc](https://pkg.go.dev/net/rpc) par exemple,
dans des sous-dossiers de net.
Une liste complète des changements est documentée dans les
[notes de version de Go 1](https://go.dev/doc/go1).
Ce document constitue une référence incontournable pour les programmeurs·euses
souhaitant effectuer une migration depuis des versions antérieures de Go.

Nous avons également restructuré la suite d'outils Go autour de la nouvelle
[commande go](https://go.dev/doc/go1#cmd_go), un programme vous permettant de
récupérer, construire, installer et maintenir du code Go.
La commande go élimine le besoin de Makefiles pour écrire du code Go car elle
tire les instructions de compilation de la source même du programme Go.
Plus besoin de scripts pour produire vos exécutables !

Enfin, la sortie de Go 1 entraine la sortie d'une nouvelle version du
[SDK de Google App Engine](https://cloud.google.com/appengine/docs/go/).
Une procédure similaire de révision et de stabilisation a été appliqué aux
bibliothèques d'App Engine, fournissant ainsi aux développeurs·euses une base
sur laquelle construire des programmes pour App Engine qui continueront de
fonctionner pendant des années.

Go 1 est l'aboutissement d'un effort majeur de la part de l'équipe Go de base
ainsi que des nombreux·ses contributeurs·rices issu·e·s de la communauté de
développement en source ouverte.
Nous remercions toutes les personnes ayant œuvré à sa concrétisation.

C'est le moment opportun pour devenir un·e programmeur·euse Go.
Vous trouverez tout ce dont vous avez besoin pour vous y mettre sur
[go.dev](https://go.dev).
