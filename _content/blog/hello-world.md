---
title: "Go : quoi de neuf en mars 2010 ?"
date: 2010-03-18
by:
- Andrew Gerrand
summary: Premier billet !
translated-by:
- Julien Cretel
original-post: https://go.dev/blog/hello-world
---


Bienvenue sur le blog officiel de Go. Nous, les membres de l'équipe Go,
espérons utiliser ce blog pour tenir le monde au courant du développement du
langage de programmation Go et de l'écosystème croissant de bibliothèques et
d'applications qui l'entoure.

Quelques mois se sont écoulés depuis notre lancement (en novembre l'année
dernière) ; parlons donc de ce qui s'est passé depuis dans le monde de Go.

L'équipe principale basée chez Google a poursuivi le développement du langage,
des compilateurs, des paquets, des outils, et de la documentation.
Les compilateurs produisent maintenant du code qui, dans certains cas,
s'exécute plus vite, d'un facteur de 2 à un ordre de grandeur, qu'au moment
de la sortie.
Nous avons réuni des graphiques [NDT : ceux-ci ne sont malheureusement plus
disponibles en ligne] résultant de quelques
[tests de performance](https://web.archive.org/web/20100411022902/http://godashboard.appspot.com/benchmarks),
et la page d'[état de construction](https://web.archive.org/web/20100411022902/http://godashboard.appspot.com)
indique, en continu, la fiabilité de chaque groupe de changements apporté au
dépôt.

Nous avons effectué des changements de syntaxe visant à rendre le langage plus
concis, plus rationnel, et plus flexible.
Les points-virgules
[ont pratiquement disparu](https://web.archive.org/web/20100413054626/https://groups.google.com/group/golang-nuts/browse_thread/thread/5ee32b588d10f2e9)
du langage.
[L'élément de syntaxe ...T](https://web.archive.org/web/20100324041415/https://golang.org/doc/go_spec.html#Function_types)
simplifie la gestion d'un nombre arbitraire de paramètres d'un même type d'une
fonction.
L'élément de syntaxe x[lo:] est maintenant un raccourci équivalent à
x[lo:len(x)].
Go permet désormais la manipulation de nombres complexes de manière native.
Consultez [les notes de version](https://web.archive.org/web/20100312050655/https://golang.org/doc/devel/release.html)
pour plus de détails.

Les bibliothèques tierces sont désormais mieux supportées par
[Godoc](https://pkg.go.dev/golang.org/x/tools/cmd/godoc),
et un nouvel outil - [goinstall](https://web.archive.org/web/20100411211758/https://golang.org/cmd/goinstall) -
visant à faciliter leur installation vient de sortir.
De plus, nous avons commencé à plancher sur un système de suivi des paquets
pour vous faciliter la découverte de ce dont vous avez besoin.
Vous pouvez observer les balbutiements de ce système sur la page dédiée aux
paquets.

Plus de 40000 lignes de code ont été ajoutées à
[la bibliothèque standard](https://web.archive.org/web/20100318042023/http://golang.org/pkg/),
qui a vu arriver de nombreux paquets tout nouveaux, dont une bonne partie a
été écrite par des contributeurs·rices externes.

D'ailleurs, en ce qui concerne les tierces parties, depuis le lancement, une
communauté très active s'est développée sur notre
[liste de diffusion](https://groups.google.com/g/golang-nuts)
et notre canal irc (#go-nuts sur freenode).
Nous avons officiellement ajouté plus de 50 personnes au projet.
Leurs contributions vont de corrections de bogues et rectifications de la
documentation à des paquets de la bibliothèque standard et au support de
systèmes d'exploitation additionnels (Go tourne désormais sur FreeBSD, et un
[portage vers Windows](https://web.archive.org/web/20100327212403/https://code.google.com/p/go/wiki/WindowsPort)
est en cours).
Ces contributions représentent à nos yeux notre plus grand succès à ce jour.

Nous avons également recueilli des avis favorables. Cet
[article récent de PC World](https://web.archive.org/web/20100304055923/https://www.pcworld.idg.com.au/article/337773/google_go_captures_developers_imaginations/)
résume bien l'enthousiasme généré par le projet.
Plusieurs auteurs·rices de blog ont commencé à documenter leurs expériences
avec le langage
(voir [ici](https://web.archive.org/web/20100314205410/https://golang.tumblr.com/),
[ici](https://web.archive.org/web/20100326140832/https://www.infi.nl/blog/view/id/47),
et [ici](https://web.archive.org/web/20100329135956/https://freecella.blogspot.com/2010/01/gospecify-basic-setup-of-projects.html)).
Dans l'ensemble, la réaction de nos utilisateurs·rices s'est avérée très
positive ;
un néophyte a d'ailleurs émis la remarque suivante :
["J'en suis sorti très impressionné. Go maintient avec élégance l'équilibre
entre simplicité et puissance."](https://groups.google.com/g/golang-nuts/c/X6vdWfhWLtI)

Quant à l'avenir ? Nous avons prêté une oreille attentive aux innombrables voix
nous soufflant ce dont elles ont besoin, et nous mettons en ce moment tout en
œuvre pour que Go soit prêt pour les choses sérieuses.
Nous améliorons le ramasse-miettes, l'ordonnanceur, les outils, et les paquets
de la bibliothèque standard, et nous étudions également l'ajout de
fonctionnalités au langage.
2010 va être une année passionnante pour Go, et nous avons hâte de travailler
main dans la main avec la communauté pour qu'elle soit couronnée de succès.
