# stria_live_electronics

;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;
;;; Stria
;;; by John Chowning
;;; This code is based on the Reconstruction - ORChestra csound code
;;; (https://github.com/TheSoundOfAIOSR/csound-web/blob/main/stria.csd)
;;; by Kevin Dahan 2007-20010
;;; kevin.dahan@wanadoo.fr
;;; translated to PD for live-performance by Dustin Zorn (https://github.com/nitsudnorz)
;;; performance score generator in R-Statistics developed by Dustin Zorn and Alex Hofmann
;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;


This PD patch is designed to play Stria by John Chowning, as a duet live-electronics performance using two MIDI controllers with faders. It is based on Kevin Dahan's reconstruction of Stria in Csound. Stria contains 383 FM sound events. In this patch, these events can be assigned to a fader either as a group or as individual events.

To play Stria, move the faders in the assigned. The following logic applies: Start at 0 and move the fader, when the maximum is reached, the assigned event(s) will finish. Move the fader back to 0 to reset and play the next event(s).

It has been tested with Korg nanoKontrol2 with MIDI-CCs 0-7.
