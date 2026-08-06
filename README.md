# stria_live_electronics

Performance material to play: Stria by John Chowning

- This code is based on the Reconstruction - ORChestra csound code
(https://github.com/TheSoundOfAIOSR/csound-web/blob/main/stria.csd)
by Kevin Dahan 2007-2010 (kevin.dahan@wanadoo.fr)

- translated to PD for live-performance by Dustin Zorn (2023) (https://github.com/nitsudnorz), performance score generator in R-Statistics developed (2022-2024) by Dustin Zorn and Alex Hofmann, developed within the artistic research project [Études for Live-Electronics](https://iwk.mdw.ac.at/hofmann/peek-etudes/).

## Usage (to play Stria with the Pure Data patch)

The PD patch is designed to play Stria by John Chowning, as a duet live-electronics performance using two MIDI controllers with faders. It is based on Kevin Dahan's reconstruction of Stria in Csound. Stria contains 383 FM sound events. In this patch, these events can be assigned to a fader either as a group or as individual events.

To play Stria move the faders in the assigned order. With each fader start at 0 and move the fader to the top, when the maximum is reached, the assigned event(s) will finish. Move the fader back to 0 to reset and play the next event(s).

It has been tested with Korg nanoKontrol2 with MIDI-CCs 0-7.

- go into patches/PD/SRIA_PD/
- open Striaport_CsoundtoPD.pd
- PD>Media->MIDI Settings - select your MIDI controllers
- eventually set your PD->Media->Audio Settings
- in the patch click on "DSP on/off" to start the patch
- start moving the faders of you MIDI controllers

If you want to change the assignment of events to faders, edit the file data/score_as_csv/Stria_score_asNumbers_FaderCC.csv

Than open "R-code/Score_Generator.R" and execute it. It will generate the PD/STRIA_PD/faderAssigns/.. files and write a new pdf-score.

The Csound_MidiTester may help to check all assignments automatically. Route the Csound MIDI-Out into the PD MIDI-IN.

(A corresponding Max Patch can be found on Dustins Github: https://github.com/nitsudnorz/StriaFaderpatch.)


## Acknowledgements
This research was funded in whole by the Austrian Science Fund (FWF) [10.55776/AR743].

## License
Distributed under the GNU Lesser General Public License v2.1.
