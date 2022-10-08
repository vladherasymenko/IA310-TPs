Question 1 : 
	- Accessible, car on peut supposer que tous les gestionnaires connaissent où se trouvent les autres planètes 
	et quels biens devraient être livrés/sont en cours de livraison 
	- Déterministe. Les actions des vaisseaux ont un impact clair sur l'environement : livraison des biens. 
	De plus on suppose qu'il n'y a rien qui peut se passer 
	avec les veisseaux en route (pas d'accidents ni de pannes)
	- Épisodique, parce que chaque livraison peut être vue comme une action atomique ne dépendante pas de livraisons précédentes. 
	- Statique : les planètes sont fixés/immobiles et ainsi l'environement ne peut pas évoluer lui-même. 
	- Continu : car il y a une continuité des positions possibles entre les planètes 
	(toutefois, cela est un peu litigieux, vu que la représentation des flottants en python est telle que leur précision est fixée et,
	 ainsi, toutes les positions des vaisseaux sont techniquement dénombrables) 

Question 2 : 
	Les items ne sont pas considérés comme agents, car, pour dire proprement, ils ne satisfont pas la définition d'un agent : 
	les items ne sont capables ni de percevoir l'environnement, ni d'agir sur lui, ils n'exhibent aucun comportement autonome et n'évoluent pas
	dans le temps (bien qu'ils soient déplacés d'un planète à l'autre par des vaisseaux)

Qustion 3 : 
	Le processus de génération des biens sur les planètes étant aléatoire, le rapport entre le nombre de biens livrés et le nombre de biens en
	cours de livraison est variable lui aussi, mais on constate que ce rapport tend à diminuer vers la fin de la simulation 

Question 4 : 
	Il s'agit d'une organisation cooprérative, car les agents utilisent le Contract Net Protocol pour communiquer entre eux

Qustion 5 : 
	Le seule aspect qui change, c'est que l'environnement est maintenant :
	- Dynqmique : car les routes (et ainsi l'environnement) peuvent dèsormais évoluer [en changeant sa bande-passante]

Question 6+7 : 
	Cette fois-ci, les encombrement sur les routes nuit aux fontionnement normale du système en rompant/relantissant les routes entre les planètes
	ce qui force les vaisseaux de s'adapter à ces nouvelles conditions et à choisir d'autres routes (qui sont forcément moins optimales qu'autrefois).
	On observe donc le fait que le rapport entre les biens livrés et non livrés devient beaucoup plus variable. 
	
Question 8 : 
	Après avoir lancé la simulation plusieurs fois, on peut constater que le Road Branching Factor a un impact significatif sur l'écart entre
	les biens livrés et non-livrés : quand ce paramètre est petit, les routes ne changent presque pas leurs états et le système se comporte 
	comme si l'environnement n'était même pas dynamique (les agents s'adaptent assez vite à ces rares changements). Et quand il est élevé, 
	l'environement se change tellement vite que les vaisseaux n'arrivent pas à se bien adapter à des nouvelles condiations et le rapport 
	entre les biens livrés/non livrés grandit.   
	
 