# PROJET ECONOMIE FINANCIÈRE 
                                  
                                  
                                  Theme :Analyse de la sensibilité du CAC40
                                 aux marchés européens : un modèle
                                 multifactoriel basé sur le STOXX50 et le DAX
                                             Réalisé par :
                                           Christ J BASSE
                                            Malang CISSE
                                            Doudou MANE
                              M2 PSA Université de Lorraine Metz , UFR MIM
                              
                                           # Introduction


            L’intégration croissante des march´es financiers européens implique une inter-
            d´ependance forte entre les principaux indices boursiers.Le CAC 40, princi-
            pal indice français, est exposé aux dynamiques économiques et financières eu-
            ropéennes, notamment via l’Allemagne première économie de la zone europe
            ainsi que les grands groupes paneuropéens.
            L’objectif de ce projet est d’´evaluer la sensibilité du CAC 40 aux marchés eu-
            ropéens en estimant un mod`ele ´econom´etrique multifactoriel expliquant
            les rendements du CAC 40 par ceux :
            • du STOXX 50, repr´esentant le march´e européen global,
            • du DAX, repr´esentant le noyau industriel allemand.
            Cette approche permet d’identifier les sources du risque systématique du
            marché français.
            
# MODÈLE THÉORIQUE DE REGRESSION LINÉAIRE MULTIPLE 

         Le rendement du CAC 40 à l’instant t, noté Rcac(t), est expliqué par les rende-
         ments de deux indices de marché Rstoxx(t) et Rdax(t) selon le modèle :
         Rcac(t) = α+ β1Rstoxx(t) + β2Rdax(t) + εt, t= 1,...,T (1)
         oÙ :


          • α est une constante r´eelle .
          • β1,β2 sont des coefficients r´e´els de r´egression repr´esentant la sensibilit´e du
            CAC 40 aux indices stoxx et dax.
          • εt est le terme d’erreur, suivant la loi normale centr´e de param´etre :
            E[εt] = 0, Var(εt) = σ2, Cov(εt,εs) = 0 pourt̸= s

# REVUE DE LA LITTERATURE

        Les modèles multifactoriels sont largement utilisés en finance pour expliquer
        les rendements des indices boursiers. Ces mod`eles permettent de distinguer
        les performances propres d’un march´e des effets des facteurs externes. Dans le
        mod`ele utilis´e ici :
• β1 mesure la sensibilit´e du CAC40 au marché européen global (STOXX50),
• β2 mesure la sensibilit´e du CAC40 `a l’économie allemande DAX,
• α représente la performance sp´ecifique du CAC40 indépendante des facteurs étudies.
       Ces paramètres permettent de quantifier la dépendance du marché français aux
       facteurs européens et de mieux comprendre les sources de risque systématique.
       
# Définition des données 

  Pour estimer le modèle, nous utilisons les indices suivants :
• CAC40 : indice fran¸cais, représentant le marché national.
• STOXX50 : indice paneuropéen, représentant le marché européen global.
• DAX : indice allemand, repr´esentant le cœur industriel europ´een.
  Les donn´ees sont collectées sur une période déterminée du 02 Janvier 2023
  au 31 Janvier 2025 avec une fréquence quotidienne .

# Calcul des rendements
  
Les indices sont transformés en rendements logarithmiques pour obtenir des
séries plus stationnaires et adaptées à l’estimation économétrique :
Rcac(t) = ln Pcac (t)
Pcac (t−1)
Rstoxx(t) = ln Pstoxx (t)
Pstoxx (t−1)
Rdax(t) = ln Pdax (t)
Pdax (t−1)
où Pt est le prix de clˆoture de l’indice à la date t.

# Interprétation des résultats

Avant l’estimation, une analyse exploratoire est réalisée :

• Corrélations entre Rcac(t)),Rstoxx(t) est 0,9498 et Rdax(t) est 0,8620
Cette étape permet de d´etecter les tendances, anomalies ou relations fortes entre
les variables avant l’estimation du modèle.
• β1 = 1,135748 est ´elev´e signifie que le CAC40 est fortement influenc´e par
le marché européen global.
• β2= - 0,237733 signifie que CAC40 et DAX ´evoluent en sens oppos´e.
• α= - 0, 015343 , révèle une performance propre du CAC40 indépendante
des facteurs étudiés.



On obtient alors comme modèle :
Rcac(t) =−0.015343 + 1.135748 Rstoxx(t)−0.237733 Rdax(t) + εt
Ajustement du mod´ele R2
Le coefficient de d´etermination R2 mesure la proportion de la variance des ren-
dements du CAC40 expliqu´ee par le modèle, ici on obtient R2= 0, 9091. omme
le R2 est proche de 1 on peut conclure que mod`ele est très explicatif.
Analyse du premier graphe : Rendements journaliers du CAC 40 et
du DAX
Description
Le premier graphique repr´esente l’´evolution des rendements journaliers de deux
indices boursiers majeurs : sur la p´eriode allant de janvier 2023 à début 2025.
Les rendements sont exprim´es en pourcentage et oscillent autour de z´ero.


 # Analyse statistique
 
On observe que les deux séries présentent :
• une moyenne proche de zéro, ce qui est coh´erent avec l’hypoth`ese classique
en finance selon laquelle les rendements journaliers n’ont pas de tendance
d´eterministe ;
• une volatilité élevée, caractérisée par de fortes fluctuations quotidiennes.
Des rendements extrˆemes sont visibles, notamment autour de l’ann´ee 2024, avec
des valeurs atteignant ou d´epassant ±3%, ce qui traduit des ´episodes de forte
instabilité des marchés.
Analyse ´economique
Les deux courbes ´evoluent tr`es souvent dans le mˆeme sens, ce qui sugg`ere une
corr´elation ´elev´ee entre le CAC 40 et le DAX. Cette similarit´e s’explique par :
• l’int´egration ´economique des march´es europ´eens,
• l’exposition commune aux mˆemes facteurs macro´economiques (politique
mon´etaire, inflation, tensions g´eopolitiques).

# Analyse économique

La plus forte volatilit´e du STOXX Europe s’explique par :
• sa diversification g´eographique, qui l’expose `a un plus grand nombre de
risques nationaux ;
• une sensibilit´e accrue aux chocs ´economiques globaux affectant l’ensemble
de la zone europ´eenne.
Interpr´etation
Le STOXX Europe refl`ete davantage le risque syst´emique europ´een, tandis que
le CAC 40 apparaît l´eg`erement moins volatil car concentr´e sur les grandes en-
treprises fran¸caises.

# Test de validation

Pouur le α on suppose comme test d’hypoth`eses:
H0: α = 0,015343
H1: α ̸= 0,015343 On a un p-value = 0,11 largement sup´erieur `a 0,05 . Donc
on rejette l’hypothèse nulle.
Pouur le β1 on suppose comme test d’hypoth`eses:
H0: β1 =1.135748
H1 : β1 ̸=1.135748 On a un p-value = 0,0000 largement inf´erieur `a 0,05.
Donc on occepte l’hypothèse nulle.
Pouur le β2 on suppose comme test d’hypoth`eses:
H0: β2 = 0.237733
H1: β1 ̸= 0.237733 On a un p-value = 2,309.10−14 largement inf´erieur à 0,05.
Donc on occepte l’hypothèse nulle.


 Pour les paramètres conjointes: tous les paramètres ont les valeurs listées
précédamment contre l’hypothèses inverse.
On a un p-value quasiment nul donc inférieur à 0,05.
Donnc on accepte l’hypoth`ese nulle, donc le mod`ele est valide.

# Conclusion

Le projet permet de quantifier la sensibilit´e du CAC40 aux march´es europ´eens et
de mesurer l’impact relatif du STOXX50 et du DAX. Le mod`ele multifactoriel
montre que le march´e fran¸cais est fortement d´ependant du march´e europ´een
global et de l’´economie allemande, tout en identifiant la performance propre de
l’indice. Les limites de l’´etude concernent notamment la p´eriode analys´ee et le
choix des facteurs. Les perspectives futures incluent l’ajout d’autres facteurs
macro´economiques et l’extension de la p´eriode d’´etude.
References
[1] J. C. Hull, Options, Futures and Other Derivatives, 10e édition, Pearson
Education, 2018.
[2] E. F. Fama, “Efficient Capital Markets: A Review of Theory and Empirical
Work”, The Journal of Finance, vol. 25, no. 2, pp. 383–417, 1970.
[3] R. Cont, “Empirical Properties of Asset Returns: Stylized Facts and Sta-
tistical Issues”, Quantitative Finance, vol. 1, no. 2, pp. 223–236, 2001.
   






            
