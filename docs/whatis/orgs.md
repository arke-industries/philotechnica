> Posted 02/01/21 by AI Wizard

# Players and Organization

It's been pretty busy with the holidays and the world continuing to end, but we're getting back into the swing of things. With Omega Release under our belt, we're proceeding to a major internal refactor, usability pass, and dev playtest to make the game accessible for our playtesters later on with Psi Release.

Today it's time to talk about how players organize themselves. We know from our past games that player organization is the lifeblood of the game and we want to encourage big, impressive empires of players. At the same time, we've seen firsthand that exclusively giant orgs can feel bureaucratic and lifeless and even make the game unfun. We'll try to balance these scales by delineating between Avatars, Squads, and Organizations.

<p align="center">
  <figure>
    <a href="https://arkeindustries.com/philotechnica/img/20.png"><img src="https://arkeindustries.com/philotechnica/img/20.png"></a>
    <figcaption>We've thought quite a bit about how players interact with one another at both the individual and group levels.</figcaption>
  </figure>
</p>


## Avatars

**Factsheet: Avatars**

- Analogous to characters
- Owns physical assets (like drones) and intangible assets (like tech)
- Can join Squads or Orgs
- Can be account-bound (personal) or Organization-bound (communal)
- Accounts start with one, may offer more later

In most games, you are your account - an identity intrinsically tied forever to your account ID and usually publicly exposed. Since one of Starfall's core design tenants is "information isn't free," this didn't make much sense for us. We wanted to pursue something more like the character model seen in many MMORPGs, where you interact with the world through a character and the account is more in the background.

You can consider Avatars the equivalent of characters. You'll give orders through your active Avatar. Avatars own the physical assets that exist on the map (which we've talked about before), and they also hold intangible things like unlocked technologies, designations, and squad and org memberships. Avatars can't be destroyed - if all of your physical assets are destroyed, the avatar will be granted some starting equipment to start over. Starting over isn't a death sentence, though - the fact that Avatars remember the techs they've unlocked means that your second (or third, or fourth) try will be exponentially faster than your first.

One of the advantages of using Avatars instead of accounts is that we don't have to limit this functionality to individual players. We can have players impersonate (play the game as) another Avatar. Organizations can create Avatars that are bound to that Org, and allow certain Squads the ability to use that Avatar. This makes things like centralized military forces possible, control of which can be delegated to authorized players via the ability to use their Avatar. 

## Squads

**Factsheet: Squads**

- Small, tight-knit units composed of Avatars
- Share common permissions to each others' drones like add/remove cargo, sensor data, allow repair
- Can join Orgs or act independently
- Only join a Squad composed of Avatars you trust, preferably a group of IRL friends

We have years of fond memories of LAN parties and tight-knit gaming clans in the 2000s, and in the browser gaming world this held true too. Groups of friends or classmates would play the classic browser games like CyberNations and Nationstates together. In the former you'd even have someone "nation-sit" while you were away for a long period of time, collecting resources and defending your nation so you'd actually have something to return to.

This is where our idea of the Squad came from. A Squad should be made up of a single-digit number of close-knit players to help them play better together. They're able to help each other out with common permissions, such as the ability to repair each others' drones without restriction, share line-of-sight, and add or remove cargo. That means that being offline in hostile territory isn't a death sentence - your squadmates have your back.

You also know where your squadmates are at all times and what they're doing to faciliate cooperation. Because of this, we envision that most Squads will be made of players who know each other outside of Starfall and can trust each other. Information, after all, is power.

We wanted to carve out a space in player organization between totally solo and in (potentially) gigantic, impersonal alliances, and make sure that space is respected. Squads don't have to dissolve if their members decide that a larger Organization is right for them, either - a Squad can join or leave an Organization without impacting its structure.

## Organizations

**Factsheet: Organizations**

- Large player organizations composed of both Avatars and Squads
- Avatars can join multiple Organizations
- Offices determine how permissions are spread among Avatars
- Can create Avatars bound to that org (instead of to a player account) to control org assets like fleets
- Can designate Squads to have permission to use Org-bound avatars

Finally, we have the large player organizations. We've seen players run large player orgs like corporations in other MMOs, in some cases even having whole IT departments running sites and services specifically for the players' benefit and organization. We wanted to give Orgs the ability to self-structure.

As mentioned above, both Avatars and Squads can join player Organizations. Players in an Org can also use Squads to structure themselves inside that Org - the command squad, the industry squad, combat squads, and so on. There are two permutations of this model specific to Organizations which extend their ability to organize:

1. Organizations can create Avatars which are bound to that Org (versus account-bound). These Avatars can serve as loci of control for Organization assets without them being owned by a player. Org fleets and holdings can remain neatly bound to that Avatar, and permission to use that avatar can be granted by the Org to specific squad(s) as needed. This ensures that, for example, a player "admiral" can easily step into an Org fleet to use it without personally owning those drones - and the Org can also revoke the admiral's access if they go rogue.
2. Organizations can create Offices held by specific Avatars. Offices have certain sets of Org permissions (like create/delete Org-bound Avatars, accept or reject new members, change join policy to open/invite/closed), and granting an Office to an Avatar grants them its powers. These can be used traditionally for roles like President, CEO, or Admiral, or in more novel fashions - for example, you could give every player in your Org the power to rename the Org. It'd be a bad idea, but you could!

Finally, unlike traditional player organizations in MMOGs, there is no limit on the amount of Organizations you can join. You needn't tie yourself to one player entity for all time - you could join a defense pact Org for military matters, a trade association Org for contracts, and a political Org for political affairs. We're not quite sure how this will play out on the UI yet, but we're very adamant about allowing this.

That's all for player organization. Join us next time when we talk about the cornerstone of player industry - Recipes!