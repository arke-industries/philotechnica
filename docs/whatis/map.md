# The Map and Exploration

Let's dive a little deeper into the game we're building, one chunk at a time. Today we're talking about the map and how you explore it.

## The Map
Everything happens on the map. Once upon a time, browser strategy games were little more than webforms where you'd click between pages of tables of data, click a few buttons, and get an image for flavor if you were lucky. This may have been acceptable in the days of DSL internet, but it's pretty boring in the futuristic year of 2020.

Almost all of our favorite strategy games revolve around the map, where you can see your empire rise and (hopefully not) fall in a way that really viscerally appeals to our primate brains. Starting with an expansive map was the obvious choice for Starfall. 

Structuring the map well and filling it with good content is so important because we want to encourage player mobility. We want players to be able to migrate to places and things they find fun over time, rather than being stuck wherever they built their headquarters. Players will be able to put engines on any of their designs - this is one reason why player assets are drones and not ships or stations. The other reason is that players are starfaring AIs, but more on that later.

We have an entire galaxy to get through, so let's start from the top down.

## The Galaxy

Star systems are our basic navigational unit - there are many of them in the galaxy, and everything interesting on the map (planets, moons, your drones, everyone else's drones) resides in specific star systems. Think of them like islands. You'll jump to new star systems using the faster-than-light (FTL) jump drives on your drones, and then once you're there you'll discover the celestial bodies and hostile natives within.

### Discovery
<p align="center">
  <figure>
    <a href="http://arkeindustries.com/philotechnica/img/7.PNG"><img width=500 src="http://arkeindustries.com/philotechnica/img/7.PNG"></a>
    <figcaption>You'll discover new star systems or buy starcharts from other players to expand your list of destinations.</figcaption>
  </figure>
</p>

One of our central game design tenants is "information isn't free." We won't provide you a map of all the stars in the galaxy - you'll have to go find and explore them yourselves. Right now we envision that happening in two ways:

1. **Detection.** [Much like the pros](https://exoplanets.nasa.gov/), you can equip exosolar detection gear on your own drones and go searching for new stars. For each one you detect you'll receive a starmap - all the data your drones need to safely FTL jump to that system. You can jump to the first one you see or stay in one place to build your own star catalog.
2. **Commerce.** On the other hand, if someone else already has starmaps you want, you can just use the ingame market to buy them. This is the more literal interpretation of "information isn't free." If you fancy yourself an astronomer, you can try jumping to the frontier of settled space and detecting a bunch of new stars in order to sell the starmaps to other players - they'll likely pay a higher price for stars nobody has explored yet.

### Star Systems
<p align="center">
  <figure>
    <a href="http://arkeindustries.com/philotechnica/img/8.PNG"><img src="http://arkeindustries.com/philotechnica/img/8.PNG"></a>
    <figcaption>Each star system is a gigantic, bustling destination unto itself - even our test star system is already getting pretty busy.</figcaption>
  </figure>
</p>

We hope to give players a good sense of how big a star system actually is. We can populate systems with a truly epic amount of celestial objects, from inner rocky planets to gas giants with their dozens of moons, from inner asteroid belts to Oort objects and comets near the heliopause.

All of them will be interactable in some way, most of them mineable. You can set up shop anywhere in a solar system, whether jockeying for control of a Jovian planetary system or disappearing into the Oort Cloud to mine, refine, and resupply. Like in the real world, most asteroids are separated by significant distance, so you can set up a defensive perimeter around one and mine it to fuel your supply chain until it's depleted or you want to move on.

We also don't plan to cap the number of players that can be present in one solar system. If there's a big showdown between Organizations, we want everyone to be able to dogpile in. For that matter, there's no restrictions on having a player's drones across multiple star systems.

Finally, some star systems will have natives to contend with. That could mean non-player drones, bases, or other species entirely. You may also run across wrecks, salvage, or ancient ruins to investigate and reverse-engineer. These will present varying levels of challenge to players. Some may be pushovers a sole explorer can handle, while you may find some so strong that a concerted effort will be required to defeat them.

## The Action
<p align="center">
  <figure>
    <a href="http://arkeindustries.com/philotechnica/img/9.PNG"><img src="http://arkeindustries.com/philotechnica/img/9.PNG"></a>
    <figcaption>You'll issue orders to your drones directly from the game map.</figcaption>
  </figure>
</p>

All gameplay happens from the map. Everything you physically own exists on the same map as all other players and NPCs in that star system. We don't plan on instancing or splitting the playerbase by server - it's just not fun.

You'll issue orders to your drones from the map, whether they'll be moving or shooting or mining or fabricating parts for construction. You'll see the results of those orders on the map on the following tick (unit of game time). Every game, even "real time" ones, measure game time in ticks - some are milliseconds long as in shooters, while ours will likely be on the order of minutes.

Right now, that's a necessary tradeoff to have one game world with no separating players or systems getting out of sync. For now we'll accept a longer tick duration and work to make the gameplay loop engaging regardless of session length. Later, we have some research to do about parallelization and infrastructure to get the best performance.

That's all for the map. Next time we'll be talking about the first step in interacting with this game world - detecting player drones and stellar objects.

