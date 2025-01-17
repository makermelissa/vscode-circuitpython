# Change Log

All notable changes to the "vscode-circuitpython" extension will be documented
in this file.

## [0.1.8]
- all the fun of 0.1.7, but built with proper bindings

## ~~[0.1.7]~~
- Upgraded Electron to 11.2.1
- Updated VSCode version requirement to 1.53.0
- Feb 2021 board refresh

## [0.1.6]
- Jan 2021 board refresh

## [0.1.5]
- Fixed issue installing 6.x mpy stubs on computers that had previous versions

## [0.1.4]
- Improved logic for generating board stubs

## [0.1.3]
- New Azure Pipelie Build
  - Should resolve native binding issues
  - New Boards are added in the build from adafruit/circuitpython:main
    - TODO: Let the user choose their version of CircuitPython, with the boards supported by that version.

## [0.1.2]
- Added `Use Ctrl-C to enter the REPL` on Serial Monitor Connect
- New Boards
  - Radomir Dopieralski : Fluff M0
  - Alorium Technology, LLC : AloriumTech Evo M51
  - maholli : PyCubed
  - PJRC : Teensy 4.1
  - Makerdiary : Pitaya Go
  - Nordic Semiconductor : PCA10100
  - HiiBot : HiiBot BlueFi
  - Espressif : Saola 1 w/WROOM
  - Espressif : Saola 1 w/WROVER

## [0.1.1]
- Updated stubs for Circuit Python 5.3.0
- New Boards
  - NFC Copy Cat
  - ST STM32F746G Discovery - CPy
  - OpenMV-H7 R1
  - Nucleo H743ZI - CPy
  - Nucleo F767ZI - CPy
  - Nucleo F746zg - CPy
  - Simmel
- Native bindings for Raspberry Pi/ARM

## [0.1.0]

- Reworked internals to be less `static`
- more robust autocomplete path handling
- updated stubs for Circuit Python 5.1.0
- new boards

## [0.0.5]

- Removed dialog on serial monitor open
- stores board info in settings.json, which has the effect of persisting your
  board choice for a project between sessions.
- Added command to manually check for bundle update

## [0.0.4]

- Refactored the serial monitor from an output channel to a terminal, allowing
  interaction with the Circuit Python REPL

## [0.0.3]

- More board completions

## [0.0.2]

- Rebuilt for Electron@7
- Reimplemented circup features directly in the extension, see libraryManager.ts for details
  - moves older bundles to the Trash instead of deleting.
- Fixed OS dependent paths ( removed direct calls to path.posix )
- In theory, native bindings should work for windows and mac
  - no linux support yet, but it's on the way. I need to streamline the very
    manual process it took to get these bindings done.

## [0.0.1]

- Initial release