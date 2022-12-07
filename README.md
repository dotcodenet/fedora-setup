# Linux Fedora Workstation setup

1. Make DNF faster

```bash
fastestmirror=True
max_parallel_downloads=10
defaultyes=True
```

2. Clean packages

```bash
sudo dnf autoremove
sudo dnf clean all
```

3. System update

```bash
sudo dnf upgrade
```

4. Install basic terminal tools

```bash
sudo dnf install neofetch inxi htop
```

5. Download and install [Flathub - flatpak](https://flathub.org/repo/flathub.flatpakrepo)

6. Install Gnome Tweaks

```bash
sudo dnf install gnome-tweaks
```

7. Install Gnome Extension Manager

```bash
flatpak install flathub com.mattjakeman.ExtensionManager
```

8. Install Flatpak Manager (FlatSeal)

```bash
flatpak install flathub com.github.tchx84.Flatseal
```
9. PortProton (for installing windows games)

```bash
wget -c "https://github.com/Castro-Fidel/PortWINE/raw/master/portwine_install_script/PortProton_1.0" && sh PortProton_1.0 -rus
```