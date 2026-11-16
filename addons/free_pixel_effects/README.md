# Free Pixel Effects

30 one-shot pixel art effects for Godot 4: 12 explosions, 10 hit sparks and 8 magic bursts, from 16 to 64 px. CC0.

## Use one

1. From the Asset Library it lands in `addons/free_pixel_effects/`. From a zip, copy the `free_pixel_effects` folder anywhere in your project.
2. Add an AnimatedSprite2D and drag an effect's `.tres` onto its Sprite Frames.
3. Call `play()` (or turn on Autoplay). It plays once at the sheet's speed.
4. To remove it when it's done, connect `animation_finished` to `queue_free`.
5. Set Texture Filter to Nearest so the pixels stay sharp.

The hit sparks end on an empty frame. The explosions and magic fade to a few wisps on the last frame, so free the sprite when the animation finishes.

Each effect is a PNG sprite sheet (one row, transparent background) with a JSON file (frame size, frame count, fps, each frame's position and the palette) and a Godot SpriteFrames file (`.tres`) next to it. They load and play in Godot 4.3, 4.5 and 4.7.

## Colors

Six palettes: fire, gold, toxic, frost, arcane and white. The hex values are in each JSON file under `palette`.

## How they were made

They're drawn by code with Puff, a pixel effect generator (https://cs5475.itch.io/puff). The code was written with help from AI; no image-generation AI made the pictures.

## Want the rest?

These 30 are free for good. The same style runs to 54 battle effects (slashes, projectiles, spells, heals, buffs and debuffs, portals, explosions) at 32, 48 and 64 px, each with a Godot SpriteFrames file, in the paid Complete Collection on itch.io: https://cs5475.itch.io/pixel-battle-effects-complete
