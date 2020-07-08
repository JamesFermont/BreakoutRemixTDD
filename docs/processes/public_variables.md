# Public Variables

These are the variables that can be modified to change aspects of the game for balancing purposes.

## Ball Prefab

### Ball Behaviour Component

| Param | Effect |
|-------|--------|
| Base Speed | Affects the velocity of the ball at the start of a round |
| Paddle Speed Increase Increment | If the mode is activated, the speed of the ball will increase by this amount when it collides with the paddle. |
| Deflection Strength | The range of motion that the paddle can deflect the ball on collision. |

## Data Pack Prefab

### Data Pack Component

| Param | Effect |
|-------|--------|
| Fall Speed | The velocity with which the data packet drops down after its creation. |
| Energy Given | The amount of energy the data packet gives when collected by the paddle. |

## Level Manager Prefab

### Score Modifiers Component

| Param | Effect |
|-------|--------|
| Score For Perfect Game | The amount of score awarded for completing a level without losing a ball. |
| Penalty For Dropped Ball | The amount of score deducted for losing a ball. |
| Seconds Per Time Mod Interval | The amount of difference in seconds between time spent and target time to change the time score modifier by + or - 0.1 |
| Min Time Mod | The lowest possible time score multiplier value |
| Max Time Mod | The highest possible time score multiplier value |

## Block Components

### Block Manager

| Param | Effect |
|-------|--------|
| Max Health | The number of hits the block takes before being destroyed |
| is Immune | The block will not take damage if this is set |
| Score on Destroy | This number is added to the player score when the block is destroyed |
| Dp Base Chance | The chance in % with which a Data Packet will drop |
| Dp Base Chance Increment | The base chance will increase by that amount for every block destroyed that didn't drop a packet since the last drop. |

### Circle Explosion Component

| Param | Effect |
|-------|--------|
| Effect Type | Determines whether or not the effect happens when the block is hit or destroyed (or both) |
| Explosion Radius | The Radius in unity units that the circle explodes around. |
| Explosion Damage | The amount of damage

### Revive Block Components

| Param | Effect |
|-------|--------|
| Revive Count Min | The minimum amount of seconds until the block revives |
| Revive Count Max | The maximum amount of seconds until the block revives |
| Revive Hp Amount | The amount of health the block revives with. |
