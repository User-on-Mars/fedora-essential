# fedora-essential
some essential things to download in fedora linux

1️⃣ Enable RPM Fusion for More Software

sudo dnf install \
https://download1.rpmfusion.org/free/fedora/rpmfusion-free-release-$(rpm -E %fedora).noarch.rpm \
https://download1.rpmfusion.org/nonfree/fedora/rpmfusion-nonfree-release-$(rpm -E %fedora).noarch.rpm

2️⃣ Install NVIDIA Drivers (For Best Performance)

sudo dnf install akmod-nvidia xorg-x11-drv-nvidia-cuda

3️⃣ Install KDE Essentials & Fix Battery Life

sudo dnf install tlp auto-cpufreq kde-connect
sudo systemctl enable --now tlp
sudo systemctl enable --now auto-cpufreq

4️⃣ Set Up OpenRGB for Dell Alienware RGB

sudo dnf install openrgb

5️⃣ Install Flatpak for More Apps

sudo dnf install flatpak
flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
