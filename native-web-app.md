To create native web app for any url
just install nativefier
 run
 ```
 nativefier -p linux -a x64 https://web.whatsapp.com
 ```
 
 Then create a desktop entry 
 ```
sudo -H gedit /usr/share/applications/whatsapp-webapp.desktop
 ```
 
 ```
[Desktop Entry]
Comment=Whatsapp created with nativefier
Terminal=false
Name=Whatsapp
Exec=/home/vidu/whatsapp/WhatsAppWeb
Type=Application
Icon=/home/vidu/icons/whatsapp.png
Categories=Network;

 ```
