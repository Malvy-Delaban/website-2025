Title: "Procedural Map"
Tags: "Web" render, "Concept" game, "Procedural" genre, "Solo Project" team
=====
# About the Procedural Map
Procedural Map is a personal challenge I embarked on during a weekend in 2022. The project was created as a solo endeavor, with the goal of building a procedural and customizable voxel map that could be run directly in a web browser. The key challenge was ensuring that it would work purely on the client-side, without relying on any back-end infrastructure. For this, I used the popular JavaScript library Three.js.

The map generation is entirely dependent on the performance of the client device, as there is no server-side support. This means that users with more powerful devices will have a smoother experience, especially when generating larger maps.

You can try the project yourself right now, with no downloads required, by clicking the link at the bottom of this article.

# How does it work ?
The map is generated using Perlin Noise, a gradient noise function commonly used for procedural content. The parameters on the right side of the website allow you to modify how the noise is interpreted and displayed. Here's a breakdown of the controls:

• Map Size: Adjusts the width and length of the voxel map (i.e., the number of squares on each side).
• Map Variation: Changes the scale of the Perlin noise used, modifying the overall "scale" of the terrain while keeping the same voxel size.
• Height Amplifier: Alters the verticality of the terrain, making it flatter or more mountainous.

Each time you generate the map, the seed is randomized, resulting in a new variation of the terrain.

!!!
(height_low.png) A map with low height
(height_high.png) The same parameters with higher height
!!!

# The map creation
To create the map, I generate a mesh for each voxel based on the Perlin noise value at each point. The height of each voxel is determined by the Perlin noise value, multiplied by the height amplifier. Each mesh is made by manually placing 8 vertices in 3D space and constructing triangles to form the faces.

Each mesh is then assigned a material that corresponds to its height:

• Blue for lower values
• Yellow and green for medium values
• White for higher values

This process allows for a dynamic, visually rich map that changes based on the parameters you set.

# Issues I'd fix
As this was a timed challenge, there were some decisions made that I would change if I had more time:

1. Server-Side Calculations: Moving the heavy calculations to a server-side back-end would reduce the client load and improve performance, especially for larger maps. As it stands, the map size directly impacts CPU usage, which can be a bottleneck on less powerful devices.

2. Material Optimization: Since this was my first 3D project, I didn't know much about materials in Three.js. For each mesh, I created a unique material, which, while visually appealing, negatively impacted performance. In hindsight, it would have been better to use just four premade materials and apply them across multiple meshes, avoiding unnecessary material creation.

!!!
(low_performances.png) Low Performance Map
(high_performances.png) High Performance Map
!!!

# Play the Procedural Map
Feel free to explore the project by visiting the link below. No downloads are needed—just click and start generating your own procedural maps!

???
(web) https://map.malvy-delaban.fr
???