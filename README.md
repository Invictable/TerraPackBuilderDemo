# TerraPackBuilder Demo
Basic overview of how my terrain generator works and the results it produces. (developed for Hoplite)

Hoplite utilzies an open source terrain generator, adapted to create ideal UHC worlds. One of the inputs this terrain generator can accept for creating worlds is images, so I created TerraPackBuilder to create images that include key features of UHC style worlds and Minecraft style terrain easily.

Two types of maps can be generated, Solo or Civilization style.

Both maps are created as islands, with ocean surrounding the playable land. Rivers cut through the land, but avoid mountains.
Solo maps features a biome at the center of the map that can never have caves, and feature small biome regions throughout the map of all types.
Civilization maps are split into 10 regions and generated so all 10 teams have equally proportioned regions.
Biome regions are generated using a randomized upscaling algorithm. Biome borders are also generated this way, allowing randomized biome and region borders that feel natural.

These images are regenerated at the start of every Hoplite season, allowing a new set of image templates to exist. Each colored pixel correlates to a set of biomes everytime the map generates, so even if a player recognizes the map template from river shapes or some other unchanging landmark, the exact biome in specific places will be different. Addtionally, the shape terrain takes is affected by the vanilla seed, so caves, ores, landmarks, etc will also be different even when playing on the same map template. 

Maps are continously generated and deleted once played to make sure players never play on the same 100% identical map twice. Only templates are reused. 

Example map template created by the program:
![image](https://github.com/user-attachments/assets/19909ff2-7109-48dd-948b-800f14dcdbf3)

Example map generated ingame via this template:
![mapfull](https://github.com/user-attachments/assets/e318b830-5fab-47ee-a2c6-9d24b6ecba6e)

Here's an example of a civ map template along multiple stages of generation:

![TenShapes-0711-1508-2275](https://github.com/user-attachments/assets/ac31e8b6-bdcf-4be3-8a33-2c23a781739b)
![TenShapes-0711-1515-9751](https://github.com/user-attachments/assets/040c029b-0c4b-42c0-9bfa-335dc1627272)
![TenShapes-0711-1516-2930](https://github.com/user-attachments/assets/dc9abd35-c750-4012-b000-602ec15e31ef)
![TenShapes-0711-1516-8091](https://github.com/user-attachments/assets/7cb50b95-9ba8-4acb-a393-1888d6aa275c)




