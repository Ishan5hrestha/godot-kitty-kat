# Kitty Kat Godot Tutorial
Following tutorial at [Link](https://www.youtube.com/watch?v=Luf2Kr5s3BM&ab_channel=Chris%27Tutorials)
## Steps
- Initialize project
- Assets download from `https://cupnooble.itch.io/sprout-lands-asset-pack` and extract the content inside `assets` folder
- Set `Default Texture Filter` to `Nearest` in Canvas Texture. Required to stop anti-aliasing for pixelart
- Created `Node2D` for scene and `CharacterBody2D` for the player
  - Add `Sprite2D` for adding the sprite
  - Add `AnimationPlayer` for the player animation. Create Key frames for animations.
  - Add `AnimationTree` to create state machine and create flows
  - Attach `Script` to the player to create movement and connect to the `Animation Tree`.
    - `Sprite2D` has sprite sheets taken by `AnimationPlayer` to create different action animations
    - `AnimationTree` takes the `AnimationPlayer` takes the different animations created from `Animation Player` and sets different condition on which to show which animation. Condition can be `Vector2D` or others
  - Add `TileMap` to `Node2D` for the scene. One of the scene created must be set a default scene when the game starts
  - Import the tileset and draw on the scene. Set different z-index of the layer and also create bitmap for tiles auto designing.