# World of Warships - Taken The Lead Remover
Replaces the World of Warships domination voice line (e.g. "Enemy has taken the lead") with silence.
As well removes the "On Fire" voiceline.


## Just a few notes for future automation implementations
```
wowsunpack.exe --list --extract bin\3173843\idx -p ..\..\..\res_packages --include "banks/Languages/EN/*.*" --output _unpack
sed /<Name>\w+Domination\w+\.wem<\/Name>/<Name>Silence.wem</Name>
sed /<Name>En_Speech_Alarms_Fire_Alarm.wem<\/Name>/<Name>Silence.wem</Name>
```
