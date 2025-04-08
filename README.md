Matt Miller 5min Wick test strategy

Code moi la « Matt Miller Wick test strategy” suivante pour LONG et SHORT en pinescript v6. Les paramètres de la stratégie sont initial_capital=20000, default_qty_type=strategy.fixed, default_qty_value=1, margin_long = 0 , margin_short = 0

Les règles sont les suivantes :
1.	Une bougie ayant une wick est formée (bougie 1).
2.	La bougie suivante (bougie 2) fait une expansion dans le même sens que la wick. La bougie 2 a une taille d’au-moins 1.5X la première (low-to-high). La bougie 2 a un corps important (au moins 70% de la bougie)
3.	Pour un trade LONG, la mèche haute de la bougie 1 doit exister. La mèche basse de la bougie 1 n’a pas d’importance. Inversement, pour un trade SHORT, la mèche basse de la bougie 1 doit exister. La mèche haute de la bougie 1 n’a pas d’importance.
4.	Ordre Limit placé au niveau de la wick. 
Sens du trade: direction de l’expansion de la bougie 2
Target: 10 handles
5.	Stop Loss pour un trade LONG: sous le plus bas low entre bougie 1 et bougie 2 - 1 tick
Stop Loss pour un trade SHORT: au-dessus du plus haut high entre bougie 1 et bougie 2 + 1 tick
6.	L’ordre est placé lors de l’ouverture de la bougie 3 (c’est-à-dire à la clôture de la bougie 2).
7.	Si à l’ouverture de la bougie 4 (c’est-à-dire à la clôture de la bougie 3), la position n’est toujours pas ouverte, annuler l’ordre.
8.	Il ne peut y avoir qu’un seul trade en cours.
9.	Afficher sur le graphique quand un ordre est placé.
10.	Afficher sur le graphique quand un ordre est annulé


Configuration de base
![image](https://github.com/user-attachments/assets/8feffa5b-175c-4c9f-892a-25421efa315a)

Short Backtest
![image](https://github.com/user-attachments/assets/c8f68505-3c01-468f-b065-1c7f1bd2bd45)

Long Term Backtesting
![image](https://github.com/user-attachments/assets/61014497-b256-4f3e-9541-59ff084b37ed)



Configuration TP37 et SL 10
![image](https://github.com/user-attachments/assets/f425dede-3909-4613-83df-966f0d134f76)

Court term très bon en profit factor
![image](https://github.com/user-attachments/assets/a63c400c-7113-419e-934c-b8c207b66e0a)

Mais en long term ça ne paye pas
![image](https://github.com/user-attachments/assets/cc279bb7-5552-46a0-bab5-667ca8b65c1b)




