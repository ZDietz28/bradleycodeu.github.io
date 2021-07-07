---
layout: project
category: turtlegames
title: Turtle Game v4
---
This is NOT a group project

You have tons of freedom with this game. 1 player or 2p co-operative or 2p competitive? Enemies or no enemies? Following enemies or guards or both? Goal or coins or both? Multiple levels or only one level?

You might want to change the controls (or not). You can continue using Turtle controls (rotate left, rotate right, move forward). You could use RPG-style controls so that W changes your y position by +5, S is y - 5, A is x - 5, and D is x + 5.
```python
#option for changing controls
def goLeft():
  player1.goto(player1.xcor() - 8, player1.ycor())
  ```
  You could use platformer controls so that W changes your yvelocity + 5 (makes you jump), A is x - 5, D is x + 5, and if not touching a wall/platform then gravity changes your yvelocity - 0.5.
  ```python
  #option for implementing gravity with a Wall object named ground
  if ground.touching(player1) == False:
    yvelocity += gravity #if not touching ground, gravity changes your yvelocity
  else:
    yvelocity = 0
    player1.goto(player1.xcor(), ground.ycor() + ground.height/2) #move to top of ground
  player1.goto(player1.xcor(), player1.ycor() + yvelocity) #use yvelocity to change y
  ```


The only requirements are the ones listed below:

1.  Create a multi-line comment at the top of you code with you name, date, and directions. Your directions must explain the way to win OR way to make it to the next level. For example... reach the goal without dying OR reach the goal before the other player OR collect more coins than the other player OR collect all of the coins without dying.
1.  Add a new file, name it wall.py, and copy/paste [THIS WALL CLASS FOR TURTLE GAMES](https://gist.githubusercontent.com/ohiofi/079e1080ece5c729931c2bdb71d7ddfa/raw/4a7480aede06e1607fd0b9b9df1c53ddfd3edebf/wall.py) You MUST use the Wall class to create 1 or more walls/platforms
1.  Your player(s) and enemies cannot walk through walls/platforms. You could make the wall just block the player OR make the wall kill the player.
