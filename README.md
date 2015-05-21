# pygame_spritesheets
Handling spritesheets in pygame in a easy way.

### Here is a quick example on how you would use this

```python
import spritesheet

ss = spritesheet.Spritesheet('somespritesheet.png')

# Sprite is 16x16 pixels at location 0,0 in the file...
image = ss.image_at((0, 0, 16, 16))
images = []

# Load two images into an array, their transparent bit is (255, 255, 255)
images = ss.images_at((0, 0, 16, 16),(17, 0, 16,16), colorkey=(255, 255, 255))
```