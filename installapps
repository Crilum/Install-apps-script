#Color Variables

NC='\e[0m'
BLACK='\e[0;30m'
RED='\e[0;31m'
GREEN='\e[0;32m'
WHITE='\e[1;37m'
ORANGE='\e[0;33m'
BLUE='\e[0;34m'
PURPLE='\e[0;35m'
CYAN='\e[0;36m'
YELLOW='\e[1;33m'
DARGRAY='\e[1;30m'

#Lighter Colors
LIGRAY='\e[0;37m'
LIGREEN='\e[1;32m'
LIRED='\e[1;31m'
LIBLUE='\e[1;34m'
LIPURPLE='\e[1;35m'
LICYAN='\e[1;36m'


#Background Color Variables

#Color Variables
BACKBLACK='\e[0;40m'
BACKRED='\e[0;41m'
BACKGREEN='\e[0;42m'
BACKWHITE='\e[1;47m'
BACKORANGE='\e[0;43m'
BACKBLUE='\e[0;44m'
BACKPURPLE='\e[0;45m'
BACKCYAN='\e[0;46m'
BACKYELLOW='\e[1;43m'

#Lighter Colors
BACKLIGRAY='\e[0;47m'
BACKLIGREEN='\e[1;42m'
BACKLIRED='\e[1;41m'
BACKLIBLUE='\e[1;44m'
BACKLIPURPLE='\e[1;45m'
BACKLICYAN='\e[1;46m'

#Markup Variables
UNDERLINE='\e[4m'
BOLD='\e[1m'
BLINK='\e[5m'
REVVID='\e[7m'

#Install Script

echo -e "${CYAN}${BOLD}\nWelcome to Crilum's Install Script for new Raspberry Pi OS installs!\n${NC}"

read -r -p "Install apt and Crilum's favorite apps on apt? [Y/n] " input
case $input in
       [Yy][Ee][Ss]|[Yy])
       sudo apt install snapd exfat-fuse exfat-utils ardour code matchbox-keyboard gparted gnome-disk-utility rhythmbox kazam ffmulticonverter flatpak cowsay picard gnome-music gnome-sound-recorder unoconv ffmpeg gnome-boxes glxgears libreoffice inkscape imagemagick qemu gimp fuse f2fs-tools epson-printer-utility epson-inkjet-printer-escpr2 epson-backend deepin-screen-recorder cups cmatrix blender appmenu-gtk2-module appmenu-gtk3-module appmenu-gtk-module-common nginx anydesk

       ;;
[nN][oO]|[nN])
 echo -e "${RED}No${NC}"
       ;;
    *)
 echo -e "${RED}${BLINK}Invalid input...${NC}"
 invalid2="i"

esac

if [ "$invalid2" == "i" ]; then
 echo -e "${RED}\nError: Invalid input!${NC}"
 exit

 else
read -r -p "Install snapd and Crilum's favorite snaps? [Y/n] " input
case $input in
       [Yy][Ee][Ss]|[Yy])
       sudo snap install youtube-dl 

       ;;
[nN][oO]|[nN])
 echo -e "${RED}No${NC}"
       ;;
    *)
 echo -e "${RED}${BLINK}Invalid input...${NC}"
 invalid3="i"
 
esac

if [ "$invalid3" == "i" ]; then
 echo -e "${RED}\nError: Invalid input!${NC}"
 exit
else

read -r -p "Do you want to install Pi-Apps and Crilum's favorite Pi Apps? [Y/n] " input
case $input in
       [yY][eE][sS]|[yY])
       cd /home/pi
       wget -qO- https://raw.githubusercontent.com/Botspot/pi-apps/master/install | bash
       wget -q https://raw.githubusercontent.com/Itai-Nelken/PiApps-terminal_bash-edition/main/pi-apps-terminal-bash-edition.sh -O $HOME/pi-apps/pi-apps-terminal-bash-edition.sh 
pi-apps multi-install AndroidBuddy AnyDesk Autostar BalenaEtcher "Bongo Cam" Box64 Box86 Wine (x64) "Chromium Widevine" CloudBuddy "Color Emoji font" "Conky Rings" "Cool Retro Term" Discord Drawing eDEX-UI "Https File Server" "Lego Digital Designer" Node.js "Pi-Apps Terminal Plugin (python)" "Pi Power Tools" QEMU Scrcpy Snapdrop "Snap Store" SpeedTest-CLI "Sublime Text" Sysmon Timeshift Turbowarp Vivaldi "Web Apps" "Windows Flasher" "Windows Screensavers" "Wine (x86)" Zoom "TeamViewer Host" "Firefox Rapid Release"
       ;;
      [nN][oO]|[nN])
 echo -e "${RED}No${NC}"
       ;;
    *)
 echo -e "${RED}${BLINK}Invalid input...${NC}"
 invalid="i"
esac
if [ "$invalid" == "i" ]; then
   echo -e "${RED}\nError: Invalid input!${NC}"
   else
   echo -e "${GREEN}\nDone!${NC}"
fi
fi
fi
