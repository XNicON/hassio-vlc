# MINIMAL Add-on VLC run as deamon

Run a VLC player on Home Assistant Supervisord.

Control it using the web interface or with the new [VLC Telnet component](https://www.home-assistant.io/components/vlc-telnet/) and control the player from your HA Automations!

Place your media files on the /media folder in your hass.io or play files from network locations, Internet included! Try for example online radio

## Installation
1. Follow the steps on [this tutorial](https://www.home-assistant.io/hassio/installing_third_party_addons/) to add this repository to your hassio installation.
2. Refresh the add-ons using the white arrow on the top right of the page
3. Search for "VLC" on the list and click on it
4. Click on the install button and wait! It could take a couple of minutes.
5. Configure a password for your telnet and web interface
6. **Configure your audio output device.** (Bluetooth Specker, analog audio output)
7. Click on start
8. Add new integration [VLC Telnet component](https://www.home-assistant.io/components/vlc-telnet/), configuring 127.0.0.1 (localhost) as the host, 4212 as the port and the configured password.
