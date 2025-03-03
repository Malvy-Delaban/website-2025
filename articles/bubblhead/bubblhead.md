Title: "Bubbl'Head"
Tags: "3D" render, "Game Jam" game, "Casual" genre, "Team Project" team
=====
# About Bubbl'Head
Bubbl'Head is a casual couch game where you need to push your opponent out of the arena. It is a fast paced 2 player game with controllers on PC. It currently has two different maps and four different skins for players.
It is the result of the 2025 Global Game Jam with the theme "bubble". We started jaming on the friday night and ended the sunday afternoon, about 48h of jamming.

# Team
The project was made by 7 people that were studying at the time at ESMA Toulouse in different sections. We were five last year students in game design, two first year students in game design and one fourth year student in animation. 
The members are the following :


<a href="https://remyalmar.github.io/Portfolio/">ALMAR Rémy - Developer</a>
<a href="https://www.linkedin.com/in/alexis-alves-de-matos-852b05252/">ALVES DE MATOS Alexis - Rig / Animator</a>
<a href="https://itch.io/profile/axel-mariotte">MARIOTTE Axel - Game Designer / Level Designer</a>
<a href="https://itch.io/profile/tsukyart">MOSTEFA Nora - Concept Artist / 3D Artist</a>
<a href="https://www.artstation.com/thrayn">RAMOND Thomas - Tech Artist / Developer</a>
<a href="https://www.artstation.com/nealyth">WEBER Ophéline -  Concept Artist / 3D Artist</a>
<a href="https://www.malvy-delaban.fr/">DELABAN Malvy - 3D Artist / UIs</a>

# Development
The real challenge on this project was to create a local multiplayer game. We took a large amount of time on this weekend making the multiplayer work. The Art direction was also a big issue as we didn't know how to create something that was simple enough to do it in a single weekend. In the end, we took the Art direction and stylization of Boomerang Fu since it had the same vibe that we wanted to create as you can see in the screenshots below. By the end of the weekend, we had something that matched the game we wanted to make. It has some obvious bugs and a bad user exeperience overall but its playable and a bit fun.

!!!
(boomerang-fu.png) Boomerang Fu - Cranky Watermelon
(screen1.png) First map of Bubbl'Head
!!!

# My role - The logo
In this project, I wanted to make sure the game didn't have this clunky feeling of a game jam game. At least, the less clunky as possible. For me, a good logo (or not just the title in an already existing font) is the key to create an appealing project at first sight. I started the jam by making the logo as the concept artists were still struggling to find the art direction and the "theme" of the game. Indeed, they had already decided that we would play as a bubble with an animal hat and the frog hat was the first one to be created. As we were all really existing about this idea, I used it in the logo that I created to be very "family friendly" looking with bright and saturated colors and round shapes (I used an existing typo that I modified a lot to make it smoother).

!!!
(frog.png) First concept by Ophéline WEBER
(logo.png) Logo of Bubbl'Head
!!!

# My role - The map
As we were struggling with the multiplayer, the team moral was pretty low at the time and we ended the first day being very demotivated. I took the initiative to stay longer alongside our animator to create a map as fast as possible to help the team project themself in the game in the hope it could cheer them up.

To do so, I started by adapting the blockout of the map, this part was pretty quick as our level designer worked hard on it beforehand. Next, I modelled the map on itself to make its organic shape and textured it as well. Then I created the passive blockers of the map (aka the rock formations) and replaced the blockout primitive shapes with those, I make 3 variations of the 3D model and textured them. As it felt a bit lifeless, I tried to see on "competitors" game, what did they use to make empty spaces more interesting. The idea that made the more sense for our island was those patches of sand that we can see everywhere on Boomerang Fu. I could have made modifications in the texture of the map but decided to make those "decals" to be able to modify them in engine and most importantly making it not map-dependant to create more maps. Those are basics shapes I created in Adobe Illustrator and exported them as png black and white masks.

!!!
(step1.png) Base map
(step2.png) Rocks and decals
!!!

# My role - Decorating the map
The map was almost ready but it lacked decorations. I imported the moai model that Ophéline WEBER made and completed with a buch of different props such as boxes, amphoras and bushes. To be coherent with the Art Direction of Boomerang Fu, I took their way of making bushes. It is basically just a bunch of flat colored leaves on a png that I created on Procreate and then applied on a fbx consisting multiple planes.

I added a bunch of scaled up rocks further in the sea to make the background. 
At this point, the map was satisfying enough for the project so I made another one with the same props and called it a day.
When I came back in the morning after getting some rest, I saw that the maps had the expected effect on the team as they were all really happy to find the game beginging to take shape. They created some other props for the map such as the palm trees and we focused on the implementation of developped feature for the remaining time.

!!!
(bushes.png) Bushes and props
(decals.png) Decals
!!!

# Play Bubbl'Head
You can find instructions on how to play and the exec of the game on Itch.io.
You will need two controllers and the mouse for the UIs.

???
(itchio) https://malvy-delaban.itch.io/bubblhead
(github) https://github.com/ThraynRmd/GameJamBubules
???