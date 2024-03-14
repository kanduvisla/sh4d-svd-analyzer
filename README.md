# SH4d SVD Analyzer

An attempt to analyze the Roland SH4D SVD format

## Initial setup

The initial idea is to have a tool that can manage the patterns, presents and rhythm kits of the Roland SH-4d Synthesizer, to provide for some copy/paste functionality that is not available on the device (firmware version 1.030. Think of stuff like: changing order of patterns & banks, backup individual patches, copy kit sounds, etc.

## Disclaimer

__Important:__ Any finding in this document, or even software tools that are added at a later point are to be used __at your own risk__. The auther of this repository is in no way responsible for loss of data, bricked devices or any other damage.

## Findings so far

Using a hex editor on a backup file, the following has already been found:

- The SVD file is 4385916 bytes large.
  - _It's not sure if the backup is always the identical size._\
- Patterns seem to start at byte 128
  - Patterns are 18988 bytes
- Instruments seem to start at byte 2430624
  - Instruments are 2048 bytes
- Rhythm kits seem to start at byte 2956348
  - Rhythm kits are 3328 bytes
