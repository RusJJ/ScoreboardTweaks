# What is this mod?
ScoreboardTweaks is a simple (maybe) mod that changes your Scoreboard to be more comfortable and more understandable (MAYBE???)

Changes:
- Bigger text for buttons
- Color square and Mute button (and also voice icon) are the same! To mute a player just press on a square!
- Voice icon changes itself to "Voice Muted" icon
- Report buttons changed their positions: under the Report button there is Cancel button (its more logical)
- Report buttons are a bit gray (to split them from the other buttons that modders can add)

## Manual Installation
Be sure that you are already installed BepInEx (using MonkeModManager for example). You need x64 version. [Take it there.](https://github.com/BepInEx/BepInEx/releases)

Unpack downloaded ZIP Archive to your GorillaTag game folder and you're ready to play!

If you're scared then copy DLL and PNG files to your Gorilla Tag/BepInEx/plugins folder somewhere (Gorilla Tag/BepInEx/ScoreboardTweaks/ for example).

## For modders
You can use that mod without hard dependency! You can work with those scoreboard buttons by your own if there's no ScoreboardTweakers installed.

Here are 3 functions for that. They should be in a mod-class:

 - void OnScoreboardTweakerStart() <- Will be called on ScoreboardTweaks::Start() so you know it's installed
 - void OnScoreboardTweakerProcessedPre(GameObject scoreboardLinePrefab) <- Will be called before ScoreboardTweaks does it's magic
 - void OnScoreboardTweakerProcessed(GameObject scoreboardLinePrefab) <- After

## How that looks? (ignore green color of my name, that's a different mod)
![image](https://user-images.githubusercontent.com/8864329/125429323-6e4ffc6d-570f-4d69-8243-241f5d73bab6.png)
