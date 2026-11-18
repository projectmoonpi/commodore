<p align="center"><img src="img/project-moon-pi-logo.png" width="200" alt="Project Moon Pi"></p>
<p align="center"><b>Designed and Created by Project Moon Pi</b></p>

# Project Moon Pi Commodore projects

New software and hardware for the **Commodore 64 and 128**. Everything is written for **NTSC** machines.
On the website: [8-Bit Corner at projectmoonpi.com](https://projectmoonpi.com/8-bit-corner/).

Each project has its own repository with source, build notes and ready-to-run downloads. This page lists them
all. You can also browse the [`commodore-64` topic](https://github.com/topics/commodore-64?q=user%3Aprojectmoonpi).

## Projects

### [Project Moon Pi intro](https://github.com/projectmoonpi/c64-moonpi-intro)

<a href="https://github.com/projectmoonpi/c64-moonpi-intro"><img src="img/c64-moonpi-intro.png" width="480" alt="The Project Moon Pi intro on a C64"></a>

The animated Project Moon Pi logo intro, built to push the C64:
- a starfield and a sprite coin fly-in;
- the badge as an FLI picture, with new colours on every raster line;
- a flare that runs round the ring while sprites move over the FLI picture;
- a three-voice SID score.

**Downloads:** [disk (.d64), program (.prg) and cartridge (.crt)](https://github.com/projectmoonpi/c64-moonpi-intro/releases/latest)

**Machine:** NTSC C64

**Status:** 1.0.0, tested in VICE; real hardware next.

### [Tidal Array 6400](https://github.com/projectmoonpi/tidal-array-6400)

<a href="https://github.com/projectmoonpi/tidal-array-6400"><img src="img/tidal-array-6400.png" width="480" alt="Two cores sharing a Mandelbrot picture"></a>

Several C64s joined into one machine, each one a "core". Step 1 links two C64s through their user ports:
- a small core kernel on each worker;
- a leader that hands out the work;
- a Mandelbrot benchmark that shows the speed-up on screen.

The goal is 8 or more C64s sharing RAM through a cartridge-port hub, all running from one clock.

**Downloads:** [disk (.d64), programs (.prg), cartridges (.crt) and Build Guide 1](https://github.com/projectmoonpi/tidal-array-6400/releases/latest)

**Machine:** NTSC C64s (two for now)

**Status:** 0.1.0. Two cores give a 1.955× speed-up in the two-machine simulator. Real hardware next. The
step 2 clock boards are designed: the Tidal (C)lock master clock and a Tidal Link Interface for each computer's
VIC-II socket (no soldering on the motherboard).

## Coming up

- Tidal Array 6400 hardware: the bench test of the clock boards, then the cartridge-port pod and the shared-RAM hub.
- More user-port and cartridge-port hardware for the C64 (and maybe the C128).

## Tools

The projects are built on a Mac with:
- the [ACME](https://sourceforge.net/projects/acme-crossass/) cross-assembler;
- [Exomizer](https://bitbucket.org/magli143/exomizer/wiki/Home);
- [VICE](https://vice-emu.sourceforge.io/) for testing;
- [OpenCBM](https://github.com/OpenCBM/OpenCBM) for writing real disks.

## Credits

- Project Moon Pi logo and designs: Project Moon Pi.
- Tools: ACME (Marco Baye and contributors), Exomizer (Magnus Lind), VICE (the VICE team), OpenCBM (the
  OpenCBM team). Each project's own README lists its full credits.
- Commodore 64 and Commodore 128 are trademarks of their respective owners. Project Moon Pi is not affiliated with
  them.
- Built with Claude Code (Anthropic).
