## The best data format - JSON5
- https://json5.org/
- https://github.com/json5/json5 (JS)
- https://github.com/rlidwka/jju (JS utility)
- https://github.com/dpranke/pyjson5 (Python reference)
- https://github.com/Kijewski/pyjson5 (Python fast)
- https://github.com/yosuke-furukawa/json5 (Golang)
- https://github.com/flynn/json5 (Golang)

## The best binary encoding - Safe Encoding
- https://github.com/kstenerud/safe-encoding
- 2nd place: https://github.com/Equim-chan/base91
- 3rd place: https://github.com/kosarev/escapeless
- others: https://github.com/kevinAlbs/Base122

## The best barcodes - Color barcodes
- https://github.com/jabcode/jabcode
- https://github.com/ouyangzhibo/HiQ-Robust-and-Fast-Decoding-of-High-Capacity-Color-QR-Codes
- https://github.com/opencv/opencv/issues/13256

## The best moving barcodes - TxQR
- https://github.com/divan/txqr
- https://github.com/divan/txqr-reader
- https://github.com/divan/txqr-tester-ios
- https://github.com/ThePlasmaRailgun/TXQR-Android
- https://github.com/ThePlasmaRailgun/QRStreamer

## The best paper backup solution - Paperback
- https://github.com/timwaters/paperback
- Alt https://github.com/Wikinaut/paperback-cli
- 2nd place https://github.com/colindean/optar
- Other https://github.com/matheusd/pypaperbak
- Other https://github.com/penma/dpaper
- Other https://github.com/colorsafe/colorsafe
- Other https://github.com/cyphar/paperback

## The best fun Grids - What3Fugs
- https://gitlab.com/IvanSanchez/geogrids

## The best hash visualisation and identicon tools
- Color strip (SVG) https://github.com/bengl/node-hashcolors
- Color strip (ANSI) https://github.com/solosodium/colorful-hash
- Ink Blots https://github.com/stuartpb/hashblot
- Bubbles https://github.com/dakridge/identicon
- Circular https://github.com/ea7ababe/identicon 
- Triangles https://github.com/Mailea/origamicons
- Semi-good designs:
    - Polygons https://github.com/yuvadm/polyhash
    - Ring based https://github.com/Zunawe/identicons
    - Ring based https://github.com/splitbrain/php-ringicon
    - Jagged https://github.com/danfinlay/jazzicon
    - Tornado https://github.com/popodidi/idoticon
    - hexagon https://github.com/naknomum/hexicon
    - Tiles https://github.com/danslocombe/tiledenticon
    - Heart https://github.com/Schlipak/IdentiHeart
- Sound: https://github.com/jasonbot/identijingle
- (Most identicons are either GitHub-like or StackOverflow-like)
- (Too much mirror or rotation symmetry is simply bad)
- (Headshot, animal/alien/robot and emoji based are also bad)

## Converting data into video
```
input=$1; output=$2; width=1280; height=720; block=8 # block cannot be smaller than 8
rate="29.97003" # it can also be "23.976024" or "25" (don't use high speed 48/50/60)
color="monob" # "monow" for BW, "bgr4_byte", rgb4_byte", "bgr8" or "rgb8" for colors
truncate -s %$(($width*$height/($block**2)/8)) $1
ffmpeg -f rawvideo -pix_fmt ${color} -s $(($width/$block))x$(($height/$block)) \
    -r $rate -i $input -vf "scale=iw*${block}:-1" -sws_flags neighbor \
    -threads 8 -deadline best -c:v libvpx -b:v 256k $2
input=$1; output=$2; block=8
ffmpeg -i $1 -vf "format=pix_fmts=${color},scale=iw/${block}:-1" \
    -sws_flags area -f rawvideo $2
```

## The most cryptic art data
- https://libraryofbabel.info/ (contains all random text)
- https://github.com/cakenggt/Library-Of-Pybel
- https://github.com/aneopsy/LibraryOfBabel
- https://github.com/zesterer/babble
- https://github.com/locusf/babel
- https://github.com/murrayc43/LibraryOfBabel
- https://github.com/angrykoala/3d-babel
- https://github.com/mrchucho/babel

