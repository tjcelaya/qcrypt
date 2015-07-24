# qcrypt

This is a copy of the [AquaQ Analytics](http://aquaq.co.uk) [contrib folder](http://code.kx.com/wsvn/code/contrib/aquaqanalytics/Qcrypt/) for qcrypt, a small interface to the OpenSSL library. Instructions for building the library were rather spread out so I decided to compile them here and include a Makefile in order to make it easier to use. I've included k.h and c.o which were created by [Kx Systems](https://kx.com) for interfacing with q from C.

## Installation

You should be able to get set up with `make` followed by `make install`. Only 32-bit Linux and OS X are targeted, but feel free to submit a pull request!

For reference, on amd64 Debian Jessie I needed to install the following libraries for compilation to succeed:

 - libssl-dev:i386 
 - libc6-dev:i386 (standard c library for 32-bit)
 - libc6-dev-x32 (for cross-compiling)

## Usage

Functions from the library can then be included in Q with:

    qrand:`qcrypt 2: (`qrand;1)

## Disclaimer
This library was initially created by AquaQ Analytics and was released by them, [check out the original article on their site](www.aquaq.co.uk/q/passwords-better-salt-hashing-salting-key-stretching-kdb/).
