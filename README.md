# riot-app
## Jungle Analytics
(naming in progress)

# What
	This app will use the Riot’s API to collect data on a jungle player's first clear (for the purposes of this app a clear is a full clear meaning all six camps). More specifically it will collect clear time, region, champion, rank, skill upgrade order, camp clear order, primary and secondary keystones (or whatever rune data I'm allowed to get),  patch, and player id. Outside of the game ALL players can look at this data in two main ways. One, average clear time based on filters the player picks (For example, a player can filter to have only NA, Amumu players, who are between Gold and Diamond, on current patch). IMPORTANT NOTE: Although this is a tool I want all people to have access to for the continued improvement of the community there will be a feature integrated with the first where a player can put in their player id and have their average time compared to the communities average time, this is limited to active users as I cant collect that data for those who do not have the app. The second feature is a clear time table showing the fastest clears on each champion, this can also be filtered by the user, the goal of this is to show just how fast each champion can clear and to push the community further. These are the two that I currently envision, but I do want to reserve the right to add more visualizations in the future so long as they don't have a leaderboard or rank system and I wont collect data I am not allowed to.
# Where
	The initial plan of this app was to have it be exclusively for the practice tool. However, it seems as though riot does not support that so it will now be built for normal draft games. I am limiting it to normal draft for competitive integrity. Although I will not include any ranking system, the sheer act of quantifying information and allowing people to see it will push them to be more competitive. In the “How” section it can be seen what actions will disqualify a run but, sometimes these are the right actions to take in a game and I don't want players to not do them or throw over some silly number collection app.
# How
	Here is a step by step of how the Riot API will be used in this app:
Find when a game is started
Find the game type
Find if the player with the app is playing jungle
Find the players name, champion, runes, region and other relevant data detailed earlier
On loading into the game ensure the player clears all 6 of their own camps without engaging in any player combat, counter jungling, or using a non smite summoner spell (this is why it wouldn't be allowed in ranked)
Log data into sql db and stop any kind of tracking 


