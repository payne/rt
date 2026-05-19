# Dudley's Repeater List

A collection of amateur radio repeater frequencies converted to CHIRP-compatible format.

## Notes from 19 May 2026

1. K0RPT -- no
2. W0JJK -- yes with CTCSS of 131.8
3. K0ASH -- yes but needs a retry
4. KD0PGV -- no.
5. AB0VX -- yes
6. K0BOY -- yes
7. N0YMJ -- no 
8. K0BOY 2 -- yes



## Files

- `list.txt` - Original repeater list in text format
- `repeaters.csv` - CHIRP-compatible CSV file for radio programming

## Conversion Notes

The `repeaters.csv` file was generated from `list.txt` using Claude Code with the following parsing:

### Source Format (list.txt)
Each line contains:
- Frequency with offset direction (+/-)
- Optional CTCSS/PL tone
- Callsign or location name
- Optional description/notes

### Output Format (repeaters.csv)
Standard CHIRP CSV format with columns:
- Location, Name, Frequency, Duplex, Offset, Tone, rToneFreq, cToneFreq, DtcsCode, DtcsPolarity, Mode, TStep, Skip, Comment, URCALL, RPT1CALL, RPT2CALL

### Repeaters Included

| Ch | Name | Frequency | Duplex | Tone | Notes |
|----|------|-----------|--------|------|-------|
| 0 | K0RPT | 147.045 | + | - | NeARES System |
| 1 | W0JJK | 145.235 | - | 131.8 | Storm Spotting |
| 2 | Ashland | 145.310 | - | - | |
| 3 | Valley | 145.265 | - | - | FM and Wires-X |
| 4 | HoneyCreek | 145.410 | - | 97.4 | IRLP connected |
| 5 | K0BOY | 145.450 | - | 131.8 | |
| 6 | N0YMJ | 145.370 | - | - | |
| 7 | K0BOY 2 | 147.360 | + | - | |

### Assumptions
- 2-meter band standard offset: 0.600 MHz
- Mode: FM
- Tuning step: 5.00 kHz
- Entries with specified CTCSS tones use "Tone" mode for transmit

## Usage

1. Open CHIRP
2. Go to File > Open
3. Select `repeaters.csv`
4. Upload to your radio

## Generated

This file was created with assistance from Claude Code (Claude Opus 4.5).
