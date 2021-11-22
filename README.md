⚠️ **WARNING:** This README is currently incomplete, This warning will be removed once it's complete.

# Friday Night Funkin' - Sword Engine
Sword Engine is based off of Psych Engine, which was originally used on the [Mind Games Mod](https://gamebanana.com/mods/301107), it's intended to be a fix for the vanilla version's many issues while keeping the casual play aspect of it. Also aiming to be an easier alternative to newbie coders.

## Compiling:
Follow a Friday Night Funkin' source code compilation tutorial, after this you will need to install LuaJIT.

**I would recommend following the compile guide at:**
[The Original Funkin Game's Github](https://github.com/ninjamuffin99/Funkin)

Scroll down to the "build instructions" section and go from there.

***MAKE SURE TO DOWNLOAD THE SOURCE CODE FOR THIS ENGINE AND NOT THE ORIGINAL BASE GAME FIRST.***

One last thing, you will need to install LuaJIT along with the other libraries such as `flixel-addons` and etc.

You can do this with: `haxelib install linc_luajit` on a Command prompt/PowerShell

...Or if you don't want your mod to be able to run .lua scripts (why), delete the "LUA_ALLOWED" line on Project.xml

## Downloading:
Go to the releases tab lol

# Psych Engine Credits

## Credits:
* Shadow Mario - Coding
* RiverOaken - Arts and Animations

### Special Thanks
* Keoiki - Note Splash Animations

# Sword Engine Credits
## Credits:
* swordcube - the only dev Lol

WARNING: This engine is still in very early development, Requesting new somewhat ***SIMPLE*** features would help alot.
_____________________________________

# Sword Engine Features

## Score Text Change
* Accuracy is now split up from the rating.
* There are 2 ratings, a accuracy rating and another one.

### Rating 1:
* Rating 1 is S++ - F, changes depending on your accuracy.

### Rating 2:
* Rating 2 changes depending on some factors:
* If you are FC'ing a song with all Sicks, you will get "MFC" (Marvelous Full Combo)
* If you are FC'ing a song with Goods and Sicks, you will get "GFC" (Good Full Combo)
* If you are FC'ing a song with Goods, Sicks, and Bads/Shits, you will get "FC" (Full Combo)
* If you have less than 10 misses you will get "SDCB" (Single Digit Combo Breaks)
* If you have 10 misses or more you will get "Clear"

## Optimization Mode
For some reason this is SUPER FUCKY on Windows and i have zero clue why, it pisses me off so much

Basically this just removes backgrounds and characters, This SHOULD be something you can use in Lua but i don't know how `FunkinLua.hx` works lmao

Not like i could test anyways, i'm on Linux for fuck's sake.

_____________________________________

## To-do list:
* > [WORKING ON THIS] Note Skins in the options menu [Hell]
* [NO PROGRESS YET] Speed feature for songs [Hell, but probably will be a copy paste]
* [NO PROGRESS YET] Extra keys [TRUE HELL, MIGHT NOT EVEN BE ADDED LOL]
* [NO PROGRESS YET]Custom difficulties without source [Hell]
* [NO PROGRESS YET] Skip song & Skip intro in Pause Menu only because fuck Skip Intro being in gameplay
_____________________________________

## A little note

oh yeah sword engine is based off of an early version of psych engine 0.5 so i'ma have to add everything from the new official release at some point
probably won't tho because i might forget lol
_____________________________________

# Psych Engine Features

## Attractive animated dialogue boxes:

![](https://user-images.githubusercontent.com/44785097/127706669-71cd5cdb-5c2a-4ecc-871b-98a276ae8070.gif)


## Atleast one change to every week:
### Week 1:
  * New Dad Left sing sprite 
  * Unused stage lights are now used
### Week 2:
  * Both BF and Skid & Pump does "Hey!" animations
  * Thunders does a quick light flash and zooms the camera in slightly
  * Added a quick transition/cutscene to Monster
### Week 3:
  * BF does "Hey!" during Philly Nice
  * Blammed has a cool new colors flash during that sick part of the song
### Week 4:
  * Better hair physics for Mom/Boyfriend (Maybe even slightly better than Week 7's :eyes:)
  * Henchmen die during all songs. Yeah :(
### Week 5:
  * Bottom Boppers and GF does "Hey!" animations during Cocoa and Eggnog
  * On Winter Horrorland, GF bops her head slower in some parts of the song.
### Week 6:
  * On Thorns, the HUD is hidden during the cutscene
  * Also there's the Background girls being spooky during the "Hey!" parts of the Instrumental

## Cool new Chart Editor changes and countless bug fixes
![](https://i.imgur.com/h6Ja7eT.png)
* You can now chart "Event" notes, which are bookmarks that trigger specific actions that usually were hardcoded on the vanilla version of the game.
* Your song's BPM can now have decimal values
* You can manually adjust a Note's strum time if you're really going for milisecond precision
* You can change a note's type on the Editor, it comes with two example types:
  * Alt Animation: Forces an alt animation to play, useful for songs like Ugh/Stress
  * Hey: Forces a "Hey" animation instead of the base Sing animation, if Boyfriend hits this note, Girlfriend will do a "Hey!" too.

## Improved Animation Debug menu (Press 8 in-game on a Debug build)
![](https://user-images.githubusercontent.com/44785097/127721062-f912853c-2513-41b8-bd66-fd80d9d4ee0f.png)
* You can now press Save Offsets to save a .txt file with the editted offsets
* You can also now change the characters while on the Menu
* Go back to the game by pressing Escape
NOTE: This should be used for fixing your character floating or being slightly under the ground! It's not for texture editting.

## Story mode menu rework:
![](https://i.imgur.com/UB2EKpV.png)
* Added a different BG to every song (less Tutorial)
* All menu characters are now in individual spritesheets, makes modding it easier.

## Credits menu
![](https://i.imgur.com/NdIQt3d.png)
* You can add a head icon, name, description and a Redirect link for when the player presses Enter while the item is currently selected.

## Awards/Achievements
* The engine comes with 16 example achievements that you can mess with and learn how it works (Check Achievements.hx and search for "checkForAchievement" on PlayState.hx)

## Options menu:
* You can change Note colors, Controls and Preferences there.
 * On Preferences you can toggle Downscroll, Anti-Aliasing, Framerate, Low Quality, Note Splashes, Hide Hud elements, Flashing Lights, etc.

## Other gameplay features:
* When the enemy hits a note, it plays the note hit animation on their strum, just like when the player hits a note.
* Lag doesn't impact the camera movement and player icon scaling anymore.
* Some stuff based on Week 7's changes has been put in (Background colors on Freeplay, Note splashes)
* You can reset your Score on Freeplay/Story Mode by pressing Reset button.
* You can listen to a song on Freeplay by pressing Space once.
