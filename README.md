# Ark-of-Klei
An attempt to make a semi-casual voxel game with a fully simulated ecosystem. (I'll be using Luanti as the base engine.) 

<details>

<summary>General Pitch</summary>

So basically, I want to make a FOSS game that will make normies want to play it even *before* they learn that it's free.
(It would be nice if I could enjoy it too- I actually find most games fairly boring.)
To do that, it should be fairly polished, and have significant novelty. 
There's tons of games out there whose sole purpose, effectively, is to let players *watch* some kind of sumlation unfold.
So surely, being able to walk around an interact with simulation would take it over the top, right? 
That simple premise is the heart of this game- most other elements are just there to make the interaction fun and accesible.

Big thanks to Klei Wright, whose excellent [video essay](https://www.youtube.com/watch?v=f21YJ5pjPog) is what ultimately inspired this project.

</details>

<details>
   <summary>The Hook</summary>
The year is 3027, and the Ark of Klei is cruising through space with some important cargo: an entire live ecosystem, destined for the colonies. 
The ship itself is completely self-maintaing, but the Ecological Zone can be a little... unpredictable. 
That's largely the point, but it can sometimes be an issue: in particular, the weather monitoring stations are prone to chewed cables, nesting critters, 
and, ironically, storm damage.

That's where you come in! I know you've been enjoying your time in the digital crew storage, but now it's time to download your mind into a fresh body,
venture into the ecological zone, and figure out how to repair the damaged weather station. When you're finished, kindly report to the disintegration
chamber to have your mind re-uploaded to digital crew storage. What's that? You don't "want" to be disintegrated? 

You want to... live a peaceful life amongst the plants and animals in the EZ? Uh... sure. Fine. Just don't screw the place up: there's a lot riding on
this thing arriving to the colonies intact. 
   
</details>

<details>
   <summary>The Spaceship</summary>
   Originally the spaceship was just an excuse to have a finite world size, but right now I think it's actually a pretty key component of the game's overall vibes.
   For the most part, everything in the "ship" part of the game is essentially Clark-Tech that just works, no matter what. Players can't mine through the hull, the gravity controls can't spontaneously malfunction (or can they? 🤔), and there's no danger of the body-synthesis chamber breaking somehow. (otherwise, the player wouldn't be able to respawn!)
   The neat thing about using a spaceship is that it gives plenty of room to add gameplay stuff that not make sense otherwise. For example, we could add a holodeck down the road that allows the player to take a break from the survival stuff and import dungeons or do creative testing. Or how about am examination chamber that essentially functions as a movement tutorial?
   Probably the most important features though are:
      <details>
      <summary>Body synthesis chamber</summary> 
         This essentially functions as the spawn point. Unlike other games, you can't casually reset your spawn (or skip the night for that matter) by simply laying down in a bed. That means that although the game's overall vibe is casual, you should still take care not to die- walking all the way back would be a pain! Of course, if setting your spawn really matters to you, you can always check out a portable synthesizer. (There's a control room for the day-night cycle, too.)</details>
   <details><summary>Check-out System</summary> 
      Yes, there's some good depth to the survival and building system. You *can* dig a charcoal pit with your bare hands, make some charcoal, and then use that charcoal to forge a steel pickaxe and shovel. Or, you can just check out a multi-tool from the crew locker. You're here to work, remember? Of course, you can only check out a small number of items at a time, so players will have to think about what they really want/need. 
   </details>
</details>

<details>
   <summary>The Ecological Zone</summary>
   This is the heart of the game! The Ecological Zone, at it's core, is really just a 3D wolf & rabbit simulation, with some added complexity. The final version will probably feature a few dozen plants, animals, and fungi, plus some modest geological complexity, and maybe some dynamic weather? 
   The Zone will have various features and areas (like a lake for example, or an area that's always shaded), but is essentially one continous biome. Maybe in the future, we can design different Arks that have different ecology.
   Before we can design the first one though, we need to know what kind of tools we'll be able to work with. (See Gangbuster Features.) Anyway here's some key features:
   <details>
      <summary>Large, but Finite</summary>
   I'm thinking, roughly, that the ecological zone should be about 1km across, and maybe half that in height? THis is for both technical and gameplay reasons. From a technical perspective, we need a finite size in order to be able to keep the entire simulation loaded. If the wolves and rabbits aren't running around doing stuff, then it's not a functioning simulation! On the other hand, it should be fairly large, or else the ecosystem won't be stable.
      From a gameplay perspective, the large size provides a period of wondrous exploration. But eventually, the player starts to see the edges, and it sinks in: this is it. If you burn the forest down, you can't just wander a few hundred blocks over and find a different one. If you want to live here, you have to take care of this place.
   </details>
</details>

<details>
   <summary>Vibe Notes and Features</summary>
   <details>
   <summary>Three-Ring Binders</summary>
   Believe it or not, this is one of the most important features in the game! They do a few things for us:
      
      -Immersion. If you've ever worked a job where you maintain critical machinery, 
      then you know 3-ring binders are king!
      
      -Documentation. Good documentation is key to accesibility, and dare I say fun? 
      Plus, some of the text from these can be put onto an online wiki, which is good for visibility.
      
      -Unique puzzling. Having myself work a job maintaining key infrastructure, 
      I can say that finding the part of the documentation that gives you that
      "aha" moment is indeed a special feeling. By having good documentation, 
      this game can have puzles in it that are uncommon in other games. 
      (Like the weather monitoring station that I mentioned in The Hook chapter.)
      
</details>
   <details>
      <summary>Semi-Casual Survival</summary>
      With regards to survival gameplay, games like Vintage Story or Exile try to keep you in the bootstrapping phase for as long as possible. Minecraft, on the other hand, has a great endgame, where the world is essentially an open canvas. Then there's the middle phase: There's plenty of important stuff to do, but at least you have the basic tools to do it with. This game is meant to drop you off right in the middle phase, and keep you there.
   </details>
   </details>

<details>
   <summary>Gangbuster Features</summary>
   These are features that I think will really add to the simulation, but may be difficult to pull off. They need to be evaluate before the ecology can really be designed, so that we know what kind of ecology is even possible.
   <details><summary>Conservation of Matter and Energy</summary>
      Sunlight enters the system, and plants combine it with nutrients to make plant matter. Animals eat the plants, and other animals eat those... when animals die, decomposers turn the carcass back into nutrients. It's all tracked- nothing "spawns in" or mysteriously vanishes. If the players drops leaves on the ground, they don't despawn: they're a part of the ecosystem now. Sticking to this principal is one of the key features that make this game's ecology different from the ecology in other voxel games.
   </details>
   <details><summary>Keeping it all Running</summary>
      If the Wolves and Rabbits aren't running around, and the plants aren't growing, then it's not really a simulation. There has to be a way to keep the key parts functioning, even when the player isn't around. Luckily, the Luanti engine has a set of tools called "VoxelManip" which can manipulate large batches of voxels, even when they aren't loaded. Clever useage of this tool should have the plants covered, at least, assuming that the enginge can keep up with it being run routinely. If there's a similar batch feature for entities, then we might be in business. 😎
   </details>
   <details><summary>Bugs (By which I mean insects)</summary>
   A healthy ecosytem, in the real world, needs bugs. They also liven up the place! But they might need to work a little differently than the macro-mobs. Like for example, if locusts are in the game, they kind of need to swarm for real, and in large numbers. (By the way: did you know that in real life, locusts come from grasshoppers? When they're low on protein, they transform into locusts to seek it out. And escape from the other locusts...)  
   </details>
   <details><summary>Fluid Dynamics</summary>
   If this can be done, even in a rudimentary form, it would add a lot of depth to the simulation. Calories can already be tracked throughout the system, but now, so can water! Expand that to temparature and humidity tracking, and now you have dynamic weather as well. Might be too much for the simulation to handle, but I know the existing dynamic liquids mod actually has something similar to this. (Just the flowing water part.) 
   </details>
   <details>
   <summary>Mixed Nodes and Composit Nodes</summary>
      Two different, but related topics. So firstly, imagine you have a groundcover flower that only takes up part of a node. It's pretty easy to make it so you can place it multiple times, and have it cluster up; you basically just need to make a few variations. Say, 4. But what if you have a *different* ground cover flower that only takes up part of a block? It would be pretty sick if they could be together, right? If there's a way to somehow handle that on the fly, then it could be expanded to half-slabs, arbitrary-liquid-logged fences, and even placing a torch and ladder on the same block. Admittedly, this does more to make the simulation *feel* alive than actually *be* alive, but it would still affect the type of ecology that can be planned for. (Plus, I've been wanting the torch and ladder thing for years.)

On the other hand, water strikes again! If we really want a full water cycle, then ideally we should be able to track the way that humidity moves through air blocks, and creeps through soil. If we want turing-complete geology, we need to be able to handle nodes with arbitrary compositions of particle size, moisture, and ... composition. (Like, what percentage of silica, metals, etc) If the number of possible states is "relatively small," then the best approach might just be to make a big table of all possible states (with textures for each 😵‍💫), and use the aforementioned VoxelManip to handle everything. Otherwise... 
The cool thing about pulling off arbitrary states though is that it could apply to liquids too. Water could erode soil, and deposit it elsewhere, for example. Or, the player could do chemistry in arbitrarily large in-world cauldrons. Although technically, I guess the "predefined table of all possible nodes" could work for this, too.  

As far simulating the ecology goes, though: being able to track the spread of roots through dirt means that plants can reproduce via rhizomes. In addition to being cool, it would also add to the resilience of the ecosystem. But what if there's also a mushroom trying to spread its mycelia?? 

Also, in terms of game play: being able to do stuff like place multiple sticks together would allow for some really smooth in-world crafting. And imagine being able to run *two* mesecon lines on the same block!
   </details>
   <details><summary>Tree Felling</summary>
      There's lots of games where chopping a single log causes the whole tree to break. What I'd really like though, is for the tree to *fall over.* It's a "small" thing, but I think it would add a lot to the feeling of liveliness. Potentially the code could be repurposed for other stuff, too.
   </details>
   <details>
    <summary>Dynamic Lighting</summary>
   Energy enters the system through sunlight, which is a type of light. If dynamic lighting can be implemented, it means the simulation can dynamically calculate which plants can grow where, and how fast, even if new trees grow or new light sources are added. (Like if the player uses grow lights for example.) 
</details>
</details>
<details>
   <summary>Features to Worry About Later</summary>
   These are features that I'm pretty confident can be pulled off, but aren't key right now.
   <details>
      <summary>Hotbar Improvements</summary>
   Hotbars can be a bit fiddly in these kinds of games. For example, if I put bricks in slot 1, and place all those bricks, I now have an empty slot that will be filled by whatver the next thing I pick up is. Ideally, I'd like the hotbar to function more like a *toolbar,* and most of the gameplay (including crafting) to take place in-world. </details>
   <details>
   <summary>Cool Art</summary>
      I don't mind commisioning an artist, but the gameplay needs to be nailed first so I know what assets are needed.
      </details>
   <details>
      <summary>Fun Tools</summary>
      Like, jetpacks and stuff. Why not?
   </details>
   <details><summary>Descriptive Names</summary>
      Instead of just telling you what block you've picked up or are looking at, the game will have a description, like "white stone" or "small bird."
      This means that there's a process of learning what things are from the 3-ring binders (or multimeter), and then identifying them yourself them in the wild. Just like birdwatching in real life, I imagine this small detail will make the game just that much slightly more magical. 
   </details>
   <details>
      <summary>Discrete Machinery (Plus philosophical rant?)</summary>
      In order for fixing stuff to be fun, machines (and stuff in general) should be made of smaller components. To use the weather station example again:
      if you just have single "weather observation" block, then that block is either working, or it isn't. What is there to engage with, as a player? This isn't just limited to the hook though: it's kind of a microcosm of the game in general. This game isn't like a typical casual voxel game, where the world is essentially an inert canvas for you to build on. But it also isn't like a hardcore survival game, where the challenge comes from bootstrapping a living from the raw earth. Here, it's relatively easy to survive and get things working, but the challenge comes from reacting to a dynamic world. 
      Of course, figuring out how the tech works, exactly, is a future problem. Ecology first!
   </details>
   <details>
      <summary>Movement Mechanics</summary>
      Moving around should feel good. If 1-block ledges are common for example, the character should auto-step up them.
   </details>
   <details><summary>Maintenence Tasks</summary>
   This game doesn't have "quests-" you're not an adventurer. Things might need attention from time to time, though, like the aforementioned weather stations. If you're up, you might as well fix them. Some of these might be scripted, but others might happen dynamically. For example, if a storm blows down a tree so that it blocks one of the entrances, you would have to clear it. 
   </details>
   <details><summary>Standalone Package</summary>
   If the game gets to be really polished, it might be nice to make a standalone download so it's slightly easier for people to get ahold of. 
   </details>
</details>
