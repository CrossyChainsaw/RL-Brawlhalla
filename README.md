# RL-Brawlhalla
(wip) Reinforcement Learning Agent trained to play the game Brawlhalla

# **----- THIS IS AN OFFLINE EXECUTED PROJECT -----**

ideally we figure out how to extract game variables out of the game and manage to monitor them. Next, we can start with Reinforcement Learning.

steps
- Define States 
- Define Actions
- Define Rewards

### States
for states i was thinking about taking p1 coordinates and p2 coordinates and return the vector between them. also the map position. And an array with platform positions which will be empty if there are no platforms. so it would look something like

[map_pos_x_min, map_pos_x_max, map_pos_y_min, map_pos_y_max, [platform_positions], (x, y, .z)]

the map can also be hardcoded sp that we dont need it in the code, since if you already know which map you play its unnecessary.

### Actions
for actions you bind a number to an action for example.
0 - Jump
1 - Right
2 - Left
3 - Light
etc.

to learn, it will use a random action on each state, slowly it should learn what is good and bad based of rewards.

### Rewards
