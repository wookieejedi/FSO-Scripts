# Custom-Movements-SEXPs
Custom sexps and functions for FSO that allow for much easier ship movements and rotations.

See main topic here:
https://www.hard-light.net/forums/index.php?topic=96082.0


TLDR: Release of custom sexps which can make cap ship (or any ship) movements much easier and more natural looking. 

[img]https://cdn.discordapp.com/attachments/223511363807346691/650508690113167426/unknown.png[/img]


Background
Do you ever get frustrated when trying and get large ship movements to look good? I've found this be especially tricky if you want the ships to act dynamically, if you want big ships to rotate in a way that looks natural, or if you want many big ships to follow a leader ship and stay in a relative formation. Dynamic waypoints provide an invaluable tool, yet ships will stop following a waypoint path once the path is complete or immediately turn around to start the path again. I wanted a single sexp that told a ship to track a waypoint or ship, thus the ship would travel to the waypoint and then move again if the waypoint moved. 

It can be similarly tricky to get large ships to rotate to a certain orientation. The rotation maneuver sexp is useful but you aren't guaranteed that the ship will stop rotating when it reaches the desired orientation. Again, I wanted a single sexp that I could use once that would move a ship to a specified orientation with a natural looking movement. 

Also, recent updates have focused on making scripted movements look natural and precise. For example, values in the sexp can be set to have ships precisely stop on waypoints, then use the natural AI methods to rotate. There’s also the addition of a 'semi-smart' waypoint order, where AI ships following waypoints will check for obstacles in their path, then stop if they are on course to hit something. Once the obstacle leaves then the path will resume. 

To achieve these goals, I developed a suite of custom lua sexps, and hopefully you might find something useful to your own missions! 


Usage:
Download these two tbm files listed within in this Github Folder (click the link to open the file on the web, then right click the `Raw` button and click `Save As`). Once downloaded, place them in your data/tables folder. Then just open FRED and you will see a new listing called LUA-Movements where all the sexps are located. There are detailed descriptions of each sexp and each argument. 

Important! You need an FSO build of August 24, 2022 or newer for these to work.

I included an example mission that shows how to use the 'move-to-orientation' and the 'add-ai-goal-track-ship' which is a higher order sexp that runs 'add-waypoint-track-ship' with 'add-ai-goal-track-waypoint' and 'set-idle-track-orientation'.

