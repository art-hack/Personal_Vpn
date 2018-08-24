# Setup Your own Vpn

## Steps
* Signup for Github Education with your College/Organisation ID.
* You will get a $50 code for Digital Ocean, signup and use it. It will let you host a Server for 10 months.
* Now after signup, Click on droplet and create a Droplet(VPS) with the least config and make sure to select Ubuntu.
* Open your Droplet using the Access > Launch Console option.
* Now Login using the root password sent on your mail and save a new password as required.
* Run the installation using the command given below and remember to use TCP, Port: 443 settings as UDP might be blocked by your organisation.
* Now register a user and a .ovpn file will be generated.
* Now in Filezila(install if not already present), Press Ctrl+S and add a new site with the following settings
  * Protocol SFTP
  * Host is the IP visible on your Droplet.
  * Port (Leave Blank)
  * Logon Type : Normal
  * User and Password: root and whatever ubuntu password you might have set up.
* Download the .ovpn file generated from there(will be visible in the right window).
* Now download OpenVpn from (https://openvpn.net/index.php/open-source/downloads.html) and install it.
* Now an OpenVpn icon will be visible in your taskbar, so Right-Click > Import File and import the file that you just downloaded with filezilla.
* Finally again right click on the OpenVpn icon and click connect under the user that u created.
* Voila!, its done, Enjoy your Vpn.

### Installation
Run the script and follow the assistant:

`wget https://git.io/vpn -O openvpn-install.sh && bash openvpn-install.sh`

Once it ends, you can run it again to add more users, remove some of them or even completely uninstall OpenVPN.
