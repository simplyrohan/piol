# piol
Portable I/O Layer for porting small applications between platforms and APIs

## What is it?
Portable Input/Ouput Layer is a specification of functions that allow C code to interact with the I/O of any system without having to worry about the system itself. PIOL abstracts away the video, audio, input, and other system specific calls to the implementation. This allows users to run their app on many platforms by just swapping the PIOL implementation and nothing else. PIOL is made with emulators in mind, but can also work with any software that relies on video, audio, input, and other I/O. PIOL is only a specification of functions, the implementation of these (which is detailed below) is not included in the repository.

## Implementing
PIOL is made for C/C++ projects. We provide the header file, and the corresponding calls are written in the implemetation. These calls depend on what your trying to target. For example, an SDL implemtation would map each call in the header to corresponding SDL logic without the header (or source program) ever worrying/knowing about SDL.

## Specification
Read at [`SPECIFICATION.md`](SPECIFICATION.com)
