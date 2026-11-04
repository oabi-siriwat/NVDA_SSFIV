# NVDA_SSFIV

NVDA_SSFIV makes the menus of **Ultra Street Fighter IV** (PC) speak through the **NVDA** screen reader.

It reads the text the game sends to its own menus, so you hear the exact words the moment the screen changes.

## What it reads

- Main menu, Arcade, Versus, Training, Challenge, Options and their descriptions
- Character select, with the Character Select heading and Player 2's turn
- Character customize (costume, color, personal action, win quote) and Ultra Combo select
- The pause menu in fights and in replays
- The command list for all 44 fighters. Each move is read with its buttons in words, for example "Hadoken: down down-forward forward plus punch, EX".
- Button config, sound, screen and graphics settings, voice language, player data, the local battle log
- Pop-up questions such as YES / NO

## Requirements

- Windows 10 or 11
- NVDA, running
- Ultra Street Fighter IV for PC, the build whose `SSFIV.exe` is version 2.0.0.68944. With any other build the reader does nothing.

## Install

1. Download `NVDA_SSFIV.exe` from the latest release.
2. Put it in the game folder, next to `SSFIV.exe`.
3. Start the game by running `NVDA_SSFIV.exe`. If the game is already running, the reader attaches to it.

The reader has no window and closes itself when the game closes. It doesn't change any game file.

## Updates

Each time you start NVDA_SSFIV.exe, it checks this page for a newer release before it opens the game.

- If there is one, it asks: "Download and install it now?" Answer Yes, and it replaces itself and starts the new version.
- If there isn't one, or there's no internet, the game opens as usual.

## Keys

| Key | What it does |
| --- | --- |
| Ctrl+F9 | Set KEYBOARD 1 to the author's layout and save it |
| Ctrl+F10 | Set KEYBOARD 2 to no keys, so NVDA's number pad keys can't move Player 2, and save it |
| Ctrl+F11 | Save a bug log and say "Bug log saved in the game folder" (see below) |
| Ctrl+F12 | Say the last thing again |
| Alt+Enter | The game's own full screen / window switch; the reader says which |

## Reporting a bug

When something is read wrongly or not read at all, press **Ctrl+F11** right away.

The reader saves what it saw and said in the last few minutes as `NVDA_SSFIV bug log <date time>.txt` in the game folder. When the file is written it says "Bug log saved in the game folder"; if it can't be written it says "Could not save the bug log". Open an issue on this page and attach that file, saying what you did and what you expected to hear.

Nothing is written to disk unless you press Ctrl+F11.

## Good to know

- If the game's current button layout doesn't work well, press **Ctrl+F9**, then **Ctrl+F10**. KEYBOARD 1 gets the author's layout and KEYBOARD 2 gets no keys, so NVDA's number pad keys no longer move Player 2. After that the keys work normally. Both are saved, so they stay after the game restarts.

- The page titles in the command list (Special Move, Super Combo...) are pictures, so they aren't read.
- Not walked through yet: story subtitles, stage select, results screens, the manual.
- Gamepads haven't been tested; the keyboard is fully supported.
