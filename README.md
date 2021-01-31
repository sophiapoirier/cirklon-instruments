# Cirklon instrument definitions

These are my instrument definition files for the Cirklon sequencer. Included are:

* Elektron Analog Heat MKII
* Elektron Analog Rytm MKII
* Erica Synths Syntrx
* Korg Minilogue XD
* Moog Matriarch
* Moog Subsequent 37
* Novation Bass Station II

Most of these are self-explanatory if you are a Cirklon user, but for those warranting extra notes:

### Analog Rytm

This file includes three instrument definitions:

* Rytm
* Rytm trak
* Rytm FX

**Rytm** is assigned to the instrument's MIDI "auto channel" and is intended for non-chromatic use of all tracks/voices of the instrument on a single Cirklon track. This is optimal for CK patterns, where each voice's trigger note has a labeled and persistent row. This is also the default channel for MIDI program changes (which correspond to pattern changes on the instrument).

**Rytm trak** is multi-timbral and intended for use of a single track/voice of the instrument on a Cirklon track. This allows for modulation of any of the voice's parameters via CC / track values. By default, the individual tracks operate on the first 12 MIDI channels.

**Rytm FX** is the FX track on the instrument. This is not intented for sequencing of voice triggers but rather for modifying the parameters of the FX track.