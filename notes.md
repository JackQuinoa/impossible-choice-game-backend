# game has many scenarios
# scenarios has many options 
# game has a time completed if beaten and a username to accompany leaderboard spot

#player model
- username:string

#game model
- completed:boolean 

#scenarios model
- img_src:string

#choices model
- choice: text

#leaderboard model
-time_completed:integer
-username:string

game has_many scenarios
scenarios belongs_to game, has_many options
options belongs_to scenario 