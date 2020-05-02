# whatsapp-webapp-linux
Just a simple method to run whatsapp webapp on linux *Securely*

This is a simple method that can be applied to any application actually 
But I have written it for whatsapp Specfically

It's a simple 2 step process
first run
```
sudo -H gedit /usr/share/applications/whatsapp-webapp.desktop
```

Then copy the text below and save.



```
#!/usr/bin/env xdg-open
[Desktop Entry]
Name=WhatsApp
GenericName=WhatsApp
Comment=WhatsApp desktop webapp
#Exec=webapp-container --store-session-cookies --webappUrlPatterns=https?://*.whatsapp.com/* --user-agent-string='Mozilla/5.0 (Windows NT 6.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/41.0.2228.0 Safari/537.36' https://web.whatsapp.com %u
Exec=/opt/google/chrome/google-chrome --app=https://web.whatsapp.com/
Terminal=false
Type=Application
StartupNotify=true
MimeType=text/plain;
# If you want icon, type path of icon
# Icon=
Categories=Network;Application;
Keywords=WhatsApp;webapp;
X-Ubuntu-Gettext-Domain=WhatsApp
StartupWMClass=web.whatsapp.com
```

And that's It we are done
### To add icon
To add a whatsapp Icon to the application just enter the path to the icon.

