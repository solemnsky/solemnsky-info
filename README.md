# solemnsky information

This repository holds information about the solemnsky project that's useful to humans.

 * `docs/` contains a brief manual of the solemnsky engine and eventual modding API
 * `status/` contains an set of past and current status updates for the project as a whole

## first development alpha release

As of the moment that I write this, I've sketched support for almost every fundamental feature that we'll need in the final product. In order to become more attractive to potential contributors and avoid any over-extension of our limited resources -- my time and our team's interest in the project -- it would be prudent to aim at a near-future goal: presenting a development alpha release.

By the development alpha release, I plan to have a highly usable client/server system, with a concrete set of foundations for all that will come. It will be playable and presentable, and prepare the ground for the addition of scripting.

A list of the foreseeable developments necessary to reach this point follows.

* Client UI 
  * Should leave a good first impression, and be intuitive and functional. 
  * Should have useful settings, with support for persistence.
* Environment (.sky) Format. 
  * Should be constructible from altitude's maps with an automated tool. 
  * Should be easy to add custom game graphics to.
* Engine 
  * Should be improved to allow the server's implementation of a basic TBD-like mode.
* Engine Sandbox 
  * Should allow experimenting with engine tuning values. 
  * Should allow testing of environments with minimal overhead.
* Multiplayer Client 
  * Should display lobby, environment loading, game, and score screens.
* Multiplayer Server 
  * Should implement a basic TBD-like mode.
* Multiplayer 
  * Should employ packet buffering to compensate latency fluctuation in `SkyDelta` (dynamic game state) packets, on both client and server.

