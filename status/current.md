# solemnsky status 2016-7-21

 * solemnsky commit: `dd942ec210e4a2940bc1168024db18efd3fcd90c`
 * solemnsky.github.io commit: `2c68e042bed772174a648b13d281b166724f54ef`

# accomplishments

Another two-week status jump. Summer has begun and I no longer have any serious obligations. But it's .. so warm. It's a challenge to keep an integral work schedule for solemnsky. My only hope is to get into a routine. Glenn (couleeapps)  is poking around solemnsky now and then, so I should get some welcome aid with C++. Lasoloz, meanwhile, has dropped from the team presently, due to academic obligations -- best of luck to him.

 * Fixed travis build.
 * Added a handful of github issues for the development alpha release, put them in a milestone.
 * General UI improvements:
    * Added `Transformed` wrapper control for easier management of UI components with spacial transformations.
    * Improved page animations and positioning.
    * Moved close game and close page buttons, to the bottom of the screen, gave them more space.
    * Put together a new color scheme, a bit more professional looking and easier on the eyes.
    * Using a new menu background -- clouds!
    * Made various fixes and color tunings.
    * Cleaned and fixed stylesheet.
  * Client improvements:
    * Introduced the `MessageInteraction` UI object, a more featureful version of the message entry / message log display combo for sandbox and client alike.
    * Saving client settings in file.
    * Cleaned a lot of code, especially surrounding `ClientShared`, to be more purposeful and restrictive.
    * User-supplied remote server IP.
    * Fixed implementation of protocol
    * Added commands for testing tuning values in the sandbox.
    * 
  * Engine improvements:
    * New, less confusing management of the environment load flag (in network deltas and initializers).
    * Better logging and implementation of environment loading.
    * Added types.hpp for faster engine compile via more selective includes.
    * Split up files on Glenn's recommendation.
    * Teams are no longer unsigned chars. Maybe a good idea.
  * Server improvements:
    * Spectators are automatically assigned a team by the vanilla server layer when they try to join during a game.
  * Util improvements:
    * Improved `Archive` et all -- cleaner logging, multiple processes in same directory, etc.
  * Various other improvements that it would be increasingly gratuitous to list here.

I just basically need to write a lot more code.
  
# next steps

  * Continue checking off boxes for the alpha demo development thing.

