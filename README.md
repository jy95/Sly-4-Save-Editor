Save file editor for Sly Cooper Thieves In Time.
For use with RPCS3.

Main purpose is to skip sections of the game with motion controls.

------------

Sly Cooper: Thieves In Time; Sixaxis Save Skip


Description: Sly Cooper Thieves In Time requires a proper DualShock peripheral in order to be completed. Sadly for those of us who have other kinds of controllers which do not feature Sixaxis, it means we're stranded, unable to pass certain missions. Well, worry not, I went ahead and figured out ways to edit the save file, and guess what, I succeeded!

___________________________________________________

Now, before we move on, here's a bit of backstory:
___________________________________________________


``You see, Sony had the great idea to add motion sensors to their DualShock 3 controller, and in hindsight, it was really neat. It added such a cool, new way to interact with your games and control them in ways that seemed like science fiction. I mean, the Wii went all out on motion controls, and I don't need to mention it was one of the most successful console in history, second to the PS2 of course.

However, if you've ever needed to get more controllers, say for local multiplayer, then you may be familiar with third-party controllers. When it came to them for PS3, it was like russian roulette. You see, alot of them didn't have Sixaxis, and being that alot of games required that feature, it was essential. Sadly, we weren't spared by the counterfeiters, and tons of very accurate DualShock 3 clones were being sold online, fooling customers into thinking they had a real one, only to find out it cannot detect motions.

Welp, that wasn't just an issue with the retail console, as playing those games is also an issue on the RPCS3 emulator. Why, well, because at the time I'm writing this, it does not feature a Sixaxis emulation nor any kind of support for UDP clients (which allows to use peripherals such as Wiimotes, Joycons and even smartphones as gyroscopic devices through Wi-Fi), and even worse, DualShock 3 controllers cannot be used for that matter because the drivers don't support that feature on PC (thanks Sony). So, if you want to play games that require motion controls on RPCS3, you would need a DualShock 4 instead.``

__________________________________________________________________

Now that that's out of the way, here's something to Keep in mind:
__________________________________________________________________


Some sections of the game feature the use of Sixaxis, but won't need it to pass them; 

For example, in "Turning Japanese/Something's Fishy", there is a section where you need to fish out, well, fishes, and you control the fishing rod with motion controls. However, it seems the fishes eventually come close enough to be pulled out without having to move the rod. You might fail for failing to pull them all out in time, but it shouldn't take more than 5 retries to pass through, hopefully.

Another example is in "Forthy Thieves/All Rolled Up!", during the rhythm game, after a section is done it says to shake the controller. Failing to do so takes out a bit of health. However, it seems like it doesn't prevent you from succeeding.

_________________________________________________________________

Here are the parts that require motion controls to be completed:
_________________________________________________________________


In "Turning Japanese/Pretty In Pinker", there is a Bentley hacking section that requires you to tilt the controller to move the orb.

In "Clan of the Cave Raccoon/Getting Stronger", there is a minigame that requires you to tilt the controller to keep an egg balanced, otherwise it will fall and you will fail. At the end of the mission, all of the minigames are shuffled, and the egg minigame is present again.

In "Clan of the Cave Raccoon/Operation: Jurassic Thievery", there is that same Bentley hacking section that requires you to tilt the controller to move the orb.

___________________________

(Semi) Automatic Solution:
___________________________


1- Download the following tool: https://github.com/ZeptoBST/Sly-4-Save-Editor/releases/tag/Releases

2- Extract the .zip file (obviously)

3- Play until you reach a part that needs motion controls to progress. 

4- Save your game, just to make sure. It also wouldn't hurt to create a new save file, in case something were to go wrong.

5- Locate your save file. Go into the "Manage" tab and click "Save Data". Look for the Sly 4 save you made. (should be the latest, thus look at the "Last modified" row to find it)

6- Right-click on it and click "Open Save Directory" and copy the path of said directory; ex: C:\Programs\RPCS3\dev_hdd0\home\00000001\savedata\BCUS98247_SAVE_SLOT_000xx

7- Run the program (duH)

8- Paste the directory of your save file in the box on the top.

9- Press the appropriate Skip button, depending of which mission you're on.

10- Load your save file and you should be done.



___________________

Manual Solution:
___________________


1- Play until you reach a part that needs motion controls to progress. 

2- Save your game, just to make sure. It also wouldn't hurt to create a new save file, in case something were to go wrong.

3- Locate your save file. Go into the "Manage" tab and click "Save Data". Look for the Sly 4 save you made. (should be the latest, thus look at the "Last modified" row to find it)

4- Right-click on it and click "Open Save Directory".

5- Open "SYS_DATA" in a hex editor (preferably HxD)

6- I'll assume you're familiar with hex editing. If not, go watch a tutorial. If you know how it works, you can continue.

7- Here are the values for each parts:
(replace the values in the save file with the ones below)
__________________________________________________________


TJ/Pretty In Pinker:

Offsets 30,31,32,33 = "FE 37 0B 12"


COTCR/Getting Stronger:

Offsets 2C,2D,2E,2F,30,31,32,33 = "00 00 00 00 00 00 00 00"
Offsets 1E3,1E4 = "02 01"
Offsets 1AE = "03"


COTCR/Operation: Jurassic Thievery:

Offsets 30,31,32,33 = "07 9A AD F2"


OMAM/Short Supply:

Offsets 30,31,32,33 = "58 B3 8C 8C"


FT/Rug Rats:

Offsets 30,31,32,33 = "3F 07 B0 10"


FT/All Rolled Up!:

Offsets 30,31,32,33 = "9C 29 40 62"

__________________________________________________________

8- Obviously, save the file.

9- Load your save file and you should be done.


You should now be able to play Sly Cooper 4 on RPCS3, regardless of the type of controller you have.
