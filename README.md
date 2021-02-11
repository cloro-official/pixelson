# pixelson
Extracts pixel data from an image and stores it in JSON. For internal use only.

## Usage
Put any MIME-supported image file types in `/input`, and the program will iterate and convert it to a JSON with all pixel data necessary at `/output`.

## Requires
Requires node.js. Populate your node_modules using package.json. Also requires RAM more than 4 GB.
The size of the JSON is big, a 720p image will generate a 16mb JSON file.

## Importance
Mainly used to counteract image imports in some platforms, by using pixel data to recreate an image individually.
