# Pokemon-Save-Dumper
Dump a Game Boy Pokemon Save file over the link port.
The save dumper is based on the work by Francis Stokes and the basic rom dumper he created. It has be modified to extract the save file of MBC3 Game Boy games but it has only been tested on the Game Boy Pokemon Games.
Also included is an example Arduino Script to read the data from the Game Boy link cable as well as a TypeScript program to convert the output into a functioning Game Boy save.

## Tega
Tega is a TypeScript libary created by Francis Stokes on Github.

Francis Stokes - https://github.com/francisrstokes

Tega Base Repo - https://github.com/francisrstokes/tega

## Save Dumper
- Inside \tega\src\save-dumper
The modified save dumper to extract the save file from real cartridges over the link port.

## Bin to Hex
A custom TypeScript program to convert the output generated by the Game Boy into a functioning save file.

## GB_Reader
An exampe Arduino script to read the data from the Game Boy.
Any way of reading raw binary will work however.

## How to install
Requirements:

    - ts-node (tega)

    - typescript (bintohex, tega)

To build save-dumper.gb

    - run ts-node index.ts in the save-dumper folder

To run bintohex

    - run tsc bintohex.ts then node bintohex.js input.txt output.sav; where the input.txt is the output from the Game Boy

## Credts
Tega, Base Save Dumper Code - Francis Stokes (https://github.com/francisrstokes)