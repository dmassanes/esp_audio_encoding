# ESP32 Audio Encoding

This repository contains a collection of various audio encoder ports for the ESP32 LyraT board (https://www.espressif.com/en/products/devkits/esp32-lyrat), including FLAC, MP3, and OPUS. The implementations in this repository are based on Espressif's two main development frameworks: https://github.com/espressif/esp-adf and https://github.com/espressif/esp-idf. All three encoder ports are implemented by adding the corresponding open source libraries as a component to an ESP32 project. There are two examples for each encoder in this repository, one for encoding WAV files on the SD card and one for encoding live recordings generated by the built-in microphones of the ESP32 LyraT.

# NOTE
For now, commits are used only to do preliminary work that serves to plan the project's realization and structure things.

# MP3

The MP3 encoder port is based on the source code from the mp3-shine library provided in https://github.com/toots/shine.

# FLAC

The FLAC encoder port is based on the source code provided in https://github.com/xiph/flac. To avoid any name collisions with the existing codec libraries contained in the esp-adf framework, the prefix "FLAC" was recursively replaced with the prefix "my_FLAC" in the entire component directory.

# OPUS

The MP3 encoder port is based on the source code provided in https://github.com/xiph/opus.

