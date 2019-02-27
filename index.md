# About TravTools!

Tarvtools is a free to use Discord Application for the game Travian! If you're a player of this game, you might now the useful wab pages of Gettertools and Killiroid! Travtools was made with the intention to replace both and to have more useful functions that can be used by alliance leaders and players on their own discord server chat :)

## Support and Contact

Travtools has expenses. Plus I need money to be able to work on it properly! become my patreon and support travtools today!

**[Become My Patreon](https://www.patreon.com/travtools)**

You can also find Travtools discord channel [here](https://discord.gg/CxKEWtE).

## Installation

To install travtools open the following link if you're a server admin: [Install Link](https://discordapp.com/oauth2/authorize?client_id=417397766931611648&scope=bot&permissions=8)

Just choose your server and confirm the captcha and it's done :)

Reminder that you don't need to give travtools the administrator permissions (you can remove that tick) :)

## Functions

### Ping

This function is to ping the bot to see if she is online or not - or to play ping pong with her!

```markdown
~ping
```

### Hi

These functions are for people who wanna greet travtools! She is really polite :)

```markdown
~hi
~hello
~hoi
```

### Created By

This function is to find me on discord! I'll like to hear your feedbacks and comments :) You can also join travtools discord for that!

```markdown
~createdby
```

### Time

Returns the time in UTC 0.00. (Soon: In future there will be a way to set the time zone for your servers!)

```markdown
~time
```

### Distance

This function can calculate the distance, travel time for your troops and the return times (if they are sent right away).

Travel time and Return time will be calculated if you input the troop name. If you also input the tribe of the troops the search will be more limited.

```markdown
~distance [Coordinates A] [Coordinates B] [Tribe name (Optional)] [Troop Name (Optional)] -x[Server Speed] -ts[TS level] -haste[Haste Artifact Rate] -(boot|merc)[Tire] -spur[Tire] -pennant[Tire] -standard[Tire] -map[Tire]

All tags that are added to the function that start with - are optional. About them pay attention that:

1. The valid values for server speed is all integers > 0. The valid values for ts option is 1 to 20. The valid values for haste option are 1, 1.5 and 2

2. -boot or -merc will consider a Mercenary/Warrior/Archon boots and will assume the hero is with troops. The valid values for this option are 1,2 or 3 (the tier of the boot)

3. -spur is for Spurs boots and will assume hero is with the troops and is mounted. The valid values for this option are 1,2 or 3 (the tier of the boot)

4. -pennant is for the Pennant and will assume hero is with the troops and that the target location is a village of yours. The valid values for this option are 1,2 or 3 (the tier of the item)

5. -standard is for the Pennant and will assume hero is with the troops and that the target location is a village in your confedracy. The valid values for this option are 1,2 or 3 (the tier of the item)

6. -map is for the Maps and will assume hero is with the troops. The valid values for this option are 1,2 or 3 (the tier of the item)

```

NOTE: The distance function will work for merchants and heroes.

NOTE: This function will only work on 801 * 801 maps (the large maps) in some servers the maps are 401 * 401 there will be an update later to allow you to set the map size for travtools in your server.

NOTE: Please input the troop speed after -x not the buildings speed. A 5x server can have 2x troop speed. This detail is announced in server start notification on forums. If you had questions about this please ask me on the discord channel.

For example:
```markdown
~distance 0|0 0|100 gaul tt -x3 -ts5 -haste1.5 -boot2 -map2
```

This example will return the distance between (0,0) and (0,100) (which is 100). It will also return the travel time and return time of Theutates Thunder assuming the troops speed in server is x3, the Tournament Square level is 5, the player has a great haste artifact (1.5x faster troops) and the hero that is with thunders is using a Boots of warrior and Map (tier 2 map)

![img](https://cdn.discordapp.com/attachments/382038627758243841/550325836574883862/distance.png)

### Info

This function is a basic search function. It can give you random information about buildings/troops/artifacts/regions and tribes. There is a specific function for each as well!

```markdown
~info [Search]
~info [Tribe name (Optional)] [Troop Name]
```

NOTE: You can't input server speed with info function.
NOTE: You can't see level specific details about buildings using info function. for that use the Building function.

![img](https://cdn.discordapp.com/attachments/382038627758243841/550328121963053066/info.png)

### Troop

This function can give you a basic knowledge about troops and their train time/cost.

```markdown
~troop [Tribe name (Optional)] [Troop Name] -x[Server Speed]

All tags that are added to the function that start with - are optional.
```

NOTE: Please input the troop training speed after -x if you want the train time to be accurate. A 5x server can have 2x troop train speed. This detail is announced in server start notification on forums. If you had questions about this please ask me on the discord channel.

NOTE: Please input the troop speed after -x if you want the troop velocity to be accurate. A 5x server can have 2x troop speed. This detail is announced in server start notification on forums. If you had questions about this please ask me on the discord channel.

**Troops train speed** and **Troop speed** Are not neccesirly equal!

![img](https://cdn.discordapp.com/attachments/382038627758243841/550328948379222026/troop.png)

### Research

This function can be used to see the research requirements for different troops. It also can show the cost and research time of each troops. (Soon: This function will have smithy upgrades as well!)

```markdown
~research [Tribe name (Optional)] [Troop Name] -x[Server Speed]

All tags that are added to the function that start with - are optional.
```

NOTE: Please input the research speed after -x if you want the research time to be accurate. A 5x server can have 2x research speed. This detail is announced in server start notification on forums. If you had questions about this please ask me on the discord channel.

![img](https://cdn.discordapp.com/attachments/382038627758243841/550329277308993549/research.png)

### Tribe

This function will give basic details about the tribes! (same information that are in ~info function)

```markdown
~tribe [Tribe name]
```

### Artifact

This function will give basic details about the artifacts!

```markdown
~artifact [Artifact name]
```

~[img](https://cdn.discordapp.com/attachments/382038627758243841/550337149749428224/artifact.png)

### Region

This function will give basic details about the regions!

```markdown
~region [Region name]
```

NOTE: all the links are set to ts19 server (will change to ptp x2 when it starts). (Soon: you will be able to set the link url to your server on your own discord server)

~[img](https://cdn.discordapp.com/attachments/382038627758243841/550337879918903316/region.png)

### Building

This function will give basic details about the buildings! If the level is specified, it will return information about that level of the building. You can also specify a period of levels (forexample level 11 to 20)

```markdown
~building [Building name] -x[Server Speed] -mb[Main Building Level]
~building [Building name] [Level] -x[Server Speed] -mb[Main Building Level]
~building [Building name] [Starting Level] [Ending Level] -x[Server Speed] -mb[Main Building Level]

All tags that are added to the function that start with - are optional.
```

![img](https://cdn.discordapp.com/attachments/382038627758243841/550340057609797652/building2.png)

NOTE: For the period use the first level is also counted. For example in
```markdown
~building treasury 11 20
```
level 11 is also counted and its returning the total cost and train time of levels 11 to 20.

![img](https://cdn.discordapp.com/attachments/382038627758243841/550339952735682570/building3.png)

### Incoming

This function is useful to detect the slowest troop in an incoming attack. You must use this function as soon as the attack appears on the screen or you see it appearing. This function returns the top 10 matches in troop speed. Also it can detect the enemy TS level.

```markdown
~incoming [Time in xx:xx:xx format] [Attacker Tribe] [Coordinates A] [Coordinates B] -x[Server Speed] -ts[TS level (optional)] -haste[Haste Artifact Rate (optional)] -(boot|merc)[Tire (optional)] -spur[Tire (optional)] -(hero|items) -all

All tags that are added to the function that start with - are optional. About them pay attention that:

1. All optional values for tags are for more specific search. forexample if you use -ts20 the function will only assume that the attacker has ts level 20. if you don't write the number (if you write -ts) it will search for all ts levels.

2. The valid values for server speed is all integers > 0. The valid values for ts option is 1 to 20. The valid values for haste option are 1, 1.5 and 2

3. -boot or -merc will consider a Mercenary/Warrior/Archon boots and will assume the hero is with troops. The valid values for this option are 1,2 or 3 (the tier of the boot)

4. -spur is for Spurs boots and will assume hero is with the troops and is mounted. The valid values for this option are 1,2 or 3 (the tier of the boot)

5. You can simply use -hero or -items to consider all boot types.

6. You can simply use -all instead of -ts, -haste and -hero. this way the function will search with all ts levels, haste types and hero items.

```

NOTE: Please input the troop speed after -x if you want the travel times to be accurate. A 5x server can have 2x troop speed. This detail is announced in server start notification on forums. If you had questions about this please ask me on the discord channel.

![img](https://cdn.discordapp.com/attachments/382038627758243841/550344627367051275/incoming.png)

### Oasis Resources

This functions calculate the amount of resource that an oasis can regenrate in a certain amount of time (ignoring what people can take from it or the maximum storage)

```markdown
~oasisres [Oasis Type Tag] [Time in minutes] -x[Server Speed]

All tags that are added to the function that start with - are optional.
```

The tags for different oasis are:

25l | 25% Lumber
50l | 50% Lumber
25c | 25% Clay
50c | 50% Clay
25i | 25% Iron
50i | 50% Iron
25w | 25% Crop (Wheat)
50w | 50% Crop
25l-25w | 25% Lumber-25% Crop
25c-25w | 25% Clay-25% Crop
25i-25w | 25% Iron-25% Crop

## Support and Contact

Travtools has expenses. Plus I need money to be able to work on it properly! become my patreon and support travtools today!

**[Become My Patreon](https://www.patreon.com/travtools)**

You can also find Travtools discord channel [here](https://discord.gg/CxKEWtE).
