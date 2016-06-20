# solemnsky status 2016-6-20

 * solemnsky commit: `489b61c465abf8e12c42d96f027e91cb7ca7ced2`
 * solemnsky.github.io commit: `b57031ae443fb61669c65e49e963122760b141fe`

# accomplishments

I still have one exam to get through, but I started my summer re-entry into solemnsky development during the past week.

* Reorganized source directories (subdivided the increasingly large engine directory), changed C++ header files to use the more correct .hpp extension.
* Improved client, refactored `appState` into the clearer and more correct `refereces` struct.
* Made asynchronous resource loading work for the client.
* Introduced the grand `Environment` struct! Maps, scripts, and graphics will be loadable asynchronously into these objects.
* Refactored engine to support asynchronous loading of `Environment` -- `SkyHandle` now has less responsibilities, since the instantiation of `Sky` isn't directly linked with a synchronous process. (The environment's map can take time to load!)
* Started refactorization of protocol to support `Environment` loading.
* Improved debugging display, brought `DebugView` back. Generally improved nature of debug prints.
* Converted "tutorial" into precursor of a featureful sandbox, for testing engine values / environments.
* General client/ codebase improvements
* Started looking for archiving library to store / load Environments (in the form of .sky files) from disk.

# next steps

* Find a decent way to manage disk archives -- you'd think there would be at least one tar library written in modern C++, but apparently this is not the case.
* Continue fixing up multiplayer protocol, reintroduce multiplayer.
* Extend `Environment`, make tools for rendering grape's graphics directly to entity sheets.
* Add environment loading screen for multiplayer client.
* Move towards the first development alpha release.

