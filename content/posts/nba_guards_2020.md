---
title: "2019-20 NBA Regular Season Guards Overview"
subtitle: ""
summary: ""
#authors: ["bear5"]
tags: [nba, sports]
categories: []
date: 2020-10-24T17:22:25-05:00
lastmod: 2020-10-24T17:22:25-05:00
featured: false

reading_time: false
commentable: false
profile: false
share: false

draft: false 

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
#image:
 # caption: ""
 # focal_point: ""
 # preview_only: false
---

If I missed a live game I cared about, the next thing I do is checking game stats on Google. A stats sheet tells part of the game story, which player has the most points, the total team rebound, and field goal percentage might justify the game result.The team like Houston Rockets builds its roaster and game strategy heavily relies on data, instead of traditional basketball sense, its success in the past few years not only changed how the league is playing but also shows the power of data.

Following the Lakers won the 2020 NBA champion (Congrats LeBron!), I'll review some advanced data for season 2019-2020. Trying not to be blinded by the normal stats like points/rebounds/assists per game, the series expects to describe players from multiple perspectives and provides data proves that can support or change your opinions. All the data comes from [basketball reference](https://www.basketball-reference.com/)

Let's start with the guards! 

There are 234 guards(both PG and SG) out of total of 529 players. Some guards' playing minutes are too few to produce any meaningful result. I'll filter it out.

The following two figures show the game played and total minutes played distribution for all players of season 2019-2020. For example, there are 60% of player's total playing minutes below 1000 minutes, and 40% of players played less than 500 minutes (which is averaging less than 10 mins per game) for the whole season. 60% of players played less than 50 games, around one-third of players played less than 20 games.

![gp_distribution](/images/nba_guards_2020/nba_2020_gp_guard.png "Player Total Game Played Distribution")

![mp_distribution](/images/nba_guards_2020/nba_2020_mp_guard.png "Player Total Minutes Played Distribution")



Based on games and minutes played distribution, only players with 50 games appearance and a total of 800 minutes (20 minutes per game for 40 games) are under the radar for analysis. 109 guards survived.

NBA advanced stats are the primary data I use for the overview, these stats consider more aspects like the pace of the game, total possessions, and contribution to success instead of just taking average points or rebounds to evaluate a player. The advanced data could be treated as standardized stats like [PER](https://en.wikipedia.org/wiki/Player_efficiency_rating) measures player's per-minute performance, [WS](https://www.basketball-reference.com/about/ws.html) counts players' contribution to team success.

 

Let's see some advanced stats!

[WS](https://www.basketball-reference.com/about/ws.html)

![ws_no_clustering](/images/nba_guards_2020/nba_2020_ws_guard_no_clustering.png)

Each dot in the above figure presents a player with x axis showing the player's offensive win share and y axis presents player's defensive win share. For example, the player with point around (10.5, 0.7), it means this player contributed a total of 11.2 wins to the team, and 10.5 out of 11.2 are contributed by his offense. The player in the left bottom corner (-1.0, 0.0) contributed negative to the team, without who the team can win one more game. Thus the right up corner player with around 10.0 and 3.2 win shares offensively and defensively probably the most important guy to his team. We are going to find out who he is.

![ws](/images/nba_guards_2020/nba_2020_ws_guard.png)

James Harden!

People won't doubt how important James Harden is to the Rockets, but no one will imagine James Harden's defense will add Rockets 3 wins.  The color of the dot presents the clustering result, which basically means which players are more likely to be the same type of players in terms of win shares. The clustering is done on normalized data using KMEAN or GuassianMixture model.  James Harden and Damian Lillard have their own group. Nobody else is comparable with them. There are several groups like Seth Curry, JJ. Redick, Bradley Beal, and Trae Young group presents an overall good offense,  Kyle Lowry, Ben Simmons group have similar offensive win share but contribtues more on the defense side. Group LeBron, Chris Paul, Luka Doncic, and Devin Booker performance better in the offense than the previous group, but far less win shares than James Harden. Here I would argue Devin Booker could be a separate group since his defensive win share is just too low.



[BPM](https://www.basketball-reference.com/about/bpm2.html)

Not everyone's contribution can lead to a win, some players might help the team, but not enough to get a win. We can use Box Plus/Minus(BPM), which is a stats to estimate a player's contribution in points above league average per 100 possessions played.

![bpm](/images/nba_guards_2020/nba_2020_bpm_guard.png)

Luka, Lebron, and James are ine the elite group. Trae, Bradley, Damian, and Kemba are players helping on the offense but have a negative impact on the defense, that's why Miami Heats attacked Kemba in the Eastern Final. Players like Buddy Hield and Devin Booker can learn from Chris Paul, who is also a small size guard, but can contribute defensively. Patrick Beverley has almost zero impact on the offense, but his defense changes the game, interestingly, Ben Simmons, a widely considered next  LeBron, is in the same group as Patrick Beverley, Ben needs to start shooting threes to help more on the offense, instead of just pushing the transitions.



[PER](https://en.wikipedia.org/wiki/Player_efficiency_rating) and [TS%](https://en.wikipedia.org/wiki/True_shooting_percentage)

Player Efficiency Rating(PER) and True Shooting Percentage(TS%) are an all in one number to evaluate a player's contribution and players efficiency in shooting. PER is to measure player's per-minute performance with a league average is 15.0, while TS% takes free-throw and three-point field goal percentage into consideration. Here I use these two stats as an indicator of player's efficiency on the offensive end.

![efficiency](/images/nba_guards_2020/nba_2020_efficiency_guard.png) 

James Harden, no doubt, is in the elite group together with Damian Lillard and Luka. Devin Booker is an elite attacker considering how many shoots he has to take while maintaining such a high TS%.



[Usg%](https://www.nbastuffer.com/analytics101/usage-rate/) and [Tov%](https://www.nbastuffer.com/analytics101/turnover-ratio/)

Besides the efficiency, how heavy the player is involved in the game should also be considered. Usage Percentage generally estimates the team's possessions used by a player (of course while he is on the court), like field goal attempt, shooting foul draw, or turnovers. Turnover percentage just one sub-field of usage percentage.

![usg_tov](/images/nba_guards_2020/nba_2020_usg_tov_guard.png)

James Harden, Trae Young, Russ, Luka and Bradley need the ball at their hand. James and Russ take more than 70% percent of the possessions when they are on court (but considering the time they are both on the court, the actual possessions ended up with them is less than 70%, but still a large number), which matches Rockets game strategy, ISO. Matthew Dellavedova, man, you should take care of the ball.



Tov% vs [Ast%](https://www.nbastuffer.com/analytics101/assist-percentage/)

When talking about turnover, people think about assists, the Assist Percentage estimates teammate field goals assisted by the player.

![tov_ast](/images/nba_guards_2020/nba_2020_ast_tov_guard.png)

Trae, Luka, and Lebron have the highest assist percentage,  they organize the games. Wonder why James Harden is not on the list, take a closer look (sorry I did not organize the text well), James and Russ have similar AST%, which probably means these two together drive the rockets plays, in another word, James shares a portion of his ball to Russ, otherwise, I believe James will have larger than 50% AST%.

Lonzo Ball and Ben Simmons, even though they are good at finding the opportunities, but need to reduce the turnovers.



[REB%](https://en.wikipedia.org/wiki/Rebound_rate)

Last, let's look at rebound rate, showing how effective a player is gaining rebound, offensively and defensively.

![rebounding](/images/nba_guards_2020/nba_2020_rebound_guard.png)

Ben Simmons has the highest offensive rebound rate (I did not really watch his game, thus this kind of new to me). Luka has the highest defensive rebound rate (thus he has so much triple-double), probably due to team strategy, big guys will box out and guards will collect the rebound, one good thing about guards getting defensive rebound is he can start the transition offense right away, Jason Kidd does this a lot. 



After seeing guards' advanced stats in the 2019-2020 seasons. Some takeaways:

1.  Luka Doncic has joined James Harden and LeBron James becoming the best guards right now. Only in his second year!
2. Damian Lillard and James Harden are unstoppable on the offensive end, and surprisingly James Harden is also a good defender!
3. Chris Paul is old, but he is still a top guard, better than Donovan Mitchell
4. Trae Young, Bradley Beal, and Devin Booker are solid in offense but can improve in defense 
5. Ben Simmons is kind of similar to Russell Westbrook,  can enlarge his offensive impact in the game by shooting better.







