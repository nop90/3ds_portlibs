3DS Portlibs
============

Here is a Makefile for building various portlibs for 3DS. You need to first
build zlib and install it. Then you can build the other portlibs.

    $ make zlib
    $ make install-zlib
    $ make <targets>
    $ make install

This will install the portlibs to `$DEVKITPRO/portlibs/armv6k`. If this is a
privileged location, you will need to `sudo make install-zlib` and `sudo make
install` in order for the portlibs to be installed.

Please note: This is an experimental repo, some of these libraries are not
complete ports and will not actually do anything useful without further work.

Currently supports the following portlibs:

* bzip2
* freetype (requires zlib)
* giflib
* jansson
* libconfig
* libexif
* libjpeg-turbo
* libmad
* libogg
* libpng (requires zlib)
* libxmp-lite
* mbedtls (requires zlib) (without net component)
* sqlite
* tinyxml2
* tremor - low memory branch (requires libogg)
* xz
* libmikmod
* zlib
* SDL_ttf (requires SDL to be installed)
* SDL_image (requires SDL to be installed)
* SDL_mixer (requires SDL to be installed)
* SDL_net (requires SDL to be installed)
* SDL_gfx (requires SDL to be installed)
* SDL_sound (requires SDL to be installed)
