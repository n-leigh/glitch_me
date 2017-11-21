# glitch_me
Python module to add some distortion/glitch effects to images.

Inspired by the work of [DataErase](http://dataerase.tumblr.com/).

## Dependencies
- [Python 3](https://www.python.org/)
- [Pillow 4.x](https://pypi.python.org/pypi/Pillow/)

## tl; dr
```
git clone https://github.com/noahleigh/glitch_me.git
python ./glitch_me image_folder/*.png output_folder --line_count 120
```

## Usage
`python ./glitch_me {INPUT} {OUTPUT} --line_count {LINE_COUNT}`

 - The `glitch_me` folder is a Python module, so that's what you pass to the `python` executible
 - `INPUT` is the path to the image you want to glitch, or a glob pattern to the images you want to glitch.
 - `OUPUT` is the path to the directory where you want the glitched images to be stored. The files will be named `{ORIGINAL_NAME}_glitch.png`
 - `LINE_COUNT` is the number of vertical pixels you want the image scaled down to before performing the glitches.
 The image will be upscaled back to it's original resolution while maintaining the pixelation.

## Examples using the included transforms
| Original | Glitched |
|----------|----------|
|![tokyo](readme_assets/tokyo_small.png) | ![tokyo glitched](readme_assets/tokyo_small_glitch.png) |
|![cafe](readme_assets/cafe_small.png) | ![cafe glitched](readme_assets/cafe_small_glitch.png) |
|![gate](readme_assets/gate_small.png) | ![gate glitched](readme_assets/gate_small_glitch.png) |
