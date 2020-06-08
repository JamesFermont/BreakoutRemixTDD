# Sprites

## Sizing

This is a list of all GameObjects using sprites and their respective size:

| Object Name  | Native Pixel Size | Asset Size   | Unity Unit Size |
|--------------|-------------------|--------------|-----------------|
| Size 1 Block | 64x40 px          | 256x160 px   | 0.64, 0.40      |
| Ball         | 20x20 px          | 80x80 px     | 0.2, 0.2        |
| Paddle*      | 192x40 px         | 768x160 px   | 1.92, 0.4       |
| Background   | 1280x720 px       | 5120x2880 px | 12.8, 7.2       |

\* The current test paddle sprite is only 20px in height but the game object is 40px in height

### Fitting the scaling

Since we work with 4x native sprites we have to make some adjustments to make them fit the intended game size. When implementing a new sprite, set it's **Pixels per Unit** value from the default __100__ to __400__.
