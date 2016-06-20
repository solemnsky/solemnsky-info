# solemnsky status 2016-6-13

 * solemnsky commit: `07c873f7a7ae39858e04c8064617eb6771abca75`
 * solemnsky.github.io commit: `b57031ae443fb61669c65e49e963122760b141fe`

# accomplishments

Unfortunately, not a lot was accomplished since the last update. I've been stuck dealing with other things that the end of high school has had to offer -- final exams and bureaucracy mainly -- and overall I found very little time to concentrate on any solemnsky work. I did manage a few small things:

* Got the `std::thread` spec available for both the Windows and Linux builds.
* Refactored resource management to solve some unfortunate segfaults and provide asynchronous resource loading.
* Chased around a bunch of loose ends in the client design (related to the resource mangement refactoring).
* Fixed `sky::Map` loading to support (eventually) graceful failure.
* Refactored utility directory to be much more stylish.
* Switched to new SFML version.
* Started using clang for sanitization.

# next steps

I still have two exams to get through, and I won't be able to jump back into development until they're completed -- but when they are (in about two weeks), I'll start having good amounts of time for this.

To release a public alpha, we need a a few networking improvements (packet caching for interpolation), some stability checks, and a more interesting gameplay demo. To release a scripting alpha, we need a series of incremental improvements to the engine and the integration of a Lua scripting API, probably http://github.com/Rapptz/sol .

