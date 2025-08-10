Creates a macro to use the auto z-offset button on the Kobra 2 Neo running klipper.

Installation:
1. Add the AutoOffset.cfg to your klipper files
2. In "printer.cfg" add the following:


When trying to use this script in my start_print macro,  the m400 command (wait for current movement to finish) will skip the whole leveling loop.

I would recommend using the Z_Offset macro and saving the adjustment before you print.


*printer.cfg*:
   
    [include AutoOffset.cfg]

    
   
    [gcode_button zbutton]
   
    pin: ^PA0
  
    press_gcode:
      
      RESPOND MSG="Z offset button PRESSED"  ; Optional, Comment out if you don't like it/
    
