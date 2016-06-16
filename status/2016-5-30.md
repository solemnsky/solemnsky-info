# solemnsky status 2016-5-30

 * solemnsky commit: `d359b3ba9a096d5c66dce26df513c44bd92e708e`
 * solemnsky.github.io commit: `b57031ae443fb61669c65e49e963122760b141fe`

# accomplishments

* Improved the site a bit. I'm going to delay any sort of launch or public visibility until we have more things working, so the site isn't a priority.
* Upgraded the client's typeface. Much more modern and readable now.
* Fixed network polling on server and client, using new pattern.
* Added network stat collection / distribution.
* Integrated scoreboard, wrote graphical representation for the client.
* Sketched and implemented the gist of our networking model -- also added diagrams to `solemnsky-info`. Implemented new multiplayer synchronization features in engine.
* Wrote entry-grade `Prop`s with networking.
* Fixed some standards in the `Sky` API to be more accessible for modding.
* Generally improved stability and added small features.
* Wrote small `Server` supporting tdm-style game with insta-kill bullets, ran demos on the remote host with up to 14 active clients. Everything seems to work fine.

# next steps

I had originally planned to introduce modding quickly, but this week ran by without giving me a break from networking. I now believe it would be prudent to make a solid multiplayer demo through a custom `Server` impl before diving into Lua, which will be a job in and of itself, given that the engine interface is still subject to change. 

I'd like to get the demo up this week -- something that can already have the 'feel' of solemnsky. Beyond improvements to the rudimentary `Props` and a improvements to the multiplayer protocol (we should have some sort of packet buffering happening on client-side), it would be smart to set flight mechanics tuning and game scales to something more sensible. Some decisions may not be indifferent to how the game is tuned, and it would be best to avoid suprises in the future.

Meanwhile, async resource loading + a map loading splash-screen (instantiating `Map` should not be `Sky`'s buisiness) are still somewhere towards the back of my mind. Hopefully I'll find time for them this week.

