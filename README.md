# Pre-Install-Arch-Packages
sudo pacman -Syu
sudo pacman -S tilix
sudo pacman -S flatpak

yay -S visual-studio-code-bin
yay -S figma-linux-bin
yay -S dbeaver
yay -S discord

sudo pacman -S nodejs npm

Canara
sudo pacman -S gphoto2 v4l2loopback-utils ffmpeg
sudo modprobe v4l2loopback exclusive_caps=1 max_buffer=2
gphoto2 --auto-detect
#iniciar la camara
gphoto2 --stdout --capture-moviie | ffmpeg -l - -vcodec rawvideo -pix_fmt yuv420p -threads 0 -f v4l2 /dev/video0


flatpak install flathub org.onlyoffice.desktopeditors

sudo pacman -S postgresql
sudo systemctl start postgresql
sudo systemctl enable postgresql



yay -S kdeconnect
yay -S arduino
yay -S simplenote-electron-bin


sudo pacman -S mongodb

https://flathub.org/apps/de.uni_heidelberg.zah.GaiaSky
