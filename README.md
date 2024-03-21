# Procedural Terrain Generation in Godot

This project demonstrates procedural terrain generation in the Godot game engine using a 3D grid map and the FastNoiseLite library for noise generation.

![Preview](https://github.com/alpapaydin/Godot4-3D-Procedural-World-Generation/blob/master/preview.png?raw=true)

## Features

- **Procedural Terrain Generation**: The terrain is generated procedurally using Perlin noise. This means that the terrain is different every time you run the game, but remains consistent across play sessions if you use the same seed.
- **Chunk-Based Loading/Unloading**: The terrain is divided into chunks, and only the chunks within a certain distance of the player are loaded. This helps to reduce memory usage and improve performance.
- **Different Terrain Types**: The terrain includes different types of blocks, including dirt, rock, sand, and water, which are placed according to the noise values.

## How to Use

1. **Adjust the Terrain Parameters**: You can adjust the size and shape of the terrain by changing the `map_width`, `map_depth`, `water_level`, and `chunk_size` variables in the `GridMap.gd` script. You can also change the `seed` values for the `terrain_noise` and `stone_noise` to generate different terrains.
2. **Run the Game**: Run the game in the Godot editor. You should see a 3D terrain generated around the player.
3. **Move the Player**: Move the player around the terrain. As you move, new chunks of terrain will be generated in front of you, and old chunks that are too far away will be unloaded.

## Limitations

- The terrain is currently only generated in the horizontal plane, and doesn't include any caves or overhangs.
- The terrain generation is quite basic and doesn't include any biomes or complex features.
- There is currently no saving or loading of the terrain, so you will start with a new terrain every time you run the game.

## Future Improvements

- Add more types of terrain blocks, such as grass, trees, and ores.
- Implement biomes, so that different types of terrain (e.g. forests, deserts, mountains) can appear in different areas.
- Add saving and loading of the terrain, so that players can continue where they left off.
- Implement caves and overhangs in the terrain.
- Improve the performance of the terrain generation and loading/unloading.
