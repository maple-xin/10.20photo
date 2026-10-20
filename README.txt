SIX POKEMON PIXEL ANIMATION SET

For Loopit upload TWO main files: pokemon-pixel-atlas.png + pokemon-pixel-atlas.json.
The root atlas contains all six characters: Pikachu, Charizard, Eevee, Gengar, Snorlax, Mewtwo.
There are 384 frames, 48 directional animations, and 64 frames per character.
Frames are 64x64 for Pikachu, Eevee, Gengar, Snorlax, and 128x128 for Charizard and Mewtwo.
Combined atlas is 2048x1536. Background is transparent; alpha is binary.
Each character also has its own atlas and JSON in its folder: 512x512 small / 1024x1024 large.

Animation names: character_action_direction, e.g. eevee_walk_left.
Actions: idle, walk. Directions: down (front), left, right, up (back).
Each action/direction has eight sampled frames. Follow animationSettings for original clip timings.
The GIF is a simultaneous 8fps overview. preview.html uses each character's actual timing.

IMPORTANT: Place characters using characters[name].anchor (normalized) or groundAnchorPixels.
Anchors differ because long tails and wings need different framing. The anchor is fixed across every frame of a character.
Do not trim/recenter frames. Disable smoothing and use integer pixel scaling.
Movement is separate map logic; walk loops are rendered in place.
These are pixelized renders from 3D models, rather than hand-drawn replacement sprites.
Keep preview.html next to the combined PNG to preview locally in a browser.
loopit-prompt.txt contains the first English import prompt.

Source collection: https://github.com/06wj/pokemon
Original GLBs: https://06wj.github.io/pokemon/models/{pokedex-number}/model.glb
Pokedex numbers: Pikachu 025, Charizard 006, Eevee 133, Gengar 094, Snorlax 143, Mewtwo 150.
The repository MIT software license does not grant Pokemon character or model asset rights.
Conversion does not change source permissions. Related rights remain with their respective owners.
