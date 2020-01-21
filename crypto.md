## The best simple stream cipher - VMPC (based on RC4)
- Python
  - https://github.com/pvial00/VMPC
  - https://github.com/Gifts/VMPC
- Golang https://github.com/amaximciuc/go-vmpcstream
- C
  - https://github.com/kjopek/vmpc
  - https://github.com/pvial00/VMPCCipher
  - https://github.com/bartek96/vmpc_c
- (Why not RC4 or Spritz? Broken compared to VMPC)
- (VMPC-MAC which is a hash https://eprint.iacr.org/2004/301.pdf)
- (VMPC-R is a bit overkill however)

## RC4 candadite collection
- JS https://github.com/hex7c0/arc4
- Python https://github.com/averykhoo/plaintext-file-fragmentation
- Golang https://github.com/andrewarchi/gocipher
- C https://github.com/AndryRafam/Chinook
- C++ https://github.com/AndryRafam/CastleBravo

## The best hand cipher - LC4
- Python https://github.com/dstein64/LC4
- JS
  - https://github.com/Gavin-Song/elsie-four-cipher
  - https://github.com/umcconnell/lc4
- Golang https://github.com/tonetheman/golang_lc4
- C https://github.com/skeeto/elsiefour
- C# https://github.com/MasterChief-John-117/ElsieFour
- Java https://github.com/ChanceReb/elsie-cipher
- Pencil cersion
  - https://crypto.anarres.info/2016/rc4_pencilandpaper
  - http://mindflare.com/cipher/
- Variant http://ipv6.snipplr.com/view/66235/improved-arc4-iarc4/

## Other Low Tech ciphers
- Aguilar Cipher http://www.sniperflashcards.com/cryptography.php
- Handycipher https://eprint.iacr.org/2014/257.pdf
- LFG https://en.wikipedia.org/wiki/Lagged_Fibonacci_generator
- The last thing you need https://github.com/fruiz500 and https://prgomez.com

## The best card cipher collection
- https://aarontoponce.org/wiki/crypto/card-ciphers
- https://github.com/atoponce/cardciphers/issues
- Bonus: marked decks
  - Classic pip https://www.youtube.com/watch?v=OsbJQaaGXtc
  - Modern scratch https://www.youtube.com/watch?v=R9RlUcOsVaI
  - Advanced https://www.youtube.com/watch?v=YT0lE1uLfuA

## The best elliptic curve - Ed448
- C
  - https://github.com/coruus/ed448-goldilocks (RIP coruus)
  - https://github.com/otrv4/libgoldilocks
  - https://github.com/armfazh/fld-ecc-vec
- Golang
  - https://github.com/otrv4/ed448
  - https://github.com/olabini/goldilocks

## The best crypto library - LibTomCrypt
- https://github.com/libtom/libtomcrypt

## The best sponge functions - NORX
- NORX
  - https://github.com/norx/resources
  - https://github.com/Daeinar/norx-py (Python)
  - https://github.com/therealmik/norxpy (NumPy)
  - https://github.com/kaepora/norx.js (JS)
  - https://github.com/Daeinar/norx-go (Go)

## The best password generator - Diceware
- The most complete site: https://www.rempe.us/diceware
  - The repo https://github.com/grempe/diceware
  - The list https://github.com/grempe/diceware/tree/master/lists
  - Other lists https://github.com/grempe/diceware/issues
- The originalm idea site http://world.std.com/~reinhold/diceware.html
- The comic that led to the idea https://xkcd.com/936/

## The best hashes - SHA3 competition round 2 and finalists
- C and Java
  - https://github.com/coruus/sphlib (RIP Coruus)
  - https://github.com/pornin/sphlib
- JS
  - https://github.com/crdrost/sha3-js
  - https://github.com/thalesfsp/insanehash
  - https://github.com/rainersu/hash
  - https://github.com/dashpay/x11-hash-js (has many clones)
- Golnag (all are the samecopy)
  - https://github.com/phoreproject/go-x11
  - https://github.com/bitbandi/go-x11
  - https://github.com/samli88/go-x11-hash
- C++/C#
  - https://github.com/jar0l/crypto
  - https://github.com/bonesoul/HashLib
  - https://github.com/K2/HashLib
  - https://github.com/mythrill/HashLib
  - https://github.com/brandonlehmann/HashLib

## The best hash documentation
- SHA2 https://nvlpubs.nist.gov/nistpubs/FIPS/NIST.FIPS.180-4.pdf
- SHA3 (Keccak) https://keccak.team/files/Keccak-reference-3.0.pdf
  - KangarooTwelve https://keccak.team/files/KangarooTwelve.pdf
- BLAKE2 https://blake2.net/blake2.pdf
  - BLAKE2 https://131002.net/blake/blake.pdf
  - BLAKE3 https://github.com/BLAKE3-team/BLAKE3-specs/blob/master/blake3.pdf
- Skein http://www.skein-hash.info/sites/default/files/skein1.3.pdf
- Groestl http://www.groestl.info/Groestl.pdf
- Other fast SHA3 round 2 hashes
  - BMW http://people.item.ntnu.no/~danilog/Hash/BMW-SecondRound/Supporting_Documentation/BlueMidnightWishDocumentation.pdf
  - SHABAL https://eprint.iacr.org/2009/199.pdf
  - ECHO https://crypto.orange-labs.fr/echo/doc/echo_description_2-0.pdf
  - Luffa http://www.hitachi.com/rd/yrl/crypto/luffa/Luffa_v2_Specification_20091002.pdf
  - SHAvite3 http://www.cs.technion.ac.il/~orrd/SHAvite-3/Spec.15.09.09.pdf

## Best Passowrd Hashing algorithms - PHC
- https://github.com/bsdphk/PHC

## The best post-quantum crypto algos
- SIDH
  - C https://github.com/microsoft/PQCrypto-SIDH
  - Go https://github.com/cloudflare/sidh
- NTRU
  - https://github.com/NTRUOpenSourceProject
- Go https://github.com/companyzero/sntrup4591761
- New Hope
  - https://github.com/newhopecrypto
  - C https://github.com/vscrypto/ringlwe
  - Go https://github.com/Yawning/newhope
- SPHNICS
  - https://github.com/sphincs

## The best genereal post-quantum cryptography
- https://github.com/PQClean/PQClean
- https://github.com/open-quantum-safe/liboqs/

## The best non-cryptographic hash test
- https://github.com/Cyan4973/xxHash/issues/257

## The primes of the world
- Adobe PGP key leak http://archive.fo/zEneN
- Texas Instruments https://brandonw.net/calculators/keys/
- If you want to go extreme https://en.wikipedia.org/wiki/RSA_numbers

## The best Latin Squares
- https://pthree.org/2018/09/20/latin-squares-mathematics-and-cryptography/

## AACS DVD keys
TBN

## VIC or straddling checkerboard
- http://users.telenet.be/d.rijmenants/en/table.htm

## Enigma Machine
- Java https://github.com/vanitasvitae/EnigmAndroid
- Python https://github.com/cedricbonhomme/pyEnigma
- Docs http://www.cryptomuseum.com/crypto/enigma/wiring.htm
- alternative https://github.com/RealGrep/lorenz-cipher-sim
- Others
  - https://en.wikipedia.org/wiki/Template:Cryptography_machines
  - http://jproc.ca/crypto/

## The best cipher lists
- http://alexbarter.com/cipher-types/
- http://www.cryptogram.org/resource-area/cipher-types/
- http://members.aon.at/cipherclerk/Doc/CipherList.html
- http://practicalcryptography.com/ciphers/
- https://kifanga.com/cryptography-ciphers/
- https://www.braingle.com/brainteasers/codes/index.php
- http://www.elonka.com/UnsolvedCodes.html
- http://rumkin.com/tools/cipher/
- http://ciphermachines.com/types.html
- http://www.cryptoprograms.com/
- https://www.thonky.com/kryptos/types-of-ciphers
- http://alexbarter.com/cipher-types/
- https://ref.wikibruce.com/
