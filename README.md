# Flash Confetti Class

A generic and flexible Flash Confetti class that generates and displays the effect of randomly-falling confetti.

### Notes

- Overall, the class automatically assigns random X coordinates, fall times, delays, scale, alpha, rotation, and tint (if colors are specified) for the effect of true randomness and depth of field.
- To import, instantiate, and start a batch of confetti in the file, only 4 lines of code are needed.
- There is a public `start()` method for the class, rather than having the class auto-start (though the demo below does auto-start, but that is through the parent file, not the class).  This is done in an effort to save in performance.  There are also public methods for `stop()`, `clear()`, and `remove()`, done in an effort to to be able to phase out the confetti (stop), clear all current instances of individual confetti pieces (clear), or stop and clear out all confetti pieces (remove).
- The class is set up to pass in an Object as the parameter when creating your Confetti object, which takes up to 6 optional attributes: `width`, `height`, `colors`, `maxPieces`, `symbol`, and `speed`.  If any or all of these are not defined, default values will be used.  Through much time and testing, calculations were solidified to make for realistic default settings.
- The class allows for passing in a custom symbol to use, rather than using the auto-generated one. This can be done with instances of MovieClips from the Library, set to export to ActionScript. These custom MovieClip symbols can have multiple frames, too.  If a MovieClip symbol has multiple frames, the class will randomly assign a frame to show for each individual piece.
