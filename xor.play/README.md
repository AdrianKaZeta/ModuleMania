# ModuleMania sysmodule - `xor:play`

## Important! Before using the sysmodule!

  - The memory of sysmodules is limited, so bigger audios may fail. There's no clear limit, just that some work and some don't.
  - Like I said above, sysmodules have limited memory, so it may fail when used along with other sysmodules.

## How do I use this sysmodule?

  - Save the kip and add it to your own CFW. I guess you'll already know how to add kips to the CFW you use.
  - Create a file on the root of the SD card named `xor.play.json`.
  Add there the Title IDs and the audio files to play when that title is opened.
  - Here's an example with BotW and Home Menu:
  ``` json
  {
      "0100000000001000" : "sdmc:/myaudios/play.wav",
      "01007EF00011E000" : "sdmc:/aud.mp3"
  }
  ```
  - This way, when there's nothing opened and you're in Home Menu `play.wav` file would be played, and while BotW is opened `aud.mp3` would be played (even if you're on Home Menu and the app is minimized)
  - This should work with any game, but the only system title working is the Home Menu.
  - If there's an audio set to a title id equal or lower than `0100000000001000` (Home Menu's one) the audio set to that ID will play any time there's no game opened.
  - Looks like opening hbmenu stops the audio playback, but when returning to Home Menu it should start again.
  - Any problems you have, ask them on my Discord server ([Nintendo H&H server](https://discord.gg/Qqnndqd)), or ask them on the release GBAtemp thread of ModuleMania.
