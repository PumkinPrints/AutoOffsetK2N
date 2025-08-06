Creates a macro to use the auto z-offset button on the Kobra 2 Neo running klipper.

Installation:
1. Add the AutoOffset.cfg to your klipper files
2. In "printer.cfg" add the following:

   
*printer.cfg*:
   
    [include AutoOffset.cfg]

    
   
    [gcode_button zbutton]
   
    pin: ^PA0
  
    press_gcode:
      
      RESPOND MSG="Z offset button PRESSED"
    
