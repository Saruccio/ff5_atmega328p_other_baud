# ff5_atmega328p_other_baud
FlashForth for ATmega328P recompiled for custom baud rate released in the hope that they will be useful.

This repository provides precompiled `.hex` binaries and configuration sources for **FlashForth 5** configured with 
serial baud rates not available in the main distribution.

At the moment, the `.hex` binaries available are:
- **115200:** `328-16MHz-115200.hex`
- **500000:** `328-16MHz-500000.hex`

The images were recompiled from source taken from official SourceForge repository, specifically commit:

**flashforth-code-6f2fd267ac54cb6cf166e29eaad3a9134170dfa0**

To recompile the sources I installed the latest MPLABX suite with all optional packages on a Linux system,
opened the project `flashforth/avr/FF-ATMEGA.X`,
and let the IDE perform an automatic conversion before building.

To change the baud rate, I edited the file `flashforth/avr/src/config-xc8.inc` directly within the IDE.

All `.hex` binaries have been tested successfully on my Arduino Nano V3 (ATmega328P) across various hobby projects.

---

## License & Attribution

This project is derivative work based on FlashForth, originally created and copyrighted by Mikael Nordman.
GNU General Public License v3.0 (GPLv3)

FlashForth and this repository are licensed under the GNU General Public License v3.0.

    FlashForth 5

    Copyright (C) Mikael Nordman

    Web: http://flashforth.com / SourceForge: https://sourceforge.net/projects/flashforth/

Under the terms of the GPLv3:

    You are free to run, study, share, and modify this software.

    Any distributed binaries or modified versions must also be made available under the GPLv3 license along with the corresponding source code / build configurations.

    This software comes with ABSOLUTELY NO WARRANTY.

See the full license text in the LICENSE file included in this repository or visit https://www.gnu.org/licenses/gpl-3.0.html.

### Acknowledgments

    Mikael Nordman for creating and maintaining the FlashForth system.

    The FlashForth community for ongoing hardware support and documentation
    
