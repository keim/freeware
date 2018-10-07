====================================================================
Nomltest FS ver 1.0.1
  Free Soft for Windows 98/me/2000/XP
  Created by Kei Mesuda (HN; keim)
====================================================================

Thank you for downloading this game.
This game is Free-Soft.

The newest version will be download here.
http://www.yomogi.sakura.ne.jp/~si/ 

[ About this game ]
  This is Shotem up game with 'bullet eating system'.

[ How to Install ] 
  Unpack zip file. And execute 'nomltest_fs.exe'.
  If your display don't support QVGA, execute 'nomltest_fw.exe'.

[ How to Uninstall ] 
  Delete all files. This software don't rewrite registry files.

[ Required Environment ]
  OSÅG Windows98/2000/XP (Not Tested; Windows95/NT/me)
  CPU; Over PentiumII 300MHz

[ Copyright ]
  Copyright 2004 Kei Mesuda All rights reserved. 
  I have no responsibility for your trouble with this game and manual.

[ Special Thanks ]
  Simple Directmedia Layer(SDL) is used in this software.
    SDL(Simple Directmedia Layer) http://www.libsdl.org/
    'sdl.dll' is under LGPL License.
    SDL Licensing                 http://www.libsdl.org/license.php
    
  Software Synth T'SoundSystem(T'SS) is used in this software.
  T'SoundSystem(T'SS) 'nptss.dll' is created by Toyoshima House.
  Special Thanks to Toyoshima House.
    Toyoshima House  http://www.toyoshima-house.net/
    
[ Support ] 
  mail; keim@nona.dti.ne.jp
  web;  http://www.yomogi.sakura.ne.jp/~si/

[ Bug Information ]
  2005.03.27
  Replay Data for "KUIDAORE Mode" cannot execute. Sorry.





//----------------------------------------
// Nomltest FS ver 1.0.1
// Manual
//----------------------------------------
- How to play.
  Play with a Keyboard or Joystick.
  Movement; Allow Key
  Shot; [Z]/[X]/[C] ([C] key is used only in Additional Mode)
Å@Pause; [P]
  Exit; [Esc]Å@
  (You can change this setting by rewriting "key.conf".)

- System
  - EAT System
    When you stay bullets within the blue square field for a certain period of time, 
    The bullets disappeared. This rule is called 'EAT System'.
  - Shot
    Shot[Z]     ; Wide Forward Shot. Mobility;Fast.   Aggressivity;Middle. Range:Middle. Eating Range; Middle.
    Shot[X]     ; Wide Shot.         Mobility;Middle. Aggressivity;Light.  Range:Wide.   Eating Range; Small.
    Shot[Z]+[X] ; Forward Shot.      Mobility;Slow.   Aggressivity;Heavy.  Range:Narrow. Eating Range; Large.
  - Bonus
    Shoot down small enemy; 10-60[points / enemy].
    Shoot down all of the small enemies in a formation group; 2000[points /10 enemies].
    Shoot down small enemy flying alone; 1000[points / enemy].
    Shoot down big enemy; 3000[points / enemy].
    EAT bullet; 10-500[points / bullet]
  - EAT Bonus rules
    min;10[points], max;500[points]
    Initial EAT Bonus; 20[points]
    Shoot down all of the small enemies in a formation group; +20[points]
    Failing to shoot down all in a formation group; -20[points]
    Miss; -160[points], (If EATing Bonus < 320[points], Go down by half.)
Å@- Extend Ship
    Extend by 200,000[points].
  - Difficulty
    Difficulty increases by play time and EAT count. 
    The increasing rate is 11[levels / min.] by play time. 
    And 0.036[level / bullet] by EAT count.
    Also, over level 150, a white-like enemy will start to appear. 
    White-like enemy will not grow more difficult.

- Additional Mode
  "OMAKE MODE" is the another rule that will be unlocked by satisfying some conditions.
  "OMAKE" meens "poor added bonus" in Japanese. So, these rules are so experimental.
  - O-GUI RULE
    This is "Bomb game" rule Using 3rd button [C].
    In this mode, OGUI rate gauge appears on the left-top side of the screen.
    When you EAT bullets, OGUI rate will increase. 
    And when the rate hits 100%, display "O-GUI OK !" on the screen.
    Then press the 3rd button to use OGUI bomb. 
    Using OGUI bomb, you EAT all of bullets on the screen.
    Replay data file saves as "hiscore_ogui.ply".
    - EAT Bonus rules
      min;10[points], max;120[points]
      Initial EAT Bonus; 10[points]
      EAT bullets continously within 0.5[sec.]; +20[points]
      Failing to EAT bullets continously within 0.5[sec.]; -10[points]      
  - KUIDAORE RULE
    This is "3 colors IKARUGA" rule Using 3rd button [C].
    I wonder that "Is this mode Shotem up game ?".
    You change my ship's color by pressing button, [Z]red, [X]green, and [C]blue.
    Same color bullet is EATen with no time. 
    And when you EAT same color bullets, ship shoot in 0.4[sec.].
    Replay data file saves as "hiscore_kuid.ply".
    - EAT Bonus rules
      min;10[points], max;100[points]
      Initial EAT Bonus; 10[points]
      EAT bullets continously within 0.5[sec.]; +10[points]
      Failing to EAT bullets continously within 0.5[sec.]; Initialize to 10[points]
    - Difficulty
      The increasing rate is 0.018[levels / bullet] by EATing.
  



