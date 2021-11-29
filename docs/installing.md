## Introduction

After [downloading a version of Floflis](https://floflis.github.io/cli/download/), read this page for official instructions on installing.

## Before installing

**Note**: You can [skip](#installing) this step if your device have enough storage space available. If the target device is limited (like a WiFi router), this pre-install step will be needed; but if you'd already downloaded the Lite version, you can skip into the [next step](#installing).

If you wish to remove the updates module (which includes .git folder), please copy the `Floflis DNA` folder, so you will have a copy which you can update (`git pull`).

Inside the clonned/downloaded extracted folder, open Terminal and type the following:

```bash
sudo chmod 755 init.sh && sudo ./init.sh
```

Respond to questions and the script will configure the installer for you.
After done, you can move the `Floflis DNA` folder to your device.
Done, you made your own build of **Floflis DNA Lite** version.

## Installing

Assuming `Floflis DNA` folder is on the target device, run the following command inside its folder:

```bash
sudo chmod 755 install.sh && sudo ./install.sh
```

Insert your password, and Floflis will be installed.

### Specific OS

#### Linux

The installation is simple on Linux, following the [above instructions](#before-installing).
Make sure you have BASH or any other compatible environment.

#### MacOS

Instructions for MacOS are yet a draft. Please stay tuned in our [blog](https://floflis.github.io/blog/) for news.

Like on Linux, make sure you have BASH or any other compatible environment.

#### Windows

Instructions for Windows are yet a draft. Please stay tuned in our [blog](https://floflis.github.io/blog/) for news.

Install [Cygwin](https://www.cygwin.com/), make sure you have BASH or any other compatible environment.

If you use Windows 10, there is no need to install Cygwin, you can install Ubuntu/BASH/Windows subsystem for Linux on it from Windows Store.

#### Android

Instructions soon, with a focus on Termux.

Please stay tuned in our [blog](https://floflis.github.io/blog/).

### Specific devices

#### x86 (usual laptops/desktops)

We are already working to provide Floflis OS and UniOS for this platform.

You can install Floflis as a program, with instructions [here](#specific-os).

Please stay tuned in our [blog](https://floflis.github.io/blog/) for news.

#### Raspberry Pi

<<<<<<< HEAD
See [here](https://learn.adafruit.com/adafruit-raspberry-pi-lesson-1-preparing-and-sd-card-for-your-raspberry-pi/balena-etcher/) how to install Linux on your Raspberry Pi device. Then, you can install Floflis DNA using [above instructions](#before-installing).
**Standalone distro is being worked**, and will be released soon; so you will flash Floflis directly.

#### RISC-V boards

See [here](https://wiki.ubuntu.com/RISC-V) how to install Linux on your RISC-V device. Then, you can install Floflis DNA using [above instructions](#before-installing).
**Standalone distro is being worked**, and will be released soon; so you will flash Floflis directly.
=======
See [here](https://www.howtoforge.com/tutorial/howto-install-raspbian-on-raspberry-pi/) how to install Linux on your Raspberry Pi device. Then, you can install Floflis DNA using [above instructions](#before-installing). Standalone distro soon.
>>>>>>> 00eaafe8877adeef389e7acd16a565c6bb54398b

#### WiFi Routers

See [here](https://www.instructables.com/id/How-To-Install-Linux-DD-WRT-Firmware-On-Your-Route/) how to install Linux on your WiFi router. Then, you can install Floflis DNA using [above instructions](#before-installing).

#### Purism Librem phones/devices

Instructions soon.

Please stay tuned in our [blog](https://floflis.github.io/blog/).

<<<<<<< HEAD
#### Pinephone/other Pine64 devices
=======
#### KaiOS phones and other devices

Instructions soon.

Please stay tuned in our [blog](https://floflis.github.io/blog/).

#### RISC-V boards
>>>>>>> 00eaafe8877adeef389e7acd16a565c6bb54398b

Instructions soon.

Please stay tuned in our [blog](https://floflis.github.io/blog/).

#### PlayStation 2

See [here](http://kernelloader.sourceforge.net/linux.html) how to install Linux on your PS2. Then, you can install Floflis DNA using [above instructions](#before-installing).

<<<<<<< HEAD
Please note the ideal version for PS2 (Floflis Grass, graphical evolution of Floflis Soil), isn't yet available, but soon you will be able to upgrade Floflis DNA.
=======
Please note the ideal version for PS2 (Floflis Grass, graphical evolution of Floflis Soil), isn't yet available, but soon you will can upgrade Floflis DNA.
>>>>>>> 00eaafe8877adeef389e7acd16a565c6bb54398b

#### PlayStation 3

See [here](https://www.wikihow.com/Get-Linux-on-PlayStation-3) how to install Linux on your PS3. Then, you can install Floflis DNA using [above instructions](#before-installing).

<<<<<<< HEAD
Please note the ideal version for PS3 (Floflis Base, evolution of Floflis Grass), isn't yet available, but soon you will be able to upgrade Floflis DNA.
=======
Please note the ideal version for PS3 (Floflis Base, evolution of Floflis Grass), isn't yet available, but soon you will can upgrade Floflis DNA.
>>>>>>> 00eaafe8877adeef389e7acd16a565c6bb54398b

#### PlayStation 4

See [here](https://appuals.com/how-to-install-linux-and-run-steam-on-playstation-4/) how to install Linux on your PS4. Then, you can install Floflis DNA using [above instructions](#before-installing).

Please note the ideal version for PS4 (Floflis Home, evolution of Floflis Base), isn't yet available, but soon you will be able to upgrade Floflis DNA.

#### Xbox

See [here](https://xboxlinuxproject.fandom.com/wiki/How_To_Install_Linux) how to install Linux on your Xbox. Then, you can install Floflis DNA using [above instructions](#before-installing).

Please note the ideal version for Xbox (Floflis Grass, graphical evolution of Floflis Soil), isn't yet available, but soon you will be able to upgrade Floflis DNA.

#### Xbox 360

See [here](https://en.wikipedia.org/wiki/Free60) how to install Linux on your Xbox 360. Then, you can install Floflis DNA using [above instructions](#before-installing).

Please note the ideal version for Xbox 360 (Floflis Base, evolution of Floflis Grass), isn't yet available, but soon you will be able to upgrade Floflis DNA.

#### Xbox One

No developments yet to hack XB One.

#### Xbox Series X/S

No developments yet to hack XB Series.

#### Nintendo DS

See [here](http://www.dslinux.org/wiki/RunningDSLinux.html) how to install Linux on your Nintendo DS. Then, you can install Floflis DNA using [above instructions](#before-installing).

Soon, you will be able to upgrade Floflis DNA to Floflis Core.

#### Nintendo 3DS

See [here](https://gbatemp.net/threads/release-linux-for-the-3ds.407187/) how to install Linux on your Nintendo 3DS. Then, you can install Floflis DNA using [above instructions](#before-installing).

Soon, you will be able to upgrade Floflis DNA to Floflis Core.

Please note the ideal version for 3DS (Floflis Soil, evolution of Floflis Core), isn't yet available, but soon you will be able to upgrade Floflis DNA.

#### Nintendo Game Cube and Wii

See [here](http://www.gc-linux.org/wiki/Main_Page) how to install Linux on your Nintendo Game Cube and Wii. Then, you can install Floflis DNA using [above instructions](#before-installing).

<<<<<<< HEAD
Please note the ideal version for GC/Wii (Floflis Grass, graphical evolution of Floflis Soil), isn't yet available, but soon you will be able to upgrade Floflis DNA. For Nintendo Wii, Floflis Base (evolution of Floflis Grass) may be the ideal.
=======
Soon, you will can upgrade Floflis DNA to Floflis Core, and will be magic when you use `CJDNS/Yggdrasil` + `Dat protocol/IPFS` using your Nintendo Ethernet/WiFi connection!

Please note the ideal version for GC/Wii (Floflis Grass, graphical evolution of Floflis Core), isn't yet available, but soon you will can upgrade Floflis DNA. For Nintendo Wii, Floflis Base (evolution of Floflis Grass) may be the ideal.
>>>>>>> 00eaafe8877adeef389e7acd16a565c6bb54398b

##### Wii U

See [here](http://nintendotoday.com/forum/wii-u/13874-how-install-ubuntu-your-wii-u.html) how to install Linux on your Nintendo Wii U. Then, you can install Floflis DNA using [above instructions](#before-installing).

Please note the ideal version for WiiU (Floflis Base, evolution of Floflis Grass), isn't yet available, but soon you will be able to upgrade Floflis DNA.

#### Nintendo Switch

See [here](https://gbatemp.net/threads/l4t-ubuntu-a-fully-featured-linux-on-your-switch.537301/) how to install Linux on your Switch. Then, you can install Floflis DNA using [above instructions](#before-installing).

<<<<<<< HEAD
Please note the ideal version for Switch (Floflis Home, evolution of Floflis Base), isn't yet available, but soon you will be able to upgrade Floflis DNA to Core, Soil, Grass, Base and Home.
=======
Please note the ideal version for Switch (Floflis Home, graphical evolution of Floflis Base), isn't yet available, but soon you will can upgrade Floflis DNA to Core, Soil, Grass, Base and Home.
>>>>>>> 00eaafe8877adeef389e7acd16a565c6bb54398b

#### Notes

Soon, Floflis will provide its own instructions and standalone OS distros to run on these devices, and software installers for other OSes.

Please stay tuned in our [blog](https://floflis.github.io/blog/) for news.

## Updating

<<<<<<< HEAD
Visit the [Updating session](../updating).
=======
Update from P2P network (not available yet):

```bash
floflis update
```

Update from GitLab:

```bash
floflis update --gitlab
```

Update from GitHub:

```bash
floflis update --github
```
>>>>>>> 00eaafe8877adeef389e7acd16a565c6bb54398b
