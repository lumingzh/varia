<p align="center"><img src="https://raw.githubusercontent.com/giantpinkrobots/varia/main/data/icons/hicolor/scalable/apps/io.github.giantpinkrobots.varia.svg" width=200 /></p>
<h1 align="center">Varia</h1>
<h3 align="center">Download manager based on aria2</h3>
<br>

<p align="center">
  
![](https://img.shields.io/github/commits-since/giantpinkrobots/varia/latest/main?label=commits%20since%20latest%20release)  ![](https://img.shields.io/github/forks/giantpinkrobots/varia.svg)  ![](https://img.shields.io/github/stars/giantpinkrobots/varia.svg)  ![](https://img.shields.io/github/watchers/giantpinkrobots/varia.svg)  ![](https://img.shields.io/github/issues/giantpinkrobots/varia.svg)  ![](https://img.shields.io/github/issues-closed/giantpinkrobots/varia.svg)  ![](https://img.shields.io/github/issues-pr/giantpinkrobots/varia.svg)  ![](https://img.shields.io/github/issues-pr-closed/giantpinkrobots/varia.svg)  ![](https://img.shields.io/github/license/giantpinkrobots/varia.svg)  ![](https://img.shields.io/github/followers/giantpinkrobots.svg?style=social&label=Follow&maxAge=2592000)

</p>

<p align="center"><a href="https://flathub.org/apps/io.github.giantpinkrobots.varia"><img src="https://dl.flathub.org/assets/badges/flathub-badge-i-en.svg" width=300 /></a></p>

Varia is a simple download manager that conforms to the latest Libadwaita design guidelines, integrating nicely with GNOME. It uses the amazing aria2 to handle the downloads.

<p float="left" align="middle">
  <img src="https://raw.githubusercontent.com/giantpinkrobots/varia/main/screenshots/Screenshot-Varia-1.png" width=500 />
  <img src="https://raw.githubusercontent.com/giantpinkrobots/varia/main/screenshots/Screenshot-Varia-2.png" width=500 />
</p>

Varia supports some basic functionality you'd expect from a download manager such as resuming incomplete downloads upon relaunch, and limiting the download speed, but (right now) doesn't support saving files outside of your default download directory. I want to change this in the future while still having a minimal set of permissions with Flatpak.

## Building

The easiest way of building Varia is to use GNOME Builder. Just clone this repository, and open the folder using Builder. Then, press run.

If you don't want to use GNOME Builder, or Flatpak, you'll need Meson. Here's how you can install it on some Linux distros:
<br>Ubuntu / Debian: ```sudo apt install meson ninja-build```
<br>Fedora / RHEL / derivatives: ```sudo dnf install meson ninja-build```
<br>Arch: ```sudo pacman -S meson```

After that, you can use these instructions to build and install Varia:
```
git clone https://github.com/giantpinkrobots/varia
cd varia
meson setup builddir
cd builddir
meson compile
meson install
```

## License

<a href=https://github.com/giantpinkrobots/varia/blob/main/LICENSE>Varia is licensed under the Mozilla Public License 2.0.</a>

But, it also application relies on the following pieces of software:
- aria2: GPL v2 License (aria2 itself relies on OpenSSL: OpenSSL License)
- aria2p: ISC License

The licenses of all of these pieces of software can be found in the dependencies_information directory in this application's app directory.

## Contributing

Contributions are always welcome, of course! In the case of translations, they are done with .po files that you can create with a program like Poedit for example. Keep in mind that Varia is kind of a simple app at the moment, and I will keep addding new features so the translations you add right now can become incomplete when I add new features.

Also, I really want to change the logo as it's something I hastly hacked together in Krita. If you can make a logo that conforms to the GNOME logo design guidelines, that would be amazing!

## The name

The name "Varia" comes from the aria2 software it is based on, and I added a "V" to make it "Varia". In the Metroid series of games, there is a special suit you eventually get named a "<a href=https://metroid.fandom.com/wiki/Varia_Suit>Varia Suit</a>" with its main feature being allowing Samus to withstand extreme temperatures. I spent some time thinking about how to connect the Varia Suit to my app, but couldn't, soooo... I think it just sounds cool.

