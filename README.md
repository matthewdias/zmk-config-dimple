# zmk-config-dimple

Keymap config for Dimple Blue Edition


## Instruction:
1. Fork this repo
2. Use https://nickcoutsos.github.io/keymap-editor/ as keymap-editor to edit the keymap you prefer (this is not a real-time keymap editor). Remember to give keymap-editor the permission to acess your fork of this repo.
3. Press 'Commit Changes' on keymap-editor page after you are done. Don't forget to set (1) 'BT_CLR' (2)sys_reset (3) bootloader to keys, cause you may have to use it when you have connection issue. 
4. Go to your own fork of this repo, check Actions page. There is a new workflow generating zmk firmware 'zmk.uf2', save it to your PC folder.
5. Press the reset button on the back of Dimple Blue Edition PCB twice to put it into bootloader mode. There will be a device popped out. Drag the zmk firmware you generated into the root folder.
6. The device will be refreshed and showed as 'dimple'. All done!

## Known Issues:
1. ~~Blue LED doesn't work.~~ Currently the blue led pin hasn't been defined in bootloader. So blue pin won't blink when usb is connected.
2. Battery Level showed in the system is not so accurate. But the difference should be in 5% deviation.(If update) 
3. Occasionally repeating key input. The cause has not been identified yet. Please press sys_reset when there is repeating keys and disconnection
4. There are some issues connecting to Mac OS devices, including Mac mini, Macbook and iMac. But it's totally fine connecting to iOS or ipadOS devices.
5. Delayed connection when startup (Might have something to do with the bluetooth hardware on PC)

It would be much appreciated that you can report issue after using Blue version Dimple.

## Credit:

ZMK is awesome!
Read the zmk doc here https://zmk.dev/

And thanks to @nickcoutsos for this amazing keymap editor
https://github.com/nickcoutsos/keymap-editor
