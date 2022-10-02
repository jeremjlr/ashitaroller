# ashitaroller
FFXI Addon for Ashita - Automated COR Rolling

- Original windower addon : not available anymore
- Ashita port this is based on : https://github.com/towbes/ffxi/tree/master/ashitaroller

## Features
- Automatic corsair rolling
- Can use Crooked Cards, Fold, Snake Eye and Random Deal
- Crooked Cards can be focus on one roll or be used for both, Random Deal can be disabled
- Stops on zones
- Normal mode to put good rolls up asap (i.e : Quick ambu runs), Gamble mode to try and maintain double 11's abusing bust immunity (i.e : ML grind)

## Commands
- On/Start/Go/Enable/On/Engage - Start rolling  
- Stop/Off/Quit/End/Disable/Disengage - Stop rolling  
- roll1 <roll> (can use beginning of roll name ie: cor = corsair's, or stat)
- roll2 <roll>
- engaged on/off - Enable or disable only rolling while engaged
- crooked2 on/off - Allows Crooked Cards to also be used for the second roll
- randomdeal on/off - Allows Random Deal to be used
- oldrandomdeal on/off - on;focuses on resetting Snake Eye/Fold, off;focuses on resetting Crooked Cards
- gamble on/off - Abuses bust immunity to try to get double 11's as much as possible
- partyalert on/off - Writes a message in /party a few seconds before rolling

## Recommendations
- Quick Ambu runs (Normal mode) : crooked2 on/random deal on/oldrandomdeal off/gamble off
- ML party (Gamble mode) : COR(roll1)/SAM(roll2)/crooked2 off/random deal on/oldrandomdeal on/gamble on

## v0.3 Patch Notes

- Fixed issues that would lead to snake eye being ignored when it should be used
- Snake Eye can now go for lucky rolls as well as 11's
- Fixed an issue with snake eye not being used for samurai's unlucky roll (6)
- Fixed issues that would lead to crooked rolls getting busted for no reason
- Fixed issues that would lead to random deal being used in the middle of rolls causing unexpected behavior
- Fixed an issue that would lead to abnormal waiting time in between rolls when busting
- Fixed a bug that made it impossible to hide the UI
- Fixed a bug that would lead to incorrect debug messages
- Changed random deal so it can also be used for crooked cards in between rolls
- Made it so crooked cards can also be used for roll 2
- Added a command to keep the old random deal behavior (use random deal for fold/snake eye) /oldrandomdeal on/off
- Added a command to never use crooked on roll 2 /crooked2 on/off
- Added a command to prevent the bot from using random deal at all (in case it musts be saved for later in the fight) /randomdeal on/off
- Added a command to let your party know that you're about to roll /partyalert on/off
- Added debug messages that explain the decision making when rolling
- Added new flags to the ingame UI

- Normal mode (better when paired with oldrandomdeal off) will focus on getting rolls up quickly focusing on Crooked/LuckyRolls using Random Deal to reset Crooked Cards. It is generally better for quick ambuscades and such.
- Gamble mode (better when paired with oldrandomdeal on) will give less importance to Crooked/LuckyRolls and focus on getting 11's using SnakeEye/Fold and abusing bust immunity. Might be better if you want to focus on keeping double 11 for whatever reason.

