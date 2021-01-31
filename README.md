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

---

### Analog Rytm

This file includes three instrument definitions:

* Rytm
* Rytm trak
* Rytm FX

**Rytm** is assigned to the instrument's MIDI "auto channel" and is intended for non-chromatic use of all tracks/voices of the instrument on a single Cirklon track. This is optimal for CK patterns, where each voice's trigger note has a labeled and persistent row. This is also the default channel for MIDI program changes (which correspond to pattern changes on the instrument).

**Rytm trak** is multi-timbral and intended for use of a single track/voice of the instrument on a Cirklon track. This allows for modulation of any of the voice's parameters via CC / track values. By default, the individual tracks operate on the first 12 MIDI channels.

**Rytm FX** is the FX track on the instrument. This is not intented for sequencing of voice triggers but rather for modifying the parameters of the FX track.

---

### Moogs

Moog synths, for parameters with discrete value sets, still spread the values across the entire 128-value CC range. For example, on/off parameters are CC value 0-63 = off and 64-127 = on. A parameter with three values has them associated with the CC value ranges 0-42, 43-84, and 85-127. Cirklon doesn't yet provide a CC "step size" or value subset or some other way to deal with this, so the only parameters that I have attempted to constrain are on/off ones, since I could make those 63 min and 64 max.
