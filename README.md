

-------------------------
### Run Google Colab

https://colab.research.google.com/drive/1OShIMVcFZ_khsUIBOIV1lzrqAGo1gfm_?usp=sharing

-------------------------


This is a multi-threaded CPU miner for bitcoin.

License: See COPYING for details.

Dependencies:
	libcurl			http://curl.haxx.se/libcurl/
	jansson			http://www.digip.org/jansson/
		(jansson is optional, and is included in-tree)

Basic *nix build instructions:
	./autogen.sh	# only needed if building from git repo
	CFLAGS="-O3 -Wall -msse2" ./configure
	make

Basic WIN32 build instructions (on Fedora 13; requires mingw32):
	./autogen.sh	# only needed if building from git repo
	rm -f mingw32-config.cache
	MINGW32_CFLAGS="-O3 -Wall -msse2" mingw32-configure
	make
	./mknsis.sh

Usage instructions:  Run "minerd --help" to see options.

Also many issues and FAQs are covered in the forum thread
dedicated to this program,
	https://bitcointalk.org/?topic=1925.0;all


----

|  | Donation Address |
| --- | --- |
| ♥ __BTC__ | 1Lw2kh9WzCActXSGHxyypGLkqQZfxDpw8v |
| ♥ __ETH__ | 0xaBd66CF90898517573f19184b3297d651f7b90bf |
