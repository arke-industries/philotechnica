> Posted 12/07/20 by AI Wizard

# Detection and Display
We push ever onward in our overview of Starfall, towards the playable test that is our goal. Today we're talking about detection and display on the map.

As we've said, "Information isn't free" is one of our design philosophies. Unlike most strategy games, detection isn't all-or-nothing. We've taken inspiration from real target acquisition in modern combat, where commanders have to quickly decide with limited information whether an incoming target is an enemy bomber or an off-course jetliner. You'll have to strike a balance with limited information - shoot first and potentially hit a third party, or wait for confirmation and risk being struck hard.

In increasing difficulty order, we want to show you multiple things about a given contact to help you decide what to do about it:

1. **Location**. Where was the contact detected? What is its bearing?
2. **Emissivity**. How much heat and EM is it giving off? Hot, "noisy" contacts can indicate a higher threat.
3. **Design**. What components are on this drone? Is it a freighter or a gunship?
4. **Identity**. Which player owns this drone? Are they a known enemy?

On top of showing you varying levels of sensor data, we'll also show you other information to understand a threat situation at a glance - info about your fellow Organization and Squad members, designations you set for other players, and who's recently been in combat.

## Scanning
You can equip your drones with Scanners to gather this information. Similarly, you can equip your drones with Jammers to make it harder for an opponent to gather certain pieces of information. Whether a scan attempt succeeds depends on how strong the Scanner is, how strong an opposing Jammer is, and the distance between the two.

Your drones' scanners scan every game tick. Because objects are often moving and there is an element of randomness to the calculations, your scanners may sometimes succeed and sometimes fail to resolve contacts, especially at range.

<p align="center">
  <figure>
    <a href="https://arkeindustries.com/philotechnica/img/14.gif"><img width=500 src="https://arkeindustries.com/philotechnica/img/14.gif"></a>
    <figcaption>Here is an extreme example of scan results varying over time, caused by setting scanner efficiencies very low.</figcaption>
  </figure>
</p>

Here are the biggest factors that impact how easily your drones can be detected:

1. **Distance**. In keeping with the [inverse-square law](https://en.wikipedia.org/wiki/Inverse-square_law), it's increasingly hard to detect electromagnetic radiation as distance increases.
2. **Heat**. The hotter you run (doing things like like using your engines, firing weapons, or heavy industry) the easier you are to detect against the cold background of space.
3. **Electromagnetic radiation**. We simply call it "EM," a catch-all for light, radar, radio sources that your drone may be putting off or reflecting. Much like stealth planes in real life, drones can be designed to reduce this output.
4. **Size**. Go figure, big stuff is easier to detect. This is most obvious for celestial bodies.
5. **Transponders**. You can broadcast your location and identity if a drone has a transponder onboard - not very useful for war, but critical for building trust for trade and cooperation.
6. **Jammers**. Different types of jammers obfuscate some of these factors - heat sinks can reduce heat signatures temporarily, ECM can make EM harder to pinpoint - but none can totally hide you. As the man says, [There Ain't No Stealth In Space](http://www.projectrho.com/public_html/rocket/spacewardetect.php#id--Strategic_Combat_Sensors--There_Ain't_No_Stealth_In_Space) - but you *can* misdirect and obfuscate enough to exploit your opponent's hesitation.

## Contacts
<p align="center">
  <figure>
    <a href="https://arkeindustries.com/philotechnica/img/13.png"><img width=500 src="https://arkeindustries.com/philotechnica/img/13.png"></a>
    <figcaption>Here, three of our drones detect an unknown Contact to the right.</figcaption>
  </figure>
</p>

When you first detect other players' drones and other game objects, they'll appear as Contacts. These are sensor objects which merely tells you that *something* exists out there. These sensor objects appear on the map and give you some or all of this information when clicked:

- **Location.**
- **Size.**
- **Bearing**. Is it headed towards you, away from you, somewhere else? Contacts on an intercept course are much more suspicious.
- **Emissivity**. How much heat and EM is it giving off?
- **External components.** What can we detect on the outside of the drone? These will be things like engines and external weapons.
- **Internal components.** What can we detect on the *inside* of the drone? This is much harder and can require specialized equipment like penetrating radar.

## Designations
<p align="center">
  <figure>
    <a href="https://arkeindustries.com/philotechnica/img/12.png"><img width=500 src="https://arkeindustries.com/philotechnica/img/12.png"></a>
    <figcaption>Here we see Enemy-marked contacts in red, Friends in blue, Suspicious in purple, and Targets in orange.</figcaption>
  </figure>
</p>

Because the combat picture can be nuanced, we want to give you a way to note to yourself players of interest. These designations will show on all contacts that you know they control. We're starting with these:

- **Friend.** Regardless of Org or combat status, you consider this player friendly. All their drones will be marked as such.
- **Enemy.** Again regardless of Org or combat status, you consider this player an enemy and want all of their drones to be marked as such. This can be useful to identify enemy reinforcements early.
- **Suspicious.** If someone's snooping around or following you, mark their drones as Suspicious to keep an eye on what they're doing.
- **Target.** This can be for anything you want - maybe you want to target a neutral player in order to protect them (perhaps as part of a contract), or there's some non-combat reason why you want them on your proverbial radar.

We'll likely add other types of Designations as users suggest them.

## Affiliations
On top of your own records about other players and their drones, you may also be in one or more Organizations of players. You may also be placed in a single Squad in your Org (more on that later). In the heat of battle, you'll need a way to easily tell who around you is in your Squad, who is merely in your Org, and who is not related to you at all.

## Combat Status
<p align="center">
  <figure>
    <a href="https://arkeindustries.com/philotechnica/img/10.png"><img width=500 src="https://arkeindustries.com/philotechnica/img/10.png"></a>
    <figcaption>Thick dashed red lines mean that a contact was attacked recently. You can see it on our drone and the neutral contact in the top left.</figcaption>
  </figure>
</p>

There's one more type of info that you'll need to know in the moment - combat action information. More specifically, you'll need to know:

**About other drones:**

- Which drones attacked you recently
- Which drones are owned by the same player as ones who attacked you recently (and so are likely threats)
- Which drones did *you* attack recently
- Which drones are owned by the same player as ones you attacked recently (and so may counterattack)

**About your drones:**

- Which of your drones attacked recently
- Which of your drones *were* attacked recently

Our current MVP of this combat information system uses boxes because they're easy to render, but we'll probably boil these down into icon sets that we can user test. These icons have to be immediately recognizable and understandable on a busy battlefield.

## History
Because we have a chunk of time between ticks (to allow us to process actions and events together), we're not quite real time. That means it's important that we give you tools to understand what's changed since you last logged on.

History will show you what happened around your ships recently, up to the limit of their scanners. It replays as if you were there to witness it, but it's just a historical record.

It's best seen to be explained. Here's a video of a user browsing the history of their drones' sensor data for the past few game ticks:

<p align="center">
    <iframe width="560" height="315" src="https://www.youtube.com/embed/6pvCr7Dqcug" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</p>

Keep in mind that the UI is very much a placeholder for testing. Before going live we'll want to give you something more like media player controls - stop, start, rewind, fast forward.

We're still testing to see how much history we can offer players on our current level of hosting since it's very CPU and memory hungry. We want to try and keep monetization limited to things that represent big hosting or processing costs for us, so having a very long history replay may be something that costs money. More on ethical monetization later.

That's all for detection and display. Next time we'll be talking about building interesting interactions that happen both with and without other players - the narrative.