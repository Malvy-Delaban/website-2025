Title: "Procedural Map"
Tags: "Web" render, "Concept" game, "Procedural" genre, "Solo Project" team
=====
# About the Procedural Map
This project was a personal challenge I've worked on during a weekend back in 2022. It is a solo project were my goal was to create a procedural and customizable voxel map. The challenge here was to make it usable on navigator. To do so, I used the library "Threejs". The big issue here, is that it rely only on the capicity of the client computer as there is no back-end supporting the site, only a front-end.
You can try the project yourself right now without any download by clicking the link at the bottom of this article.

# How does it work ?
The map is generated using a perlin noise. In fact, the parameter you can change in the right of the site are modifying how the perlin noise is interpreted. The map size will change the width and length of the voxel map (the number of squares for a side). The map variation will change the scale of the taken part ofthe perlin noise, therefor, changing the "scale" of the map while keeping the same voxel size. Finally, the height amplifier simply changes the height variation of the map making it rather flat or very vertical. The seed is changed randomly at each generation.

!!!
(height_low.png) A map with low height
(height_high.png) The same parameters with higher height
!!!

# The map creation
For each voxel, I create a mesh corresponding to the height of the given perlin noise at that point multiplied by the height amplifier. Each mesh (rectangle) is creating manually by placing the 8 vertices in the 3D space and then creating each triangle composing the faces. When created, the mesh is given a material depending on the height. Blue for lower values, then yellow, green and white for the highest.

# Issues I'd fix
This project being a timed challenge, I took decisions without thinking much and ended up with some things I would do differently if I had to work on this project again.

Firstly, making the calculation back-end sided would reduce the client load and making it faster and not client device dependent. As for now, a lot of CPU is used on larger map (with a high value in the map size parameter). In a second time, as it was my first "3D project", I didn't know much about materials and for each mesh, a dedicated material is created. As I do not use gradient, this feature is useless and costs performances. It would have been better to use premade materials (they would have been only 4 of them) and use them on multiple meshes.

!!!
(low_performances.png) A map that is cheap to render
(high_performances.png) A map that uses a lot of CPU
!!!

???
(web) https://map.malvy-delaban.fr
???