# Wine to rule them all !

## PLEASE DO NOT REPORT BUGS ENCOUNTERED WITH THIS AT WINEHQ OR VALVESOFTWARE, REPORT HERE INSTEAD !

Wine-tkg-osu is a build-system aiming at easier custom wine-osu build creation.


# Quick how-to :

(for dependencies, see the [wiki page](https://github.com/Tk-Glitch/PKGBUILDS/wiki/wine-tkg-git) )

**Independently of the distro used, you'll want MinGW compiler to build recent wine as it fails to build more often than not without it these days.**


## Download the source :

 * Clone the repo (allows you to use `git pull` to get updates) :
```
git clone https://github.com/Mini-Gaunt/wine-tkg-osu-git.git
```

## Configuration/customization :

If you want to customize the patches and features of your builds, you can find all the settings in [customization-osu.cfg]

You can also create an external configuration file that will contain all settings in a centralized way and survive repo updates.


## Building :

 * We need to get into the wine-tkg-osu-git dir first:
```
cd wine-tkg-osu-git
```

### For Arch (and other pacman/makepkg distros) :

 * From the `wine-tkg-git` directory (where the PKGBUILD is located), run the following command in a terminal to start the building process :
```
makepkg -si
```

### For other distros (make sure to check the [wiki page](https://github.com/Tk-Glitch/PKGBUILDS/wiki/wine-tkg-git)) :

 * From the `wine-tkg-git` directory (where the PKGBUILD is located), run the following command in a terminal to start the building process :
```
./non-makepkg-build.sh
```
**Your build will be found in the `PKGBUILD/wine-tkg-git/non-makepkg-builds` dir (independently of the chosen configuration)**

