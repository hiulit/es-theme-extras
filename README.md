# Extras for RetroPie themes

This scripts let's you install some extras for RetroPie themes. These extras are:

* Icons
* Splashscreens
* Launching images

![Install Pixel](example-images/example-01.jpg "Install Pixel")
![Update or Uninstall Pixel](example-images/example-02.jpg "Update or Uninstall Pixel")
![Extras](example-images/example-03.jpg "Extras")
![Install Pixel icons](example-images/example-04.jpg "Install Pixel icons")
![Install Pixel splashscreen](example-images/example-05.jpg "Install Pixel splashscreen")
![Choose splashscreen](example-images/example-06.jpg "Choose splashscreen")
![Install Pixel launching images](example-images/example-07.jpg "Install Pixel launching images")

## Installation

```
git clone https://github.com/hiulit/es-theme-extras.git
cd es-theme-extras/
./es-theme-extras.sh
```

At this moment, [Pixel](https://github.com/ehettervik/es-theme-pixel) is the only theme that works with this script because it's the only one (that I know of) that has [icons](https://github.com/ehettervik/es-theme-pixel/tree/master/retropie/icons), splashscreens ([16:9](https://github.com/ehettervik/es-theme-pixel/blob/master/splash16-9.png) and [4:3](https://github.com/ehettervik/es-theme-pixel/blob/master/splash4-3.png)) and [launching images](https://github.com/ehettervik/es-runcommand-splash).

Pixel theme has both icons and splashscreens in the same repository and launching images has its own repository.

This script is created under these premises:

* Icons and splashscreens must be in the same repository `https://github.com/USERNAME/es-theme-THEME`
* Icons must be in path `/retropie/icons`
* Splashscreens must be in the root path and named `splash16-9.png` and/or `splash4-3.png`
* Launching images must be in another repository `https://github.com/USERNAME/es-runcommand-splash`

I think that could be standarized so that every theme could take advantage of this script.

## Proposal for standarization

I propose two versions:

* [Self-contained](#self-contained-same-repository-version): All extras in the same repository
* [Diferent repositories](#diferent-repositories-version) for each extra (icons, splashscreens and launching images)

When the decision is made, I'll make the necessary changes according to the version agreed upon.

### Self-contained (same repository) version

#### Theme URL

`https://github.com/USERNAME/es-theme-THEME`

e.g. `https://github.com/ehettervik/es-theme-pixel`

#### Icons URL

`https://github.com/USERNAME/es-theme-THEME/retropie/icons`

e.g. `https://github.com/ehettervik/es-theme-pixel/retropie/icons`

#### Splashscreens URL

`https://github.com/USERNAME/es-theme-THEME/retropie/splashscreens`

e.g. `https://github.com/ehettervik/es-theme-pixel/retropie/splashscreens`

### Launching images URL

`https://github.com/USERNAME/es-theme-THEME/retropie/launching-images`

e.g. `https://github.com/ehettervik/es-theme-pixel/retropie/launching-images`

### Diferent repositories version

#### Theme URL

`https://github.com/USERNAME/es-theme-THEME`

e.g. `https://github.com/ehettervik/es-theme-pixel`

#### Icons URL

`https://github.com/USERNAME/es-theme-THEME-icons`

e.g. `https://github.com/ehettervik/es-theme-pixel-icons`

#### Splashscreens URL

`https://github.com/USERNAME/es-theme-THEME-splashscreens`

e.g. `https://github.com/ehettervik/es-theme-pixel-splashscreens`

### Launching-images URL

`https://github.com/USERNAME/es-theme-THEME-launching-images`

e.g. `https://github.com/ehettervik/es-theme-pixel-launching-images`

## Filetype, naming convention and formatting

In both cases the filetype, naming convention and formatting must be the same, as follows:

* [Icons](#icons)
* [Splashscreens](#splashscreens)
* [Launching images](#launching-images)

### Icons

#### Filetype

* Icons must be `.png` filetype

#### Naming conventions

Names must be the same as RetroPie's default icons:

* audiosettings.png
* bluetooth.png
* configedit.png
* esthemes.png
* filemanager.png
* raspiconfig.png
* retroarch.png
* retronetplay.png
* rpsetup.png
* runcommand.png
* showip.png
* splashscreen.png
* wifi.png

See https://github.com/RetroPie/RetroPie-Setup/tree/master/scriptmodules/supplementary/retropiemenu/icons

#### Formatting

Same as RetroPie's default icons:

* Names must be all lowercase
* No spaces

See https://github.com/RetroPie/RetroPie-Setup/tree/master/scriptmodules/supplementary/retropiemenu/icons

### Splashscreens

#### Filetype

* Image splashscreens must be `.png` filetype
* Video splashscreens must be `.mp4` filetype

#### Naming conventions

#### Images

* `THEME`-`splashscreen`-`16-9.png`

e.g `pixel-splashscreen-16-9.png`

* `THEME`-`splashscreen`-`4-3.png`

e.g `pixel-splashscreen-4-3.png`

#### Videos

* `THEME`-`splashscreen`-`video.mp4`

e.g `pixel-splashscreen-video.mp4`

#### Formatting

* Names must be all lowercase
* Spaces must be hyphens

### Launching images

#### Filetype

Launching images must be `.png` or `.jpg` filetype

#### Naming conventions

* `SYSTEM_NAME/launching.png`

e.g. `nes/launching.png`

See https://github.com/ehettervik/es-runcommand-splash

#### Formatting

* Names must be all lowercase
* No spaces

## Credits

Filetype, naming conventions and formatting taken (partially and revisited) from [ retropie-splashscreens-extra repository by HerbFargus](https://github.com/HerbFargus/retropie-splashscreens-extra/blob/master/README.md)
