# Crosscode Notes
This will contain all my notes about the Crosscode Codebase and how it Works


## High level notes
Creating a mod for a game that's already been made is quite difficult. One of the main reasons for that is that it's already built as a singleplayer game. So the process would be to understand how the game was made and architected in the first place, and then recreating a compatible architecture with an emphasis on moddability and multiplayer.

## Modules
This section holds high level knowledge about each module and the relaxant bits from them:

- **Window.ig**: This seems to be the fundamental module that interacts with your computer
- **Impact.base.worker**: This seems to be for multi-threading where you give a worker *tasks* and it can run it's *tasks* and send messages
- **Impact.base.loader**: Defines Cacheables and Loadables, and is in charge of maintaing the Cache
- **Impact.base.image**: Base code for handling images, including the loading, drawing and updating along with helper functions
- **Impact.base.font**: Base code for font handling, which includes helper functinos, and drawing stuff.
- **Impact.base.system.web-audio**: A wrapper for *web-audio*
- **Impact.base.sound**: Base code for Sound, including a SoundManager, Music, Volume control, and more. 
- **Impact.base.timer**: A simple class for Timers and WeightedTimers
- **Impact.base.vars**: This module is essentially a fancy map with code that allows for entites and such to grap information in releavent filepath like pieces of information. That also has some unique feartures like Accessors.
- **Impact.base.System**: This module is what interacts with your system, and sends things that need to change from there.
- **Impact.base.input**: adds all the different kinds of input and listeners to the game
- **Impact.base.lang**: adds support for the lang resourcing so that labels can be used and changing the languge isn't triple the work
- **Impact.base.impact**: the wrapper for all the engine code (above) also has the main method. 

# Game Loop
**ADD DESCRIPTION**

# Events/Steps/Actions
**ADD DESCRIPTION**
