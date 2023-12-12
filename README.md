# ZMK firmware

This is my [ZMK](https://zmk.dev/docs) firmware
 for the Ferris Bling LP.

![](https://keonigarner.com/assets/images/keymap.png)

It contains keymap definition files for the following boards in [./config](./config):

 - Cradio (Also used for the Ferris LP Bling, my main board) with 3x5+2 keys

Pushing changes will build all the keyboards. You need to be signed in to a GitHub account to push changes and build the firmware. To not waste build time, comment out the keyboards in [./build.yaml](./build.yaml) that you do not have.

To build the firmware:

- Fork this repo on GitHub
- Clone your fork locally
- Trigger a build:
  - Make a trivial change to ./build.yaml (or any non *.md file)
  - Push that change
- Look in the [Actions](https://github.com/ObiWanKeoni/zmk-config/actions) tab
     for the build triggered by that change.
- Wait for the build to finish
- Click on the build link next to the green checkbox
- Download the artifact file with the firmware
- See [Installing The Firmware](https://zmk.dev/docs/user-setup#installing-the-firmware)
  for more details from there.

*Once* your board works with the default firmware,
  you can modify the keymap.

If you want to enable features,
  modify the appropriate `.conf` file.

Ripped off from @urob 's [ZMK Config](https://github.com/urob/zmk-config/)
