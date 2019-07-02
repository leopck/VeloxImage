VeloxImage viewer
===========

# Design considerations

- [  ] Performance of the image viewer must be as fast as MangaMeeya
- [  ] Capable of uncompression from compression types (e.g. zip, tar.gz, rar, 7z, ...)
- [  ] Capable of lazy loading
- [  ] Load time between page jumps must not go beyond 500ms
- [  ] Initial loading of images on first startup
- [  ] Loading all images into RAM? Possible memory leak or lack of memory

# Language consideration

- [  ] Language needs to have image codec support
- [  ] Language needs to have good graphics toolkit support
- [  ] Language needs to be able to run on website

# Vision

- [  ] Websites that specializes in image loading would use this library
- [  ] If user wants to save memory and disk, can re-encode all images and compression to more optimize codec (preferred for website hosting)
- [  ] Website is client based, server only provides API for loading the compression file

# Roadmap

- [  ] Using WebAssembly instead of Javascript
