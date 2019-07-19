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

# Objective

- This image viewer is not designed to be codec-rich
- This image viewer is designed with performance only in mind
- GUI is a tough question:
-- Cross OS agnostic
-- Cross platform agnostic (RPi)
-- Should this work for web browser as well? (WebASM)
- This image viewer incorporates all latest technologies
-- WebASM for web browser native
-- Lossless codec with highest performance (WebP, AVIF)
-- Compression technologies (7z?)

By the end of this project, hopefully the software would be a software that is able to run in high performance on Desktop to Smartphone to Web browser. You shuold also be able to store high quality images in lowest compression size while enjoying highest performance for manga or high quality image viewing.

# Codec in consideration

- AVIF
- PNG
- WebP

# Compression in consideration