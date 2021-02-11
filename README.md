# pixelson
Extracts pixel data from an image and stores it in JSON. For internal use only.

## Usage
Put any MIME-supported image file types in `/input`, and the program will iterate and convert it to a JSON with all pixel data necessary at `/output`.

## Requires
Requires node.js. Populate your node_modules using package.json. Also requires RAM more than 4 GB.
The size of the JSON is big, a 720p image will generate a 16mb JSON file.

One pixel is indexed according to its `IDX` from `JIMP`, it contains the pixel's position (w, h) and its color data (red, green, blue, alpha).

## Importance
Mainly used to counteract image imports in some platforms, by using pixel data to recreate an image individually.

## Packages Used
[JIMP (JavaScript Image Manipulation Program)](https://github.com/oliver-moran/jimp)
[fs-extra](https://github.com/jprichardson/node-fs-extra)
[image-type](https://github.com/sindresorhus/image-type)
