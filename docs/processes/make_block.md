# How to create a new block for the Game

## Drag the "Base_Block" prefab into any scene

It is located in the folder "MyAssets/prefabs/Base_Block".

You can use any scene for this as by the end you will delete 

The base block has the BlockManager component attached to it. With it, you can set up the health points of the block as well as whether or not the block is immune to damage by default.

The BlockManager also holds information how big the block is in **Level Editor Grid Size**. The default block has a size of 1x1, adjust this value based on the size of the sprite/block you wish to implement.

## Assign it a base sprite

Every block is a sprite by nature and as such features a SpriteRenderer component. Drag and drop the sprite you want this new block to use into the Sprite field of the SpriteRenderer component.

## Add block behaviours to your liking

Go into the "MyAssets/Scripts/Game/Block/Effects" folder and add scripts to the prefab that you wish to add.  
Currently there are these block behaviours available:

| Behaviour Name   | Effect                                    | Parameters                |
|------------------|-------------------------------------------|---------------------------|
| Revive           | The block will reappear after destruction | Whether to respawn after ball bounces or time and the amount until respawn |
| Circle Explosion | The block will deal damage to surrounding blocks in a circle area | Amount of damage dealt, radius of explosion |
| Horizontal Line Explosion | The block will deal damage to all blocks on the same horizontal line as itself. | Amount of damage dealt |

Some of these effects also have a type called "ON_DAMAGE", "ON_DESTROYED" or "ON_ALL".
* ON_DAMAGE will trigger the effect whenever the block is hit, but not destroyed.
* ON_DESTROYED will trigger the effect whenever the block is destroyed.
* ON_ALL will trigger the effect whenever the block is hit or destroyed.

## Tweak the parameters to your liking

As mentioned above every behaviour is highly customizable and you're free to adjust the parameters as you wish to design. Should you require new functionality speak to a programmer to add an item to the project backlog.

## Save the new block as a prefab
