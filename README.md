ly2midi
=======

_Convert lilypond files to MIDI_

This tool does three things:

* It removes the `\layout` block from the input .ly file's `\score` block
* If not already present, it adds a `\midi` block with an empty body to the `\score` block
* It invokes `lilypond` on the modified version of the input file

If all these steps succeed (which they may or may not do -- this tool has not been exhaustively tested!)
you end up with a .midi file.

Usage
-----

    ly2midi [-h] [--outfile OUTFILE] lilypondfile

Requirements
------------

* The lilypond package
* The Python argparse module (`easy_install argparse`)
