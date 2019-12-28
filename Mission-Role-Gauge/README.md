# Custom-Wingmen-Gauge
Script files for wookieejedi's custom wingmen gauge for Freespace 2 Open. 

See main topic here:
https://www.hard-light.net/forums/index.php?topic=95180.0

Background: 
This script creates a new wingmen HUD gauge that provides three large differences compared to the default Wingmen HUD Gauge.


Major Features:

1) Gauge writes the full wingnames. The script updates the width of the gauge so that you will always see the fill wing name. It will not show characters after a "#", too.

2) Gauge can use two different styles, the traditional wingmean gauge layout, or a compact grid layout. To change to grid layout simply set CustomWingGauge.style = "grid".

3) Gauge shows a color for each wingman's relative health. The color transitions from green to orange to red. If the wingman is dead then a hollow red circle is shown. If the wingman departed then a hollow circle with a line is shown with the color of the departed wingman's health. If you would prefer to use gray-scale dots instead of green-orange-red dots then open the file and simply change CustomWingGauge.isgrayscaled = false to CustomWingGauge.isgrayscaled = true.

4) Different icons are used to differentiate between bombers and other ships. Bombers are shown as square icons and other ships are shown as circles. This feature can be turned off by setting CustomWingGauge.isbombdifferent = false

5) You can specify the type of font the gauge uses from fonts.tbl. To specify a different font then the default change the values of CustomWingGauge.fonts = {default=1, low_resolution=3} to desired the font name or index.

6) You can specify the position of the gauge easily. To change position of the gauge set values of origin and offset, similar to hud_gaugles.tbl. For example, CustomWingGauge.origin = {x=0.85, y=0.2} and CustomWingGauge.offset = {x=0, y=0}. If you want to use RTT to a cockpit display you can also set CustomWingGauge.RTT = {use=true, gauge_name="Wingmen_Custom_RTT}. If using the RTT feature, the script will use RTT in internal view then switch to screen render for external view. Also, for RTT to work be sure to also make a '+Scripted Gauge:' entry in hud_gauges.tbl, and the 'gauge_name' should equal the 'Name' of the '+Scripted Gauge' in the 'hud_gauges.tbl'.

Installation:
Download and copy the "cuswingmengag-sct.tbm" file into your data/tables folder. If you know a bit of basic scripting you can also set this to appear on a mission by mission basis.
To change the color of the gauges text and outline simply change the HUD color for the wingmen gauge in the HUD configuration settings.

Last Items:
Here is a screenshot showing it in action.
Script file is attached. I would be happy to hear any feedback, suggestions, or overall thoughts.

Thanks!
