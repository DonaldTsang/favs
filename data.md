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
- Very smart https://gitlab.com/IvanSanchez/geogrids
  - Side note: 45 bits for 4.78m accuracy, 47 bits for 2.39m, 49 bits for 1.19m
- Basic https://en.wikipedia.org/wiki/ISO_6709
- Recommended https://en.wikipedia.org/wiki/Geohash
- ALternative https://plus.codes/
- Others
  - http://www.makaney.net/mkc_standard.html
  - https://en.wikipedia.org/wiki/Military_Grid_Reference_System
  - https://en.wikipedia.org/wiki/Postal_addresses_in_the_Republic_of_Ireland#OpenPostcode
- Do not use irregular scaling
  - https://en.wikipedia.org/wiki/Maidenhead_Locator_System
  - https://en.wikipedia.org/wiki/World_Geographic_Reference_System
  - https://en.wikipedia.org/wiki/C-squares
  - https://en.wikipedia.org/wiki/Global_Area_Reference_System
- Do not use irregular grid shapes
  - https://en.wikipedia.org/wiki/Universal_Transverse_Mercator_coordinate_system
  - https://en.wikipedia.org/wiki/Universal_polar_stereographic_coordinate_system
  - https://en.wikipedia.org/wiki/Quadrilateralized_spherical_cube
  - http://www.sai.msu.su/~megera/wiki/SphereCube
  - http://s2geometry.io/
- Do not use proprietary naming schemes
  - https://what3words.com/
  - https://en.wikipedia.org/wiki/Natural_Area_Code
- Do not use overly large divisions
  - https://en.wikipedia.org/wiki/Marsden_square
  - https://en.wikipedia.org/wiki/World_Meteorological_Organization_squares
- Do not use low entropy formats
  - https://en.wikipedia.org/wiki/QDGC

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

## Converting data into audio
- https://github.com/rraval/pied-piper

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

## The best decentralization info
- https://github.com/redecentralize/alternative-internet

## The best compression benchmark
- https://github.com/powturbo/TurboBench
- 2nd place http://pages.di.unipi.it/farruggia/dcb/
- For the crazies:
  - http://www.mattmahoney.net/dc/text.html
  - More benchmarks at http://www.mattmahoney.net/dc
  - And https://cs.fit.edu/~mmahoney/compression/
  - https://www.maximumcompression.com/data/summary_mf3.php
  - http://qlic.altervista.org/

## The best file format standard docs
- https://coptr.digipres.org/Category:File_Format_Identification
- https://knihovnarevue.nkp.cz/kplus-text-en/archives/2015-2/library-and-information-at-home/digital-preservation-from-theory-to-practice#endref32
- https://madfileformatscience.garymcgath.com/tag/fident/
