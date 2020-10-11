# Arena-Macros
Just a list of macros and scripts for a silly game within a game



ONE-
Script to keep yourself set as party1 (necessary for modifier macros!!!) - Make sure to have leads before queueing:
Place everything in quotations into a non character specific macro

"/run LoadAddOn("Blizzard_CompactRaidFrames") CRFSort_Group=function(t1, t2) if UnitIsUnit(t1,"player") then return false elseif UnitIsUnit(t2,"player") then return true else return t1 < t2 end end CompactRaidFrameContainer.flowSortFunc=CRFSort_Group"



TWO-
Focus target modifier macro-Replace "spell_name_here" with desired ability to macro. When macro is used it will cast the chosen ability on your target unless you use your modifier, in this case shift, in combination with the button the macro is keybound to (example: shift+r)


"#showtooltip 
/cast spell_name_here [nomod,exists,target=target] 
/cast spell_name_here [@focus,modifier:shift]"

THREE-
Teammate modifier macro- replace "spell_name_here" with desired ability. It will cast macro'd ability on yourself if no modifier button is used, if alt modifier is used + macro keybind it will target party2, and if shift is used it will target party1, NOT SELF. (Example "r","ALT+r","SHIFT+R"

"#showtooltip
/cast spell_name_here [@player,nomod,exists]
/cast spell_name_here [modifier:alt,target=party2] 
/cast spell_name_here [modifier:shift,target=party1]"

FOUR- 
Enemy Target modifier macro- follows the same principle as teammate modifier macro, except for arena enemies

"#showtooltip
/cast spell_name_here [target=arena1]
/cast spell_name_here [modifier:alt,target=arena2] 
/cast spell_name_here [modifier:shift,target=arena3]"


FIVE-
Stopcast macro- Simple macro to generate jukes on enemy interrupts. I highly suggest using a stopcast macro

"/stopcasting"

Tip you can also macro all of your cast time abilities to have a stopcast macro on them so that if you press them twice it will stopcast, this does take some getting used to, however. Example:

"#showtooltip Holy Light
/cast Holy Light
/stopcasting"


SIX
Global Cooldown Macro/Nuke Macro another simple macro for placing multiple buttons into one, I'm going to use divine favor+medallion+holy light as an example

"#showtooltip Divine Favor
/cast Divine Favor
/use Gladiator's Medallion
/cast Holy Light"





Please make sure none of your modifier macros share binds with anything else, as this will sandbag your improved setup. Visit me @ twitch.tv/remyplayer1 for more help, to play, or just hang out=)





