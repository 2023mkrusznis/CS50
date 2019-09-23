# Code For Cat Sprite
 To make the cat move and face the direction of the arrow key pressed:
* When Right Arrow Key Pressed
1. Change x by 20
2. Point in Direction 90
* When Left Arrow Key Pressed
1. Change x by -20
2. Point in Direction -90

 To make the game end when the cat touches a droplet:
* When Green Flag clicked
1. Forever
2. If touching droplet or droplet 2 or droplet 3 or droplet 4 or droplet 5
3. Broadcast "Game Over"
4. Stop All

## Code For Droplet Sprites
 To make the drops hide when they touch the ground:
* When I recieve "Start Game"
1. Forever
2. If color 53 is touching color 0 then
3. Hide
4. Else show

 To make drops fall from top of screen continuously:
 * When I recieve 'Start Game"
 1. Go to x: pick random from -240 to 240 y:250
 2. Glide 4 seconds to x: x position y:-250
 3. Forever
 4. Wait .2 seconds
 5. Create clone of myself
 6. Go to x: pick random from -240 to 240 y:250
 7. Glide 4 seconds to x: x position y:-250
 
  To make drops stop their scripts when touching cat sprite:
  * When Green Flag clicked
  1. If touching cat then
  2. Broadcast "game over"
  3. Stop all
  
  ### Code For Counter
   To make counter change by 1 when round of drops hit the ground:
  * When I recieve "start game"
  1. Count 1
  
   To define block "count 1"
  1. Set rounds passed to 0
  2. Forever
  3. Wait 4 seconds
  4. Change Rounds passed by 1
