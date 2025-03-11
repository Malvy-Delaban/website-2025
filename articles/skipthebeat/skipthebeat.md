Title: "Skip The Beat"
Tags: "2D" render, "Full Game" game, "Rythm" genre, "Solo project" team
=====
# About Skip The Beat
This project is the very first "complete" game I created. It was the final project of the first year in game design at ESMA Toulouse. It is a 2 month long project were the goal was to create a 2D platformer. We needed to create the universe, general mood, search for inspirations and create the game from A to Z. This is a solo project.

# Tools
For the musics, I used Soundraw.io to create AI generated songs as I didn't think I could learn music creation in 2 months on top of the development of the game.
For the other parts of Skip The Beat, I used :

• Unity
• Procreate (for concepts arts and illustrations)
• Adobe Illustrator (for the logo)
• Blender (for some 3D meshes I didn't use in the end)

# Concept
Skip The Beat is a 2D platformer and rythm game. The game is simple, in the first part, you have a menuing step in which you choose wich patterns of map you'll play in your level. Each level is associated with a tempo, a difficulty and a part of the music.
The goal is to make a music that is easy enough to beat in the 2D platformer but hard enough to give you some points. On top of that, your creativity is needed to create your own music.
Once the game is finished, if you have succesfully finished the level without it, your song is considered "complete" and you basically won.

@@@https://www.youtube.com/watch?v=xxzNb_dM8TY&ab_channel=MalvyDelaban@@@

# Story
Moky is a music artist who creates electronic tracks. She gained recognition less than a year ago thanks to a successful feature. But since then, she’s been stuck. Not the slightest idea seems to come to her, and she’s starting to doubt herself.

One evening, over a drink, a friend of hers—also in the music scene—tells her about an AI that’s been making waves. It’s called Xochi, an AI that composes music tracks and allows artists to adapt them as they wish.

Curious and with no other options, Moky decides to try out this so-called amazing AI the next day. To her surprise, the tool’s interface is much more playful than expected, and she quickly gets hooked—a rather ironic twist, given that the tool is actually designed to let users play a rhythm game based on the generated music.

!!!
(moky_solo.png) Moky - in game
(xochi_solo.png) Xochi - in game
!!!

# Character design
DJ xochi is a pretty straight forward reinterpretation of Xochipilli, an aztec god that represents passion, love, sexuality, music, arts, playfulness and more. It is often represented with very colorful skin tones or clothes and often with leaf clothes. I added traditionnal Mexico clothes and I mixed it with the modern representation of sexuality through clothes (lingerie) and modern musical accessories such as large golden jewelry to mention a recent musical movement (hip-hop / old school US rap).

Moky on the other hand is exclusively a representation of modern music and in particular, electronic music.
She has a design inspired obviously by the Daft Punk helmets, LED dotted screens, winged helmet to enhance her fast music and hasty personality.

!!!
(Moky.png) Moky
(DJ_Xochi.png) DJ Xochi
!!!
!!!
(research.png) inspirations
!!!

# Ripomatik
In the pre-production phase, I worked on a "ripomatik". This is a video editing of different elements taken from movies, music, images, games to present a general mood of the game / the project without having to create anything. It has a huge power to communicate an artistic intention but can easily lock someone in a particular vision of the project
Here is the ripomatik I made for SkipTheBeat :

@@@https://www.youtube.com/watch?v=xxzNb_dM8TY&ab_channel=MalvyDelaban@@@

# Dynamic Sound interpretation
Even if it can be subtle in game, a lot of work has been made on the dynamic sound-responsive elements in-game. For example, the background in the menus or in game is always rotating and scaling on itself depending on the tempo of the current music playing. This was made using a tool I developped on Unity, allowing me to get a real-time fedback on a scale from 0 to 1 of the music. It can be used to detect bass sounds as well as trebels depending on my needs. It allows me to adapt anything in game based on the music very easily wherever needed.

This tool was based on some of the work of "Peer Play".
@@@https://www.youtube.com/watch?v=4Av788P9stk&t=5s&ab_channel=PeerPlay@@@

# Map generation
The game allows you to create a music composed of existing music parts (around 15s each). You can choose between multiple tempo and place them as you'd like. Once the music being "contructed" (all the parts adjusted as you like), you can validate the music. It then launches the 2D platformer part of the game where the level is constructing itself around the tempo you chosed earlier.

So basically, chosing exclusively "very hard" parts will make the level nearly impossible to pass for most people and will ask you to be very well timed in your movements and placment in the level, allowing you no rest throughout thewhole music. On top of that, to make the music intersting to listen, you'll need to vary the different tempo at your disposition.

# Difficulty
As the player is building its own level, SkipTheBeat was really hard to balance and as they often tend to make the level really hard just by cuiriosity of what could happen, the players lost really fast in the playtests. It was also really frustrating for them as they were not able to listen to the music they "created" earlier.

To balance things up, I decided to not make it a death on hit but to add a "hit count".
You cannot "finish" the level if you were hit, but you could train yourself as you'd like and listen to your whole music. It was far better and I started to see rivality between playtesters as they tried to take the less hit possible on the same patterns. It looked like the frustration was gone on this point and I was very satisfied with the new gameplay it offered.

# Play Skip The Beat
You can test SkipTheBeat yourself by downloading it on itch.io or download the Unity project.
Click on the logo below.

???
(itchio) https://malvy-delaban.itch.io/skipthebeat
(github) https://github.com/Malvy-Delaban/SkipTheBeat
???