# cisse
  portofolio 
  Prtojet Economie Financi`ere
Th`eme :Analyse de la sensibilit´e du CAC40
aux march´es europ´eens : un mod`ele
multifactoriel bas´e sur le STOXX50 et le DAX
R´ealis´e par :
Christ J BASSE
Malang CISSE
Doudou MANE
M2 PSA Universit´e de Lorraine Metz , UFR MIM
Introduction
L’int´egration croissante des march´es financiers europ´eens implique une inter-
d´ependance forte entre les principaux indices boursiers.Le CAC 40, princi-
pal indice fran¸cais, est expos´e aux dynamiques ´economiques et financi`eres eu-
rop´eennes, notamment via l’Allemagne premi`ere ´economie de la zone europe
ainsi que les grands groupes paneurop´eens.
L’objectif de ce projet est d’´evaluer la sensibilit´e du CAC 40 aux march´es eu-
rop´eens en estimant un mod`ele ´econom´etrique multifactoriel expliquant
les rendements du CAC 40 par ceux :
• du STOXX 50, repr´esentant le march´e europ´een global,
• du DAX, repr´esentant le noyau industriel allemand.
Cette approche permet d’identifier les sources du risque syst´ematique du
march´e fran¸cais.
Mod`ele th´eorique de r´egression lin´eaire multiple
Le rendement du CAC 40 `a l’instant t, not´e Rcac(t), est expliqu´e par les rende-
ments de deux indices de march´e Rstoxx(t) et Rdax(t) selon le mod`ele :
Rcac(t) = α+ β1Rstoxx(t) + β2Rdax(t) + εt, t= 1,...,T (1)
o`u :
1
• α est une constante r´eelle .
• β1,β2 sont des coefficients r´e´els de r´egression repr´esentant la sensibilit´e du
CAC 40 aux indices stoxx et dax.
• εt est le terme d’erreur, suivant la loi normale centr´e de param´etre :
E[εt] = 0, Var(εt) = σ2, Cov(εt,εs) = 0 pourt̸= s
Revue de la litt´erature
Les mod`eles multifactoriels sont largement utilis´es en finance pour expliquer
les rendements des indices boursiers. Ces mod`eles permettent de distinguer
les performances propres d’un march´e des effets des facteurs externes. Dans le
mod`ele utilis´e ici :
• β1 mesure la sensibilit´e du CAC40 au march´e europ´een global (STOXX50),
• β2 mesure la sensibilit´e du CAC40 `a l’´economie allemande DAX,
• α repr´esente la performance sp´ecifique du CAC40 ind´ependante des fac-
teurs ´etudi´es.
Ces param`etres permettent de quantifier la d´ependance du march´e fran¸cais aux
facteurs europ´eens et de mieux comprendre les sources de risque syst´ematique.
D´efinition des donn´ees
Pour estimer le mod`ele, nous utilisons les indices suivants :
• CAC40 : indice fran¸cais, repr´esentant le march´e national.
• STOXX50 : indice paneurop´een, repr´esentant le march´e europ´een global.
• DAX : indice allemand, repr´esentant le cœur industriel europ´een.
Les donn´ees sont collect´ees sur une p´eriode d´etermin´ee du 02 Janvier 2023
au 31 Janvier 2025 avec une fr´equence quotidienne .
Calcul des rendements
Les indices sont transform´es en rendements logarithmiques pour obtenir des
s´eries plus stationnaires et adapt´ees `a l’estimation ´econom´etrique :
Rcac(t) = ln Pcac (t)
Pcac (t−1)
Rstoxx(t) = ln Pstoxx (t)
Pstoxx (t−1)
Rdax(t) = ln Pdax (t)
Pdax (t−1)
o`u Pt est le prix de clˆoture de l’indice `a la date t.
2
Interpr´etation des r´esultats
Avant l’estimation, une analyse exploratoire est r´ealis´ee :
• Corr´elations entre Rcac(t)),Rstoxx(t) est 0,9498 et Rdax(t) est 0,8620
Cette ´etape permet de d´etecter les tendances, anomalies ou relations fortes entre
les variables avant l’estimation du mod`ele.
• β1 = 1,135748 est ´elev´e signifie que le CAC40 est fortement influenc´e par
le march´e europ´een global.
• β2= - 0,237733 signifie que CAC40 et DAX ´evoluent en sens oppos´e.
• α= - 0, 015343 , r´ev`ele une performance propre du CAC40 ind´ependante
des facteurs ´etudi´es.
On obtient alors comme mod´ele :
Rcac(t) =−0.015343 + 1.135748 Rstoxx(t)−0.237733 Rdax(t) + εt
Ajustement du mod´ele R2
Le coefficient de d´etermination R2 mesure la proportion de la variance des ren-
dements du CAC40 expliqu´ee par le mod`ele, ici on obtient R2= 0, 9091. omme
le R2 est proche de 1 on peut conclure que mod`ele est tr`es explicatif.
Analyse du premier graphe : Rendements journaliers du CAC 40 et
du DAX
Description
Le premier graphique repr´esente l’´evolution des rendements journaliers de deux
indices boursiers majeurs : sur la p´eriode allant de janvier 2023 `a d´ebut 2025.
Les rendements sont exprim´es en pourcentage et oscillent autour de z´ero.
3
Figure 1:
Figure 2:
4
Analyse statistique
On observe que les deux s´eries pr´esentent :
• une moyenne proche de z´ero, ce qui est coh´erent avec l’hypoth`ese classique
en finance selon laquelle les rendements journaliers n’ont pas de tendance
d´eterministe ;
• une volatilit´e ´elev´ee, caract´eris´ee par de fortes fluctuations quotidiennes.
Des rendements extrˆemes sont visibles, notamment autour de l’ann´ee 2024, avec
des valeurs atteignant ou d´epassant ±3%, ce qui traduit des ´episodes de forte
instabilit´e des march´es.
Analyse ´economique
Les deux courbes ´evoluent tr`es souvent dans le mˆeme sens, ce qui sugg`ere une
corr´elation ´elev´ee entre le CAC 40 et le DAX. Cette similarit´e s’explique par :
• l’int´egration ´economique des march´es europ´eens,
• l’exposition commune aux mˆemes facteurs macro´economiques (politique
mon´etaire, inflation, tensions g´eopolitiques).
Interpr´etation
Cette forte d´ependance implique que la diversification entre ces deux indices est
limit´ee, car les chocs affectent simultan´ement les deux march´es.
Analyse du second graphe : Rendements journaliers du
CAC 40 et du STOXX Europe
Description
Le second graphique pr´esente les rendements journaliers du : CAC 40, STOXX
Europe, sur la mˆeme p´eriode d’´etude. Le STOXX Europe regroupe un ensemble
plus large de march´es europ´eens, ce qui permet une comparaison `a une ´echelle
continentale.
Analyse statistique
Les rendements des deux indices restent centr´es autour de z´ero, confirmant
l’absence de tendance journali`ere marqu´ee. Cependant, la s´erie du STOXX
Europe pr´esente :
• une volatilit´e plus importante que celle du CAC 40 ;
• des fluctuations plus extrˆemes, avec des chutes pouvant atteindre−4% `a
−5% sur certaines journ´ees.
5
Figure 3: Valeurs des p-values
Analyse ´economique
La plus forte volatilit´e du STOXX Europe s’explique par :
• sa diversification g´eographique, qui l’expose `a un plus grand nombre de
risques nationaux ;
• une sensibilit´e accrue aux chocs ´economiques globaux affectant l’ensemble
de la zone europ´eenne.
Interpr´etation
Le STOXX Europe refl`ete davantage le risque syst´emique europ´een, tandis que
le CAC 40 apparaˆıt l´eg`erement moins volatil car concentr´e sur les grandes en-
treprises fran¸caises.
Test de validation
Pouur le α on suppose comme test d’hypoth`eses:
H0: α = 0,015343
H1: α ̸= 0,015343 On a un p-value = 0,11 largement sup´erieur `a 0,05 . Donc
on rejette l’hypoth`ese nulle.
Pouur le β1 on suppose comme test d’hypoth`eses:
H0: β1 =1.135748
H1 : β1 ̸=1.135748 On a un p-value = 0,0000 largement inf´erieur `a 0,05.
Donc on occepte l’hypoth`ese nulle.
Pouur le β2 on suppose comme test d’hypoth`eses:
H0: β2 = 0.237733
H1: β1 ̸= 0.237733 On a un p-value = 2,309.10−14 largement inf´erieur `a 0,05.
Donc on occepte l’hypoth`ese nulle.
6
Pour les param`etres conjointes: tous les param`etres ont les valeurs list´ees
pr´ec´edamment contre l’hypoth`eses inverse.
On a un p-value quasiment nul donc inf´erieur `a 0,05.
Donnc on accepte l’hypoth`ese nulle, donc le mod`ele est valide.
Conclusion
Le projet permet de quantifier la sensibilit´e du CAC40 aux march´es europ´eens et
de mesurer l’impact relatif du STOXX50 et du DAX. Le mod`ele multifactoriel
montre que le march´e fran¸cais est fortement d´ependant du march´e europ´een
global et de l’´economie allemande, tout en identifiant la performance propre de
l’indice. Les limites de l’´etude concernent notamment la p´eriode analys´ee et le
choix des facteurs. Les perspectives futures incluent l’ajout d’autres facteurs
macro´economiques et l’extension de la p´eriode d’´etude.
References
[1] J. C. Hull, Options, Futures and Other Derivatives, 10e ´edition, Pearson
Education, 2018.
[2] E. F. Fama, “Efficient Capital Markets: A Review of Theory and Empirical
Work”, The Journal of Finance, vol. 25, no. 2, pp. 383–417, 1970.
[3] R. Cont, “Empirical Properties of Asset Returns: Stylized Facts and Sta-
tistical Issues”
