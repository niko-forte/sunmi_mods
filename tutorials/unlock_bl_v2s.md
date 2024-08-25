How to unlock the bootloader on the Sunmi V2s

## FOLLOW THE STEPS CORRECTLY IF YOU DON'T WANT TO BRICK YOUR DEVICE!!!

Enable the developer options, open settings, scroll down to the device information section and enter
look for the build number option and click 7 times in a row, then return to the settings screen and now go to system, enter
click on advanced and enter developer options, enable OEM unlocking and USB debugging
Now connect the USB cable to the computer and the PC (make sure you have the drivers installed)
Open the cmd win+r cmd.exe, type adb devices and make sure that your device appears
if everything is ok write in the cmd adb reboot bootloader (the device will reboot)
and it will start in fastboot mode In the same cmd window type fastboot devices (to check that it is connected)
ATTENTION TO THE NEXT STEP, THE NEXT COMMAND WILL DELETE EVERYTHING, COPY YOUR IMPORTANT FILES
Type in cmd fastboot flashing unlock and follow the instructions on the device screen And that's it
your bootloader will now be unlocked.
