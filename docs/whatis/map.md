# The Map and Exploration

Let's dive a little deeper into the game we're building, one chunk at a time. Today we're talking about the map and how you explore it.

## The Map
Everything happens on the map. Once upon a time, browser strategy games were little more than webforms where you'd click between pages of tables of data, click a few buttons, and get an image for flavor if you were lucky. This may have been acceptable in the days of DSL internet, but it's pretty boring in the futuristic year of 2020.

Almost all of our favorite strategy games revolve around the map, where you can see your empire rise and (hopefully not) fall in a way that really viscerally appeals to our primate brains. Starting with an expansive map was the obvious choice for Starfall. 

Structuring the map well and filling it with good content is so important because we want to encourage player mobility. We want players to be able to migrate to places and things they find fun over time, rather than being stuck wherever they built their headquarters. This is why players will be able to put engines on any design they choose - we call player assets *drones* for this reason. We have an entire galaxy to get through, so let's start from the top down.

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

Everything happens on the map. The galaxy has many star systems, and each star system is its own sprawling map filled with things to interact with. Heavenly bodies like stars, planets, moons, asteroids, and comets all exist on the map and can be interacted with, from mining asteroids to solar power from stars. Artificial objects exist too - other players' assets, obviously, but also non-player drones and bases, wrecks and salvage, and ancient ruins to investigate and reverse-engineer. We expect to see thousands of objects in star systems, and since all of them can be depleted, stolen, or blown up, each star system will change dramatically over time as players live in them. We're not fans of procedural generation and its endless piles of same-y stuff so we're working on ways to provide truly massive amounts of interesting, unique content.

## The Action
<p align="center">
  <figure>
    <a href="http://arkeindustries.com/philotechnica/img/9.PNG"><img src="http://arkeindustries.com/philotechnica/img/9.PNG"></a>
    <figcaption>You'll issue orders to your drones directly from the game map.</figcaption>
  </figure>
</p>

All gameplay happens from the map. Everything you physically own exists on the same map as all other players and NPCs in that star system. We don't plan on instancing or splitting the playerbase by server - it's just not fun.

You'll issue orders to your drones from the map, whether they'll be moving or shooting or mining or fabricating parts for construction.

3. Each star system has game objects.
4. We populate star systems with realistic usable objects.