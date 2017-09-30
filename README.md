# Extras for themes in RetroPie

At this moment, [Pixel](https://github.com/ehettervik/es-theme-pixel) is the only theme that works with this script because it's the only theme that has [icons](https://github.com/ehettervik/es-theme-pixel/tree/master/retropie/icons), splashscreens ([16:9](https://github.com/ehettervik/es-theme-pixel/blob/master/splash16-9.png) and [4:3](https://github.com/ehettervik/es-theme-pixel/blob/master/splash4-3.png)) and [launching images](https://github.com/ehettervik/es-runcommand-splash).

# Proposal for theme designers/developers

* [Icons](#icons)
* [Splashscreens](#splashscreens)
* [Launching images](#launching-images)

## Icons

### Repository URL

`https://github.com/USERNAME/es-theme-THEME-icons`

e.g. `https://github.com/ehettervik/es-theme-pixel-icons`

### Filetypes

* Icons must be `.png` filetype

### Naming conventions

Same as RetroPie's default icons:

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

### Formatting

Same as RetroPie's default icons:

* Names must be all lowercase
* No spaces

See https://github.com/RetroPie/RetroPie-Setup/tree/master/scriptmodules/supplementary/retropiemenu/icons

## Splashscreens

### Repository URL

`https://github.com/USERNAME/es-theme-THEME-splashscreens`

e.g. `https://github.com/ehettervik/es-theme-pixel-splashscreens`

### Filetypes

* Image splashscreens must be `.png` filetype
* Video splashscreens must be `.mp4` filetype

### Naming conventions

#### Images

* `THEME`-`splashscreen`-`16-9.png`
* `THEME`-`splashscreen`-`4-3.png`

#### Videos

* `THEME`-`splashscreen`-`video.mp4`

e.g `pixel-splashscreen-16-9.png`
e.g `pixel-splashscreen-4-3.png`
e.g `pixel-splashscreen-video.mp4`

### Formatting

* Names must be all lowercase
* Spaces must be hyphens

## Launching images

### Repository URL

`https://github.com/USERNAME/es-theme-THEME-launching-images`

e.g. `https://github.com/ehettervik/es-theme-pixel-launching-images`

### Filetypes

Launching images must be `.png` or `.jpg` filetype

### Naming conventions

* `SYSTEM_NAME/launching.png`

e.g. `nes/launching.png`

See https://github.com/ehettervik/es-runcommand-splash

### Formatting

* Names must be all lowercase
* No spaces
