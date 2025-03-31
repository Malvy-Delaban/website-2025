Title: "Poke Adventure"
Tags: "Mobile" render, "Web" render, "Full Game" game, "Advent Calendar" genre, "Solo Project" team
=====
# About Poke Adventure
Poke Adventure is a mobile-exclusive game playable on a browser. While the game cannot run natively on PC through a browser (except with developer tools like simulating an iPhone 12 on Chrome), it's designed with mobile devices in mind.

This project was born out of a personal tradition with my partner: every year, we select a theme for Christmas and base our gifts around that theme. For 2024, we chose Pokémon. I wanted to create a digital Advent calendar filled with Pokémon-themed surprises for each day leading up to Christmas.

# Concept & gameplay
The core concept is simple: each day, you encounter 3 Pokémon and choose one to capture. It adds to your collection, and you can use it in daily battles. The game includes features like Pokémon evolution, shiny Pokémon, a shop for items, event codes, and much more.

!!!
(main-page.jpg) Main page
(encounter.jpg) Encounter
(my-pokemons.jpg) Your pokémons
(poke-detail.jpg) Pokémon view
!!!

# Development & community
I began prototyping in September 2024, aiming for a December 1st launch. With a deadline of November 1st for the playtest, I worked diligently to make sure everything was ready in time. While this was a solo project, I received valuable feedback from testers, my partner, and a few players who were interested in the concept.

To keep players engaged during December, I hosted special events, such as giveaways and unique encounters with Legendary Pokémon. The game quickly gained traction with a small but loyal group of players—around 20 to 30 active users by Christmas. Some even requested an infinite mode, which I later implemented to continue the adventure beyond December 25th.

!!!
(poster.png) Poster
(event-poster.png) Event poster
!!!

# New features
With the number of reccurent players not decreasing after January and February, I decided to make a huge patch to fix the bugs they noticed and implement some features they asked for weeks. For the completionnists, I created a pokedex, to help them track the Pokémons they encountered and catched and an egg shop to help them find the Pokémon they struggle to find. I also implemented an automatic recurrent event based on the phase of the moon to break the monotony of the encounters, thus, 2 times a month, a special encounter will provide shinies on full moons and another with increased rarity pokémons for new moons.

!!!
(egg.png) Egg buying
(egg-wait.png) Waiting
(egg-atch.png) Atched
!!!

!!!
(pokedex.jpg) Pokedex
(pokedex-detail.jpg) Pokedex details
!!!

# Difficulties
Though I didn’t face any massive blockers, there were some challenges along the way:

No Backend:
The game runs entirely locally, which meant no online saves. I used local storage and created a save file system to ensure that players didn’t lose progress if they cleared browser cache. This setup also allowed some players to cheat, but I chose not to complicate the system, as it was meant to be fun.

Data Collection:
With over 1000 Pokémon to gather data for, I used Python scripts to collect and format the necessary information. I also ensured everything was in French, as the game was created specifically for my partner.

No Frameworks:
I built the entire game from scratch, including UI and CSS, without relying on external libraries or frameworks.

# Pre-production
I spent considerable time balancing the gameplay, making sure each Pokémon I selected for each day was not too strong to win every battle easily but also not too weak to be frustrating. I used graphs and tier lists to help balance Pokémon strength and rarity, as shown in the graph below. It was also mainly based upon the likings of my other half.

!!!
(balance-days.png) Balancing encounters
(huge-graph.png) Each days
(tierlist.png) Rarities - Gen 1
!!!

# Play Poke Adventure
Ready to start your adventure? Play the game on your phone now by clicking the Web icon below. You can also check out the project on GitHub and read the patch notes there.

???
(web) https://poke.malvy-delaban.fr/
(github) https://github.com/Malvy-Delaban/christmas-2024
???