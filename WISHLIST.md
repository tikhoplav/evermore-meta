# My MUD wishlist.

> This is Heroes of Evermore community project. The idea behind this is to organize and accumulate as much great ideas that community generate as possible. The whishlist is still pretty raw, so let's improve it together.

<br />

Some rules to follow working with this document:

- Post every new idea under it's bullet (list item) in the according section `Visuals`, `Gameplay`, `UX`, `Lore`. If are not sure which section to pick for your idea, contact me (`@V`) in the discord or put it under the `Raw ideas` section.

- If your idea can not be described in a couple sentences, use child bullets to provide more info:

  - Like this.

- Try to use as less images and external links as possible, but if it's really necessary - just go for it.

- If you want any idea from the list to be adjusted/redefined, please create a comment to it describing your thoughts.

- If you like the idea as it is, leave the comment with `+` sign to vote. The most voted ideas will be implemented in the game.

- Feel free to ask any help in the discord chat [TESTER GUILD / alpha-pass](https://discord.com/channels/883956356397269082/945543263446761562).

> This 

## Visuals.

The following is ideas of visual improvements of the game client.

- Make enemy corpses to not disappear from the target list:

  - This is a good indicator that enemy has been killed;

  - When corpse disappears - this means that enemy character has been revived;

  - Corpses can serve multiple interesting mechanics such as:

    - Resurrection of a fallen ally;

    - Skills that make corpses explode;

    - Consumption of a corpse to gain buff;

    - Consumption of a corpse to summon a minion;

    - Turn a corpse into a portal...


- Make all current statuses, such as stunned, silenced, trapped etc displayed
  somewhere at the screen as icons with timers on it and on-hover popups with
  explanation of the status; All buffs and debuffs should also be displayed;


- Some of the statuses, buffs and debuffs should also be displayed as miniature
  versions of original icons at enemies tiles. The list could be limited to the
  most crucial effects;


- Add a progress bar to enemies and allies tiles if they are in the process of
  casting a spell;


- When selecting a direction for a ranged skill, like `quickshot`, make it's
  icon glowing or have an animated border;


- Add colors to the damage output notifications according to the skill that has
  inflicted the damage. The same should be applied to non-damaging skills too;


- Add `flee` and `attack` icons with timers and on-hover descriptions the same
  way it is done for skills. `Attack` icon should also show approximate damage;

- Make movement between tiles animated, instead of a simple frame switch. A
  character symbol should fade out from the current tile, "camera" should
  smoothly go above the next tile, and after the symbol should fade in; 

<br />

## Gameplay.

The following is ideas about the gameplay: game mechanics, effects, skills, map features e.t.c.

- Add `movement speed` as a time delay between two consequent movements between
  tiles. If players are moving in group using the `follow` logic, make whole
  group move with the speed of the slowest group member;


- Make `flee` only possible to a tile that was occupied before the current one.
  Add a cooldown to `flee` that based on the character's `movement speed`;


- Make vision shared between members of one team in a match and make `heat` not
  displayed for rooms outside of the group vision. Dead character should have
  zero vision range;


- Make mobs to chase players only if players are in their vision range. Taking
  into account that `movement speed` is limited, shaking a tale would be not a
  trivial task;


- Add a slight delay for all auto attacks, so that when player enters a room
  with aggressive mobs, there is a chance, for characters with high `movement
  speed`, to bypass before the combat starts;
  

- Change character leveling system:

  - Make it so that the average level reached during a standard 30 min match
    would reach 20. All the benefits of gaining a new level should be adjusted
    accordingly;

  - Make skills unavailable by default. In order to enable skills player should
    spend skill points, that he receives as a reward of gaining a new level;

  - In addition to skill point and slight hp / mana powerups when new level is
    reached, player should be asked to choose between three random bonuses.

    The bonuses could be of various kinds starting with simple + to attribute,
    addition to certain skill damage/cooldown/cast speed, or even a significant
    modification to a skill, for example double cast, or a single target skill
    turns into a multi-target etc.

    No pause should be provided for player to choose a bonus and the decision
    should be made right after level is gained;

  - Instead of the plain list of skills available for each class, make skill
    trees with branches, where each ascendant node is available only after
    descendant nodes are opened. In addition to active skills such tree would
    also contain various passive skills and switchable skills like auras.

    Having more then 7 active skills would require configurable skill bar where
    skills can be selected from the list and would be assigned to a hot key;

- Add/Adapt properties of attacks/skills/spells, assign each property a color:

  - Physical;

  - Fire;

  - Cold;

  - Lightning;

  - Poison;

  - Shadow;

  - Light;

  - Chaos;

  - Nature;

  - Arcane;

- Add more status effects:

  - Poison - damages a character over time, with damage decreasing over time;

  - Burn - damages a character over time, increases it's resistance to cold
    property attacks;

  - Freeze - disables a character's ability to perform actions, increases it's
    physical defense and makes it vulnerable to lightning property attacks;

  - Chill - slows a character's action speed and reduces it's defense against
    lighting property attacks;

  - Petrified - prevents a character from performing any actions, highly
    increases it's physical defense and reduces it's defense against fire
    property attacks;

  - Bleed - damages a character over time and reduces all healing effects
    applied to it;

  - Shock - reduces a character's action speed as well as it's ability to flee
    attacks. Increases a chance for a critical hit against the character;
    
  - Hex - prevents a character from performing any actions except for moving,
    reducing it's action speed and dramatically reducing it's physical defense;

  - Fear - makes a character uncontrollably run away;

  - Chaos - inverses a character's controls, switch west to east etc;

  - Silenced - Prevents a character from using spells;

  - Disarmed - Prevents a character from using skills and attacks;

  - Blind - Reduces a character's vision range and it's ability to hit a target
    when attacking or using a skill;

- Add spells aimed at removing harmful statuses for support classes. Example:
  `cure` - removes `chaos`, `silenced`, `disarmed` and `blind` status effects;

- Add aura spells. Example: `clarity` - regenerates `X` mana per second to each
  ally in radius of `Y` tiles;

- Add switching (toggable) passive skills. Example: `burning arrow` - adds
  damage of fire property to all ranged physical attacks and skills, increasing
  the amount of mana/energy consumed (base attacks would also take some mana);

- Add ground based buff skills. Example: `rally banner` - increases defenses of
  all allies in the tile when placed, lasts for `X` seconds. `Healing totem` -
  restores `X` hp each second to each ally in the tile, lasts `Y` seconds;

- Add movement skills. Example: `dash` - causes the character to quickly move
  `X` tiles forward, bypassing the front line of the enemy;

<br />

## UX.

The following is ideas related to the User Experience (UX): game responsibility, speed of processing, usability of the interface e.t.c.

- Instead of having an input lag at the MUD side, after which all commands that
  was enqueued explodes, make input disabled at the client side, except for a
  number of commands like `who`, `where`, `scan` etc. During input cooldown, UI
  should be showed disabled by graying out interactive elements;

- Reduce the amount of packets transferred with WS, as it leads to freezes and
  stutters of the client with high ping high latency connection. Optimize net
  packets to reduce their weight;

- Reduce the bundle weight for website and client (Probably event detach client
  from the website) as it leads to long loading time and unreasonably high
  memory consumption (6s and 3.6Mb at average);

- Make media (like sounds) loading optional, as it prevents playing from mobile
  network due to large amount of traffic downloaded;

- Increase the overall performance of the game client, probably by using Wasm
  with more performant language;

<br />

## Lore.

The following is ideas related to the games Lore.

- Add resources to read about game lore, currently there is none. All info
  about game setting, the World and concepts of the game are provided verbally.
  
<br />

## Raw ideas.

Here comes all the ideas that hasn't been yet fully figured out but has some value behind it.
  
<br />
<br />
<br />
<br />