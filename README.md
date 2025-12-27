# Component 3 Manual
This manual will explain how the component works and how it will be used in the final prototype

## Spawner
The enemy spawner on the right hand side of the screen moves up and down the screen and instantiates enemies on a random interval timer. This is to make the player unaware of the spawn habits of the enemies. The code used to move the spawner is a translation that changes from a positive y value to a negative y value when the spawner hits one of the objects at the top or bottom of the screen.

## Enemies
The enemies that are spawned in move on a similar script to that of the bullet from component 2, moving constantly by their own script. However, once the enemy hits an invisible wall near the middle of the screen, they stop moving. This is so that the player can position themselves to shoot them.

## Limit
There is a limit in place so that only 5 enemies can be on screen at a time. This is achieved by adding each instantiated enemy to a list and then stopping the instatiations once there are 5 items in the list.

## Implementation
In the final prototype, the enemies will be shooting at the player on the same line as where they spawned. Once they are killed, they will be removed from the list so that the spawner has the ability to spawn another enemy. The spawner will always be present and won't be killable by the enemy. There will be 2 sets of spawners and invisible walls based on the camera positions that the levels will be set in.
