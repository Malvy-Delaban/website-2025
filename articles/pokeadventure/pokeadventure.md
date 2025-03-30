Title: "Poke Adventure"
Tags: "Mobile" render, "Web" render, "Full Game" game, "Advent Calendar" genre, "Solo Project" team
=====
# About Poke Adventure
Poke Adventure is a mobile game playable on navigator. It is mobile exclusive as it cannot be run on PC with a navigator (except using the Chrome development tool to simulate an Iphone 12 for example).

At first, this project was created for my other half. We have that little ritual of ours each year to give a theme to our christmas together. In that way, the little things we buy for each other / the gifts are resolved around that theme at that period of the year. In 2024 we had the Pokémon theme.
I had the idea to create a numeric advent calendar of Pokémons.

# Concept & gameplay
The concept is the following: each day, you encounter 3 pokémons and you choose one to capture. It is added to your Pokémons collection and you can then add it in your team to fight one battle each day. You can make them level up and evolve. The game also includes some other mechanics such as shiny Pokémons, a shop to buy evolving items / useful items, an event code system and more.

!!!
(main-page.jpg) Main page
(encounter.jpg) Encounter
(my-pokemons.jpg) Your pokémons
(poke-detail.jpg) Pokémon view
!!!

# Development & community
I had the idea and started prototyping in September 2024 with the objective to have it ready on December 1st, date of the advent calendar start. Therefore, I had 3 months for development with a deadline on November 1st for the start of my playtests with 3 previously selected testers that I choose for there knowledge of the Pokémon franchise.

This project is an exclusively solo project but I had the help of multiple players, my platesters obviously, my other half but also other players that wanted to play when they heard about the idea. Their feedbacks were crucial to fix bugs along the development and during the month of December.

To maintain some interest for the game, I created multiple ponctual events during December. Some giveaway of in-game currency or extraordinary encounters with legendaries for example. I displayed posters to advertise the game and some events in my school.

!!!
(poster.png) Poster
(event-poster.png) Event poster
!!!

From this small base of players (around 20 to 30 persons in December), a few asked for an infinite mode to continue to play after December 25th. I did implement that and some of them continue to play to this very day. As I write those lines in March 2025, the game have, at my knowledge, 8 active players that get their pokémons everyday.

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
During the development, I had the chance not to encounter huge issues that would stop the development for multiple days.
But I had issues nonetheless. Here are some examples and how I solved them.

Firstly, the game was made without a backend / a server due to the lack of budget I had for this project. Thus, no save can be made on distant server and everything has to be done in local on client side. So, to save the progression of player, I used the localstorage. This way, even by closing navigator or the tab, progression is saved locally. I implemented a download and upload save file system to ensure that my players do not lose their progression on deleting the cache of the navigator.
doing things locally have downsides, for example, a player can easily cheat if they have the basis in webdevelopment. I considered it to be a good way to create interactions between players and didn't complicate things up while developping to allow them to search around and have fun with the game system. The local-based system also prevents me from implementing combats and exchange between players but as it was meant to be an exclusively solo game, that was something that didn't bothered me much at the time.

The data collection and structure was a big chunk of the project as I had to get data of all the 1000+ Pokémons, get their sprite in normal and shiny variants and have them game ready for me. To do so without losing to much time making it by hand, I created a dozen of python scripts to gather the data I needed and format them. Another issue with this is that I had to gather all data in french and to code the whole U.I. in french as my other half doesn't speak english. I had to use different APIs to get the equivalent in french of the data I had.

Also, it is interesting to note that I challenged myself to create this project in pure JS without any framework or external library. All was made by hand, from the mockups to the CSS.

# Pre-prod
As I wanted the game to be balanced and enjoyable I had to spend a lot of time in pre-production to be sure each pokémon I gave each day were not too strong to beat every battle on its own but also not to weak to prevent player frustration. I made a lot of graph that helped me to balance Pokémon stength, rarity and drop rate. For example, the above graph was the way I set up the rarity spreading and the drop rates for each 24 days of the advent calendar.

!!!
(balance-days.png) Balancing encounters
(huge-graph.png) Each days
!!!

I also needed to write down which Pokémon would have which rarity. As I wanted the rarity to be based on my other half's liking for each Pokémon, I had to do it manually and couldn't make the process automatic by scripts. It took my hours to do but I decided to create a "tier list" to sort every Pokémon. To be efficient and coherent, beforehand, I established some rules for the tier list.
The rarity are the following: Common, Uncommon, Rare, Epic, Ultra, Legendary.

Some rules I followed to help me gain time:
- Every starter Pokémon and their middle evolution would be EPIC
- Every last evolution of a starter Pokémon would be ULTRA
- Each legendary and mysthical Pokémon would obviously be LEGENDARY
- The last evolution of a Pokémon should always be of higher rarity than its "prevolution"
- The last evolution of a Pokémon that my other half like must be ULTRA

This way, I ended up with this tier list of the 1000+ Pokémons.

!!!
(tierlist.png) Rarity tier list
!!!

# Play Poke Adventure
You can play right now ! Click on the Web icon below and start your adventure if you're on your phone. You can also browse the project on Github and check the patchnotes in the github readme.

???
(web) https://poke.malvy-delaban.fr/
(github) https://github.com/Malvy-Delaban/christmas-2024
???