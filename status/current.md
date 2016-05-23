# solemnsky status 2016-5-23

 * solemnsky commit: `02871d27d94b71a54cf2aa006a409a043617654d`
 * solemnsky.github.io commit: `59941a1ed3c2d2a8b1f638f01188388c83904655`

This is our second solemnsky status update! I think that for the most part I'll be updating
 on a weekly basis from now on.

# accomplishments

Outline of the changes made during the week since the last update:

* Moved documentation / status reports into new repository, solemnsky-info.
* Wrote more documentation; documented engine and server, added and fixed diagrams.
* Followed up with changes to a part of the engine design: Sky is now a subsystem, SkyHandle's tasks are much simpler, and game state invariants are clearer -- separately networked components are no longer inter-dependent.
* Refactored the client (particularly `MultiplayerCore`) to be simpler and adhere to the new design.
* Put `Game` information into an improved debug overlay.
* Started work on the new site -- got new member of the team (welcome airballer), sketched the design, made a logo, and wrote a demo homepage.
* Introduced the `Scoreboard` subsystem to manage score data with a separate networking strategy.
* Extracted some geometry / graphics data from altitude maps!
* Added serialization of `Map`s through cereal (JSON archive), created our first non-trivial map (a copy of `ball_asteriods` without graphics).
* Added support for non-convex map obstacles, sourced and adjusted a triangulation lib.
* Ran our first inter-continental multiplayer game. Woo.

# next steps

The site should to be edited and published, in order to start pitching the project to 
 more potential collaborators.

I need to add a host of small features to the client; also, develop some aspects of the
 networking system (e.g. filtering of packets by latency) and put the network sync
 design I've been dreaming up into place. I'm planning on diverging from Altitude's "annoying"
 totally-authoritative clients to a partial degree, while keeping some of the benefits this
 approach offers.

Additionally, we'll need async resource loading for maps, and will probably want to 
 substitute our static resource loading with it... perhaps we'll make a nice 
 loading screen while we're at it too.

Finally, to speak of scripting: it would be prudent to start putting writing up some 
 hello-world scripting demos -- probably in Lua?

