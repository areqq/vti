VU+ VTI tools

```
opkg list_installed | grep kernel-module  | egrep -v  "(ext2|ipv6|tun)" | awk '{print "opkg remove "$1}' | sh
opkg list_installed | grep enigma2-locale- | egrep -v "(-pl|-en)"  | awk '{print "opkg remove "$1}' | sh
opkg list_installed | grep hbbtv | awk '{print "opkg remove "$1}'  | sh
opkg remove enigma2-plugin-extensions-cutlisteditor enigma2-plugin-extensions-dvdplayer enigma2-plugin-extensions-graphmultiepg enigma2-plugin-extensions-mediaplayer enigma2-plugin-extensions-mediascanner enigma2-plugin-extensions-moviecut enigma2-plugin-extensions-mo
vieretitle enigma2-plugin-extensions-piconmanager enigma2-plugin-extensions-pictureplayer enigma2-plugin-extensions-remotechannelstreamconverter enigma2-plugin-extensions-tageditor enigma2-plugin-systemplugins-blindscan enigma2-plugin-systemplugins-cablescan enigma2-plu
gin-systemplugins-fastscan enigma2-plugin-systemplugins-networkbrowser  enigma2-plugin-systemplugins-remotecontrolcode enigma2-plugin-systemplugins-ui3dsetup enigma2-plugin-systemplugins-uipositionsetup enigma2-plugin-extensions-piconmanager enigma2-plugin-extensions-streamtv enigma2-plugin-systemplugins-commoninterfaceassignment enigma2-plugin-systemplugins-satfinder enigma2-plugin-systemplugins-toolkit enigma2-plugin-systemplugins-ui3dsetup �enigma2-pl
ugin-systemplugins-zappingmodeselection enigma2-plugin-extensions-epgsearch

opkg remove wpa-supplicant wpa-supplicant-cli wpa-supplicant-passphrase  enigma2-plugin-systemplugins-wirelesslan  --force-depends

```
