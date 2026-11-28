# M490F Stereo Input Module · Input Pre Amps

Ward-Beck Systems M490F, 1978|11. Wiki page: [M490F on WBSps.ca](https://wardbecksystems.github.io/WBSps.ca/WBSps.ca/Github.WardBeckSystems/MODULES.INPUT-PRE-AMPS.M490F-Stereo-Input-Module/)

| Folder | What is in it | Files |
|---|---|---|
| [SCHEMATICS/](SCHEMATICS/) | electrical drawings: schematics, functional diagrams, component layouts, wiring | 40 |
| [MECHANICAL/](MECHANICAL/) | front panels, cover plates, metalwork, assemblies; the front panel as vectors | 11 |
| [PINOUTS/](PINOUTS/) | the RTO-144 connector: connection sheets, connector layouts, rear views | 10 |
| [MANUALS/](MANUALS/) | manuals, manual pages, price lists, brochures, documents | 254 |
| [PHOTOS/](PHOTOS/) | photographs of the module | 3 |
| [KICAD/](KICAD/) | KiCad schematics traced from the drawings, the symbol, PCB projects | 13 |
| [OCR/](OCR/) | the note of every file: date, origin, title block, OCR text | 65 |

<!-- module data: tools/module_specs.py, tools/forum_quotes.py -->

**On the WBSps forum (2006|39 - 2014|47):** [12 topics](FORUM.md): what owners and technicians said about it.

## Specifications

From the technical data sheet: [1978 - M490F - 004.jpg](MANUALS/1978%20-%20M490F%20-%20004.jpg) page 1 (read by OCR; check against the page). As data: [`Specifications.json`](Specifications.json).

| | |
|---|---|
| **Input sensitivity** | Frequency Response: -10 to +10 dBm (ref. 600 ohm source) ±0.5 dB from 30 Hz to 20 kHz_:, ^ '.:. Noise: 75 dB be Tow nomina [ operating Teve]: `. with mixing attenuator set at 15 dB o. 3 s in-hand&quot; (20 Hz to 20 kHz) _. 7&lt;:..... ` Harmonic Distortion: Less than 0.35% THD from 30 Hz to /, ' 20 kHz at 20 dB above nomina ] 4'.; operating Teve] or Tess ` /d.:: Less than 0.1% at kHz at 20 dB:&gt;^. s above nomina] operating level or Tess _ ';.X Less than 0.5 % at kHz through cue P.. channe] at 20 dB above nomina ] operating Teve] or Tess ` Source Impedance: 600 ohms or less, balanced. &quot;. 4... Input Impedance: 30, 000 ohms |
| **Output impedances** | edo,. n. Output Leve]: 30,000 ohms balanced (program circuits) 60,000 ohms balanced (cue circuits) _ 0 dBm nomina] +22 dBm maximum |
| **Channel separation** | 50 dB from 50 Hz to 15 kHz. |
| **Phasing** | Input and output terminals designated by numbers are in phase, or Tower number of numbered pair is in phase with ower number of other numbered pair |
| **Input levels** | (to operate ch ON CH OFF:` {.s U. Logic 0: 0 to +13 volts.,. '`.' Logic 1: +16 to +24 volts Ut 4. =. '..:. ': ^. ` 3.. '..:.; '.. 7`... ` 4.` ' a &quot;.. |

## Circuit description

From [1978 - M490F - 007.jpg](MANUALS/1978%20-%20M490F%20-%20007.jpg) page 1 (read by OCR; check against the pages). As data: [`CircuitDescription.json`](CircuitDescription.json).

<details><summary>Read it</summary>

M490F STEREO InpuT MODULE M490F STEREO InPUt MODULE number of individual input functions govern the status of the dual flip-flop 210 _ description of each input function follows Pin of P2 is isolated through diode CR4 When connected in para ] Tel with the same output of other modules it provides convenient or gate configuration, suitable to reset common timer each time CHANNEL on button is depressed. 2:. Channel 0ff.;.. Momentary operation of the CHANNEL OFF switch Sw8 or momentary ground closure of the EXTERNAL CHANNEL OFF control input at P2, pin 12 Wil result in negative going pulse at 210 pin and &quot;clear the A-section of 210 producing volts at 210, pin 15 Consequently the Teft and right solid state PROGRAM switches wil switch OFF, Q7 will stop conducting causing DS3 to extinguish, and the muting contro] outputs at P2, pins 13 and Wi1l be disabled _. separate contact is ava i lab ]e on Sw8 and is ^ accessible at P2, pins 17/U. It maybe used for machine top&quot; 60 `. separate CHANNEL 0FF tally Tamp is built into Sw8 and is connected to P2 pins 18/V.. '... In addition to the norma 1 pushbutton operated 2 CHANNEL 0FF function, both Teft and right solid state PROGRAM switches are switched 0FF whenever the mixing attenuator 15 moved to the infinite position and switch SW10 is closed The vo ]t 21 ` potential] developed at 29 pin 10 is fed directly. ' to the two PROGRAM switches and causes them to ^. switch OFF However, the status of 210 the CHANNEL on indicator and the muting controls, _ remain unaffected by this operation _ (^ &quot;):. ^.'. Aa..:.: &lt;.: &gt;. Cue '.... n... ', 6 `., to `;. a 4'.. ` The B-section of 210 is used to contro] the solid state ' CUE switches The flip-flop will change state each.a time negative g0 ing transition takes pace at pin 2 of 210 Consequently, with each input pulse, the &quot;' CUE channels willa Iternate between on and 0FF ~.` &quot;,.: ` ` ` Initial Reset When power is initially applied to the system, the ion Bomhi&quot;cteon &quot;fnFRt? _fRZia CRz3] acd8c38 FullyPcharged; thus ensuring that all so] id state switches are in the {, OFF position... a P Channel On Momentary operation of the ChAnNEL ON switch SWg wil] Produce negative going pulse at 210 pin and {`.. preset the A-section of 210. Alternatively, momentary ground closure of the EXTERNAL CHANNEL on. control nput at P2, pin Will result in the same. condition. &quot;.. &lt;.`:.. 3; &quot; ` ' Once the flip-flop is &quot;preset&quot; its output at Pin 15 changes from to (approximately +10 volts) This Wi1] cause the Teft and right PROGRAM switches to switch on Furthermore, Q7 will saturate resulting in the CHANNEL on indicator Tamp DS3 to switch on With Q7 saturated the contro] common potential] '.;` appears at the emitters of Q8 and Q9 A' positive.^ base potential] is app] ied to either Q8 or Q9 depend ing on whether InPUt SELECTOR switch SW1 or SW2 is depressed Effectively Q8 and Q9 operate, similarly to two AND gates The co ]vectors of the &lt;.. two transistors represent the outputs of the AND gates They appear at P2, pin 13 and These terminals are:` capab ] e of sinking maximum current of 40 mA each:cc % from 24 vot source and maybe used for muting. ' G purposes... u{ ' When operating the CHANNEL on switch Sw9 separate &quot;.^ contact is closed accessible at P2, Pins 15/5 This &quot;A1 contact maybe used for simultaneous machine start.

</details>

<!-- /module data -->

## Photos

_Photographs of the module itself: front, back, inside, racked._

<table>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKX204N283RDdHT0k/view?resourcekey=0-aQZeth1ElqcTqYS0VUFlNw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKX204N283RDdHT0k&resourcekey=0-aQZeth1ElqcTqYS0VUFlNw" width="240" alt="1978 - M490F - Input Module.jpg"></a><br><sub>1978|11 · Input Module</sub></td></tr>
</table>

Shared privately on Google Drive (opens after sign-in): [1978|11 · Input Module _small](https://drive.google.com/file/d/0B0yR0b5T78SKMlpmZEZlam5rNUE/view?resourcekey=0-ussf-pmC_zVPSN4-9bFp1w)

## Mechanical

_Mechanical drawings: front panels, cover plates, metalwork and hardware (-03- drawings), AutoCAD files, each with its `(EXTRACTED).svg` vectors; `<module> - front panel.svg` is the front panel as vectors._

<table>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKLVE4QTEzRUd4TjA/view?resourcekey=0-jWKLxTi669xez-5KfQKVug" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKLVE4QTEzRUd4TjA&resourcekey=0-jWKLxTi669xez-5KfQKVug" width="240" alt="1978 - M490F - 490-04-014 - USED FOR IGNA PURPOSES FROM REMOTE LOCATION.jpg"></a><br><sub>1978|11 · 490-04-014 - USED FOR IGNA PURPOSES FROM REMOTE LOCATION · <a href="MECHANICAL/1978%20-%20M490F%20-%20490-04-014%20-%20USED%20FOR%20IGNA%20PURPOSES%20FROM%20REMOTE%20LOCATION%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKTHk4THo2RzRjQlk/view?resourcekey=0-9iAcWQjGhY57yCHbi2BAhw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKTHk4THo2RzRjQlk&resourcekey=0-9iAcWQjGhY57yCHbi2BAhw" width="240" alt="1978 - M490F - 90-04-014 - STEREO INPUT MODULE FRONT PANEL.jpg"></a><br><sub>1978|11 · 90-04-014 - STEREO INPUT MODULE FRONT PANEL · <a href="MECHANICAL/1978%20-%20M490F%20-%2090-04-014%20-%20STEREO%20INPUT%20MODULE%20FRONT%20PANEL%20(EXTRACTED).svg">vectors</a></sub></td></tr>
</table>

## 3-D model

[`MECHANICAL/M490F.stl`](MECHANICAL/M490F.stl) (GitHub turns it in 3-D) · [view, change and generate it on WBSps.ca](https://wardbecksystems.github.io/WBSps.ca/2026/stl.html?m=M490F)

- **Size:** 49.87 × 301.83 mm panel, 165 mm deep, 3.2 mm plate (the drawing sheet, taken as drawn 1:1)
- **From the drawing:** 14 holes and cut-outs, 1 knobs (front panel: `MECHANICAL/M490F - front panel.svg`)
- the drawn panel is 0.11 wide to high, the size 0.17: placed by its height
- Made by `tools/module_models.py` (→ `MECHANICAL/M490F.model.json`) and `tools/stl/make_stl.mjs` in [WBSps.ca](https://github.com/WardBeckSystems/WBSps.ca); the site makes the same STL from the same JSON.

## Schematics

_Electrical drawings: schematics (-02-), functional diagrams (-01-), component layouts (-06-), wiring (-09-), PCB files (.pcb .dsn), and beside each scan its `(EXTRACTED).svg`: the vectors traced from it._

<table>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKMTl1UjFhT2t0NWM/view?resourcekey=0-rjYF9RqVvTPSta8uSpraKA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKMTl1UjFhT2t0NWM&resourcekey=0-rjYF9RqVvTPSta8uSpraKA" width="240" alt="1978 - M490F - 490-01-006 - ISTART TIMER RESET OFF TALLY OFFISTOP.jpg"></a><br><sub>1978|11 · 490-01-006 - ISTART TIMER RESET OFF TALLY OFFISTOP · <a href="SCHEMATICS/1978%20-%20M490F%20-%20490-01-006%20-%20ISTART%20TIMER%20RESET%20OFF%20TALLY%20OFFISTOP%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKZW1Pb3FWTUdubHM/view?resourcekey=0-s5OM56qpnA--xlRQSxhc3g" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKZW1Pb3FWTUdubHM&resourcekey=0-s5OM56qpnA--xlRQSxhc3g" width="240" alt="1978 - M490F - 490-01-006 - MACHINE CONTROLS REVISED.jpg"></a><br><sub>1978|11 · 490-01-006 - MACHINE CONTROLS REVISED · <a href="SCHEMATICS/1978%20-%20M490F%20-%20490-01-006%20-%20MACHINE%20CONTROLS%20REVISED%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKZkJCRlA2SUZ5dFE/view?resourcekey=0-YBMB4_cdCUGSWBggMmoE6g" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKZkJCRlA2SUZ5dFE&resourcekey=0-YBMB4_cdCUGSWBggMmoE6g" width="240" alt="1978 - M490F - 490-02-007 - RIIE IOOK.jpg"></a><br><sub>1978|11 · 490-02-007 - RIIE IOOK · <a href="SCHEMATICS/1978%20-%20M490F%20-%20490-02-007%20-%20RIIE%20IOOK%20(EXTRACTED).svg">vectors</a></sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKV3VRRnhnY3A3eUE/view?resourcekey=0-jEyjtaj9zpccYO36fCeKOA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKV3VRRnhnY3A3eUE&resourcekey=0-jEyjtaj9zpccYO36fCeKOA" width="240" alt="1978 - M490F - 490-02-007 - STEREO INPUT MODULE.jpg"></a><br><sub>1978|11 · 490-02-007 - STEREO INPUT MODULE · <a href="SCHEMATICS/1978%20-%20M490F%20-%20490-02-007%20-%20STEREO%20INPUT%20MODULE%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKdUhEa2hxMlo4RnM/view?resourcekey=0-ssO2bIHl5u5m0K_allXcFg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKdUhEa2hxMlo4RnM&resourcekey=0-ssO2bIHl5u5m0K_allXcFg" width="240" alt="1978 - M490F - 490-06-007 - IBS CANAD.jpg"></a><br><sub>1978|11 · 490-06-007 - IBS CANAD · <a href="SCHEMATICS/1978%20-%20M490F%20-%20490-06-007%20-%20IBS%20CANAD%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKMUprQzFPaVYwVUU/view?resourcekey=0-WJSFSOitzWWu_3OPR32Z2A" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKMUprQzFPaVYwVUU&resourcekey=0-WJSFSOitzWWu_3OPR32Z2A" width="240" alt="1978 - M490F - 7-112-02-001 - ALL CAPACITORS.jpg"></a><br><sub>1978|11 · 7-112-02-001 - ALL CAPACITORS · <a href="SCHEMATICS/1978%20-%20M490F%20-%207-112-02-001%20-%20ALL%20CAPACITORS%20(EXTRACTED).svg">vectors</a></sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKTDFNZ2I0aUdUazQ/view?resourcekey=0--LSUQ97q6FGAAz11ozaUfA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKTDFNZ2I0aUdUazQ&resourcekey=0--LSUQ97q6FGAAz11ozaUfA" width="240" alt="1978 - M490F - 7-112-02-001 - CHANNEL AMPLIFIER SCHEMATIC ISSUL.jpg"></a><br><sub>1978|11 · 7-112-02-001 - CHANNEL AMPLIFIER SCHEMATIC ISSUL · <a href="SCHEMATICS/1978%20-%20M490F%20-%207-112-02-001%20-%20CHANNEL%20AMPLIFIER%20SCHEMATIC%20ISSUL%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKaDd6dG0xRU5jTkE/view?resourcekey=0-BOqg_fQscmW2lYbTDQaJVw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKaDd6dG0xRU5jTkE&resourcekey=0-BOqg_fQscmW2lYbTDQaJVw" width="240" alt="1978 - M490F - 7-112-06-001 - CHANNEL AMPLIFIER COMPONENT LAYOUT.jpg"></a><br><sub>1978|11 · 7-112-06-001 - CHANNEL AMPLIFIER COMPONENT LAYOUT · <a href="SCHEMATICS/1978%20-%20M490F%20-%207-112-06-001%20-%20CHANNEL%20AMPLIFIER%20COMPONENT%20LAYOUT%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKTUh5OUVLWkdBVzQ/view?resourcekey=0-b-u1j-WPtdp3nR19YyCspQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKTUh5OUVLWkdBVzQ&resourcekey=0-b-u1j-WPtdp3nR19YyCspQ" width="240" alt="1978 - M490F - 7-112-06-001 - COMPONENT SIDE NOTE COMPONENTS.jpg"></a><br><sub>1978|11 · 7-112-06-001 - COMPONENT SIDE NOTE COMPONENTS · <a href="SCHEMATICS/1978%20-%20M490F%20-%207-112-06-001%20-%20COMPONENT%20SIDE%20NOTE%20COMPONENTS%20(EXTRACTED).svg">vectors</a></sub></td></tr>
</table>

## Pinouts

_Pinouts: the RTO-144 edge connector (connection sheets, connector layouts and rear views, strapping), and the pinout / connections drawings made from them. The module root `RTO.json` lists every contact._

<table>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKOTZ0RGlMWlY0eGc/view?resourcekey=0-QyPCHnHvORsjqJ_L8Bikgw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKOTZ0RGlMWlY0eGc&resourcekey=0-QyPCHnHvORsjqJ_L8Bikgw" width="240" alt="1978 - M490F - 490-04-007 - CONNECTOR REAR VIEW.jpg"></a><br><sub>1978|11 · 490-04-007 - CONNECTOR REAR VIEW · <a href="PINOUTS/1978%20-%20M490F%20-%20490-04-007%20-%20CONNECTOR%20REAR%20VIEW%20(EXTRACTED).svg">vectors</a></sub></td></tr>
</table>

## RTO-144 pinout

Read from 1 pinout picture (each its own `.pinout.json` beside it); the RTO-144 sheet agrees on 15 of 15 contacts. Every contact, with where it was read: [`RTO.json`](RTO.json). How a picture becomes this table: [the pinout decision tree](https://github.com/WardBeckSystems/WBSps.ca/blob/main/2026/Engineering/PINOUTS.md).

**To check:**

- insert guessed: recorded as a send/return pair per channel, but the send/return assignment is assumed from row order, not drawn. (M490F: 1978 - M490F - 490-04-007 - CONNECTOR REAR VIEW.jpg)

**Inserts:** INSERT LEFT: INSERT SEND LEFT → INSERT RETURN LEFT · INSERT RIGHT: INSERT SEND RIGHT → INSERT RETURN RIGHT

| Pin | Signal | Kind | Port | Confidence |
|---|---|---|---|---|
| P1-1 | PGM 1 OUT LEFT | out | PGM 1 OUT LEFT L | medium |
| P1-2 | PGM 1 OUT LEFT | out | PGM 1 OUT LEFT L | medium |
| P1-3 | PGM 1 OUT RIGHT | out | PGM 1 OUT RIGHT R | medium |
| P1-4 | PGM 1 OUT RIGHT | out | PGM 1 OUT RIGHT R | medium |
| P1-5 | PGM 2 OUT LEFT | out | PGM 2 OUT LEFT L | medium |
| P1-6 | PGM 2 OUT LEFT | out | PGM 2 OUT LEFT L | medium |
| P1-7 | PGM 2 OUT RIGHT | out | PGM 2 OUT RIGHT R | medium |
| P1-8 | PGM 2 OUT RIGHT | out | PGM 2 OUT RIGHT R | medium |
| P1-9 | SHIELD | shield | shield | medium |
| P1-10 | N/C | nc |  | medium |
| P1-11 | AUX OUT LEFT | out | AUX OUT LEFT L | medium |
| P1-12 | AUX OUT LEFT | out | AUX OUT LEFT L | medium |
| P1-13 | AUX OUT RIGHT | out | AUX OUT RIGHT R | medium |
| P1-14 | AUX OUT RIGHT | out | AUX OUT RIGHT R | medium |
| P1-15 | CUE OUT LEFT | out | CUE OUT LEFT L | medium |
| P1-16 | CUE OUT LEFT | out | CUE OUT LEFT L | medium |
| P1-17 | CUE OUT RIGHT | out | CUE OUT RIGHT R | medium |
| P1-18 | CUE OUT RIGHT | out | CUE OUT RIGHT R | medium |
| P1-19 | N/C | nc |  | medium |
| P1-20 | N/C | nc |  | medium |
| P1-21 | N/C | nc |  | medium |
| P1-22 | CHASSIS | ground |  | medium |
| P2-1 | INPUT B LEFT | in | INPUT B LEFT L | medium |
| P2-2 | INPUT B RIGHT | in | INPUT B RIGHT R | medium |
| P2-3 | INPUT A LEFT | in | INPUT A LEFT L | medium |
| P2-4 | INPUT A RIGHT | in | INPUT A RIGHT R | medium |
| P2-5 | INSERT SEND LEFT | insert_send | INSERT SEND LEFT L | medium |
| P2-6 | INSERT SEND RIGHT | insert_send | INSERT SEND RIGHT R | medium |
| P2-7 | INSERT RETURN LEFT | insert_return | INSERT RETURN LEFT L | medium |
| P2-8 | INSERT RETURN RIGHT | insert_return | INSERT RETURN RIGHT R | medium |
| P2-9 | SHIELD | shield | shield | medium |
| P2-10 | INPUT A CTL | control_in | INPUT A CTL | medium |
| P2-11 | EXT CUE | control_in | EXT CUE | medium |
| P2-12 | EXT CH OFF | control_in | EXT CH OFF | medium |
| P2-13 | CH A CTL OUT | control_out | CH A CTL OUT | medium |
| P2-14 | N/C | nc |  | medium |
| P2-15 | ON CTL | control_in | ON CTL | medium |
| P2-16 | INTERNALLY CONNECTED | other |  | medium |
| P2-17 | OFF CTL | control_in | OFF CTL | medium |
| P2-18 | OFF TALLY | control_out | OFF TALLY | medium |
| P2-19 | -25 V | power |  | medium |
| P2-20 | 25 V COMMON | ground |  | medium |
| P2-21 | +25 V | power |  | medium |
| P2-22 | CONTROL COMMON | ground |  | medium |
| P2-A | INPUT B LEFT | in | INPUT B LEFT L | medium |
| P2-B | INPUT B RIGHT | in | INPUT B RIGHT R | medium |
| P2-C | INPUT A LEFT | in | INPUT A LEFT L | medium |
| P2-D | INPUT A RIGHT | in | INPUT A RIGHT R | medium |
| P2-E | INSERT SEND LEFT | insert_send | INSERT SEND LEFT L | medium |
| P2-F | INSERT SEND RIGHT | insert_send | INSERT SEND RIGHT R | medium |
| P2-H | INSERT RETURN LEFT | insert_return | INSERT RETURN LEFT L | medium |
| P2-J | INSERT RETURN RIGHT | insert_return | INSERT RETURN RIGHT R | medium |
| P2-K | SHIELD | shield | shield | medium |
| P2-L | INPUT B CTL | control_in | INPUT B CTL | medium |
| P2-M | INPUT CTL COMMON | ground |  | medium |
| P2-N | EXT CH ON | control_in | EXT CH ON | medium |
| P2-P | CH B CTL OUT | control_out | CH B CTL OUT | medium |
| P2-R | TIMER RESET | control_out | TIMER RESET | medium |
| P2-S | ON CTL | control_in | ON CTL | medium |
| P2-T | INTERNALLY CONNECTED | other |  | medium |
| P2-U | OFF CTL | control_in | OFF CTL | medium |
| P2-V | OFF TALLY | control_out | OFF TALLY | medium |
| P2-W | -25 V | power |  | medium |
| P2-X | 25 V COMMON | ground |  | medium |
| P2-Y | +25 V | power |  | medium |
| P2-Z | CONTROL COMMON | ground |  | medium |

**Straps:** JMP.6.7: P2-6 P2-7 · JMP.F.H: P2-F P2-H

## Manuals and documents

_Manuals and manual pages, price lists, RTO-144 connection sheets, brochures, ads and other document scans._

<table>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKeko1di1iQnl6RjQ/view?resourcekey=0-r0PrLH4YXnrM96FyFPWXgw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKeko1di1iQnl6RjQ&resourcekey=0-r0PrLH4YXnrM96FyFPWXgw" width="240" alt="1978 - M490F - 000 - cover.jpg"></a><br><sub>1978|11 · 000 - cover</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKTzJWR1JJVi14R3c/view?resourcekey=0-CTJSefwGJRwiZrsmJ02adg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKTzJWR1JJVi14R3c&resourcekey=0-CTJSefwGJRwiZrsmJ02adg" width="240" alt="1978 - M490F - 001.jpg"></a><br><sub>1978|11 · 001</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKTlNFb1JHZHNtaXc/view?resourcekey=0-R3IXalX9pviSufXZ-CTGwQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKTlNFb1JHZHNtaXc&resourcekey=0-R3IXalX9pviSufXZ-CTGwQ" width="240" alt="1978 - M490F - 002.jpg"></a><br><sub>1978|11 · 002</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKdlJNajgzYVEyakk/view?resourcekey=0-UT0LGKjl-AZjEfDFnnzKUA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKdlJNajgzYVEyakk&resourcekey=0-UT0LGKjl-AZjEfDFnnzKUA" width="240" alt="1978 - M490F - 003.jpg"></a><br><sub>1978|11 · 003</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKQzJFbXM1MDZMaTg/view?resourcekey=0-HeejMCHWRDDa5_NkC_LEbQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKQzJFbXM1MDZMaTg&resourcekey=0-HeejMCHWRDDa5_NkC_LEbQ" width="240" alt="1978 - M490F - 004.jpg"></a><br><sub>1978|11 · 004</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKVzlrX20xc3czR2c/view?resourcekey=0-l6H7-m5FJoxgesErQGxd1Q" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKVzlrX20xc3czR2c&resourcekey=0-l6H7-m5FJoxgesErQGxd1Q" width="240" alt="1978 - M490F - 005.jpg"></a><br><sub>1978|11 · 005</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKcWxXTkwyazBkOVk/view?resourcekey=0-7e_-OIHJPfPebPVPqQ67gw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKcWxXTkwyazBkOVk&resourcekey=0-7e_-OIHJPfPebPVPqQ67gw" width="240" alt="1978 - M490F - 006.jpg"></a><br><sub>1978|11 · 006</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKTjlETnc3UU5fbkE/view?resourcekey=0-l1Aw5yhRsppsR_mnPX2j-Q" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKTjlETnc3UU5fbkE&resourcekey=0-l1Aw5yhRsppsR_mnPX2j-Q" width="240" alt="1978 - M490F - 007.jpg"></a><br><sub>1978|11 · 007</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKTGRCZnE0TGZJY0k/view?resourcekey=0-m2Em9ceqGK-jbKCXqJvucg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKTGRCZnE0TGZJY0k&resourcekey=0-m2Em9ceqGK-jbKCXqJvucg" width="240" alt="1978 - M490F - 008.jpg"></a><br><sub>1978|11 · 008</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKT3lmcEFiRkVNZlE/view?resourcekey=0-8d4V-xs_iCxuE9KaHAfFjg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKT3lmcEFiRkVNZlE&resourcekey=0-8d4V-xs_iCxuE9KaHAfFjg" width="240" alt="1978 - M490F - 009.jpg"></a><br><sub>1978|11 · 009</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKVERWa0Jkako2ZW8/view?resourcekey=0-zObarRJXGF-LVDmN0vuN0A" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKVERWa0Jkako2ZW8&resourcekey=0-zObarRJXGF-LVDmN0vuN0A" width="240" alt="1978 - M490F - 010.jpg"></a><br><sub>1978|11 · 010</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKUld6U2JMZVh5Q1E/view?resourcekey=0-Z43WaDpaQHzIFu410TznzA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKUld6U2JMZVh5Q1E&resourcekey=0-Z43WaDpaQHzIFu410TznzA" width="240" alt="1978 - M490F - 011.jpg"></a><br><sub>1978|11 · 011</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKNWVyTHYwU0hwNkU/view?resourcekey=0-aO7J6UzvAfK2wtxYX6bQ5w" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKNWVyTHYwU0hwNkU&resourcekey=0-aO7J6UzvAfK2wtxYX6bQ5w" width="240" alt="1978 - M490F - 012.jpg"></a><br><sub>1978|11 · 012</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKWkhsZVNEMjJ1UEk/view?resourcekey=0-iwBR4W3GKVgsw_nlSVx6hQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKWkhsZVNEMjJ1UEk&resourcekey=0-iwBR4W3GKVgsw_nlSVx6hQ" width="240" alt="1978 - M490F - 013.jpg"></a><br><sub>1978|11 · 013</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKbEg4OTYycXFtQnc/view?resourcekey=0-gdCIpP_xI2jyJhfMZOIyBQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKbEg4OTYycXFtQnc&resourcekey=0-gdCIpP_xI2jyJhfMZOIyBQ" width="240" alt="1978 - M490F - 014.jpg"></a><br><sub>1978|11 · 014</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKOWNxcGRtUjl5SVE/view?resourcekey=0-1lnSqpmKSW3vLcpKJUacVw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKOWNxcGRtUjl5SVE&resourcekey=0-1lnSqpmKSW3vLcpKJUacVw" width="240" alt="1978 - M490F - 015.jpg"></a><br><sub>1978|11 · 015</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKb3RzNG1VVkRvRTg/view?resourcekey=0-A4De-FoCIBKp55wMHJzYLg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKb3RzNG1VVkRvRTg&resourcekey=0-A4De-FoCIBKp55wMHJzYLg" width="240" alt="1978 - M490F - 017 - 7-112.jpg"></a><br><sub>1978|11 · 017 - 7-112</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKODRWOFNPdlItbDQ/view?resourcekey=0-hOFQ9-rhGjD001YfjjBYUA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKODRWOFNPdlItbDQ&resourcekey=0-hOFQ9-rhGjD001YfjjBYUA" width="240" alt="1978 - M490F - 018 - 7-112.jpg"></a><br><sub>1978|11 · 018 - 7-112</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKQkR3ampGOGtKLVE/view?resourcekey=0-lM-ZBFjqe8MAW0paNj_Bwg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKQkR3ampGOGtKLVE&resourcekey=0-lM-ZBFjqe8MAW0paNj_Bwg" width="240" alt="1978 - M490F - 019 - 7-112.jpg"></a><br><sub>1978|11 · 019 - 7-112</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKZUFWcDQwVVhUSmc/view?resourcekey=0-fS5HsYbCBKt7aBhm0u4V5w" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKZUFWcDQwVVhUSmc&resourcekey=0-fS5HsYbCBKt7aBhm0u4V5w" width="240" alt="1978 - M490F - 023.jpg"></a><br><sub>1978|11 · 023</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKdGJmM19RaURlaEE/view?resourcekey=0-87MBO0zkphtjLhwLFmQvPg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKdGJmM19RaURlaEE&resourcekey=0-87MBO0zkphtjLhwLFmQvPg" width="240" alt="1978 - M490F - P001 - Title Page.jpg"></a><br><sub>1978|11 · P001 - Title Page</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKeVJTTU1RYnZGaG8/view?resourcekey=0-ujOkWt5u7upG2wgLzRfP0A" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKeVJTTU1RYnZGaG8&resourcekey=0-ujOkWt5u7upG2wgLzRfP0A" width="240" alt="1978 - M490F - P002.jpg"></a><br><sub>1978|11 · P002</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKNTBBWUp2cnd0OUU/view?resourcekey=0-xzoZE2cc7h5rHLmZfO4TrA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKNTBBWUp2cnd0OUU&resourcekey=0-xzoZE2cc7h5rHLmZfO4TrA" width="240" alt="1978 - M490F - P003 - 1-1.jpg"></a><br><sub>1978|11 · P003 - 1-1</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKaW1TbHBsRVRxdEk/view?resourcekey=0-lG2BIjlTVzC0NMCSdOP0oQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKaW1TbHBsRVRxdEk&resourcekey=0-lG2BIjlTVzC0NMCSdOP0oQ" width="240" alt="1978 - M490F - P004 - 1-2.jpg"></a><br><sub>1978|11 · P004 - 1-2</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKNjE4TmJmb0g4dGM/view?resourcekey=0-5eOL_px7JD3jdQ5XYWcxVw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKNjE4TmJmb0g4dGM&resourcekey=0-5eOL_px7JD3jdQ5XYWcxVw" width="240" alt="1978 - M490F - P005 - 2-1.jpg"></a><br><sub>1978|11 · P005 - 2-1</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKcHpvTmZhT3NnZUE/view?resourcekey=0-xyVU2mylLtRl5JvL0GR9kw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKcHpvTmZhT3NnZUE&resourcekey=0-xyVU2mylLtRl5JvL0GR9kw" width="240" alt="1978 - M490F - P006 - 2-2.jpg"></a><br><sub>1978|11 · P006 - 2-2</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKaXRWZE13UThLSGs/view?resourcekey=0-1jb27f4MIuAHVgLgQ82q9Q" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKaXRWZE13UThLSGs&resourcekey=0-1jb27f4MIuAHVgLgQ82q9Q" width="240" alt="1978 - M490F - P007 - 2-3.jpg"></a><br><sub>1978|11 · P007 - 2-3</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKSWNZSVpuN25raDA/view?resourcekey=0-9YcF-yAHHMElG5Hkfcu1lg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKSWNZSVpuN25raDA&resourcekey=0-9YcF-yAHHMElG5Hkfcu1lg" width="240" alt="1978 - M490F - P008 - 2-4.jpg"></a><br><sub>1978|11 · P008 - 2-4</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKWmc3TDBpX2dfSHc/view?resourcekey=0-T_qZ2oiJqdEJ5QUhecxb-A" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKWmc3TDBpX2dfSHc&resourcekey=0-T_qZ2oiJqdEJ5QUhecxb-A" width="240" alt="1978 - M490F - P009 - 2-5.jpg"></a><br><sub>1978|11 · P009 - 2-5</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKbkR6dFlEVkQyQ1k/view?resourcekey=0-njRrg0M0Km5kScnxBlcnqg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKbkR6dFlEVkQyQ1k&resourcekey=0-njRrg0M0Km5kScnxBlcnqg" width="240" alt="1978 - M490F - P010 - 2-6.jpg"></a><br><sub>1978|11 · P010 - 2-6</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKaWNmZk9nRXVqVVE/view?resourcekey=0-4UMnZUYIdu9e1ZpxS6w9xg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKaWNmZk9nRXVqVVE&resourcekey=0-4UMnZUYIdu9e1ZpxS6w9xg" width="240" alt="1978 - M490F - P013 - 3-1.jpg"></a><br><sub>1978|11 · P013 - 3-1</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKYkFpSjNPc0p5elU/view?resourcekey=0-AxRa8JnGGXOf04CvOKOtFQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKYkFpSjNPc0p5elU&resourcekey=0-AxRa8JnGGXOf04CvOKOtFQ" width="240" alt="1978 - M490F - P014 - 3-2.jpg"></a><br><sub>1978|11 · P014 - 3-2</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKSGRyYmF4RWZpbzQ/view?resourcekey=0-gpGuQoBslBTJXwhTsWI8Hw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKSGRyYmF4RWZpbzQ&resourcekey=0-gpGuQoBslBTJXwhTsWI8Hw" width="240" alt="1978 - M490F - P015 - 3-3.jpg"></a><br><sub>1978|11 · P015 - 3-3</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKYWVwTENqQXpJRGM/view?resourcekey=0-RyfLTxKhuAFYm-bdnZOsWQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKYWVwTENqQXpJRGM&resourcekey=0-RyfLTxKhuAFYm-bdnZOsWQ" width="240" alt="1978 - M490F - P016 - 3-4.jpg"></a><br><sub>1978|11 · P016 - 3-4</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKeGp5aFVkSEdvN2s/view?resourcekey=0-bNT0u6LZ0PX5vVsduIggxw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKeGp5aFVkSEdvN2s&resourcekey=0-bNT0u6LZ0PX5vVsduIggxw" width="240" alt="1978 - M490F - P017 - 3-5.jpg"></a><br><sub>1978|11 · P017 - 3-5</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKNEczd3NLamtabVE/view?resourcekey=0-nLVCv4wKVbqIADoh0qCr-A" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKNEczd3NLamtabVE&resourcekey=0-nLVCv4wKVbqIADoh0qCr-A" width="240" alt="1978 - M490F - P018 - 3-6.jpg"></a><br><sub>1978|11 · P018 - 3-6</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKaU5FdmpXb0wxc00/view?resourcekey=0-q7x4D7TmpSvwq2c2mggBRw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKaU5FdmpXb0wxc00&resourcekey=0-q7x4D7TmpSvwq2c2mggBRw" width="240" alt="1978 - M490F - P019 - 3-7.jpg"></a><br><sub>1978|11 · P019 - 3-7</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKNG0xcjI5MGF4WGs/view?resourcekey=0-Bg-1vZbFG-RPhdTlTVJHsg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKNG0xcjI5MGF4WGs&resourcekey=0-Bg-1vZbFG-RPhdTlTVJHsg" width="240" alt="1978 - M490F - P020 - 3-8.jpg"></a><br><sub>1978|11 · P020 - 3-8</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKTUt5YWI3ek8tTGM/view?resourcekey=0-HvY41BSm2U3vV5Qv2tnChw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKTUt5YWI3ek8tTGM&resourcekey=0-HvY41BSm2U3vV5Qv2tnChw" width="240" alt="1978 - M490F - P021 - 3-9.jpg"></a><br><sub>1978|11 · P021 - 3-9</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKS1A3aEVEVTBKUkU/view?resourcekey=0-GpkXQyB13NNoAlqldjujrA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKS1A3aEVEVTBKUkU&resourcekey=0-GpkXQyB13NNoAlqldjujrA" width="240" alt="1978 - M490F - P022 - CD4016.jpg"></a><br><sub>1978|11 · P022 - CD4016</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKQk5QSG5mUEpGQ0U/view?resourcekey=0-E4TYnQvBNcJwHfBoELwUYg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKQk5QSG5mUEpGQ0U&resourcekey=0-E4TYnQvBNcJwHfBoELwUYg" width="240" alt="1978 - M490F - P023 - 74C76.jpg"></a><br><sub>1978|11 · P023 - 74C76</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKcjBTRVM0VEZhZDg/view?resourcekey=0-fbeKKVPoNAI4cREpm6w1Dw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKcjBTRVM0VEZhZDg&resourcekey=0-fbeKKVPoNAI4cREpm6w1Dw" width="240" alt="1978 - M490F - P024 - 74C221.jpg"></a><br><sub>1978|11 · P024 - 74C221</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKNFVLUjdSNHVZOVE/view?resourcekey=0-nqAEwafFFxyn9Yd0jf75eA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKNFVLUjdSNHVZOVE&resourcekey=0-nqAEwafFFxyn9Yd0jf75eA" width="240" alt="1978 - M490F - P026 - 7-112 - 1-1.jpg"></a><br><sub>1978|11 · P026 - 7-112 - 1-1</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKamRJNDBkWnZLbWc/view?resourcekey=0-IOetA_AX4gyuiQTfZ_r4OQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKamRJNDBkWnZLbWc&resourcekey=0-IOetA_AX4gyuiQTfZ_r4OQ" width="240" alt="1978 - M490F - P027 - 7-112 - 1-2.jpg"></a><br><sub>1978|11 · P027 - 7-112 - 1-2</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKbUFHamRGcjN0Z1E/view?resourcekey=0-wqisGtHgV7khoK4JyGMhDw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKbUFHamRGcjN0Z1E&resourcekey=0-wqisGtHgV7khoK4JyGMhDw" width="240" alt="1978 - M490F - P028 - 7-112 - 1-3.jpg"></a><br><sub>1978|11 · P028 - 7-112 - 1-3</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKV0xhNl81RmUxRmc/view?resourcekey=0-Ja1ENk6tl0xpUwOcJo12PA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKV0xhNl81RmUxRmc&resourcekey=0-Ja1ENk6tl0xpUwOcJo12PA" width="240" alt="1978 - M490F - P029 - 7-112 - 1-4.jpg"></a><br><sub>1978|11 · P029 - 7-112 - 1-4</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKS1Z2QUd0Qk1KaWM/view?resourcekey=0-wD12l1snyjMga5rVcsHMkQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKS1Z2QUd0Qk1KaWM&resourcekey=0-wD12l1snyjMga5rVcsHMkQ" width="240" alt="1978 - M490F - Stereo Input Module.pdf"></a><br><sub>1978|11 · Stereo Input Module</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKTlIxS283dzlackU/view?resourcekey=0-AEkvA9xa-2NLEQYgVin8qg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKTlIxS283dzlackU&resourcekey=0-AEkvA9xa-2NLEQYgVin8qg" width="240" alt="1983 - M490F - 016 - 7-112.jpg"></a><br><sub>1983|16 · 016 - 7-112</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKMUVxQ1QxblJhZnc/view?resourcekey=0-nr9yBRLWmbfyHSGgaTbBig" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKMUVxQ1QxblJhZnc&resourcekey=0-nr9yBRLWmbfyHSGgaTbBig" width="240" alt="1983 - M490F - P025 - 7-112.jpg"></a><br><sub>1983|16 · P025 - 7-112</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKOHhQU1pKeWloQ3M/view?resourcekey=0-702VO2S7YHtgs5hAWOkH8g" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKOHhQU1pKeWloQ3M&resourcekey=0-702VO2S7YHtgs5hAWOkH8g" width="240" alt="1983 - M490F - Stereo Input Module.pdf"></a><br><sub>1983|16 · Stereo Input Module</sub></td></tr>
</table>

## KiCad

_KiCad: a schematic (`.kicad_sch`) traced from each electrical drawing, the module symbol (`.kicad_sym`) and its PCB projects. Traced schematics are the line work only: redraw with symbols over them._

- [1978 - M490F - 490-01-006 - ISTART TIMER RESET OFF TALLY OFFISTOP.kicad_sch](KICAD/1978%20-%20M490F%20-%20490-01-006%20-%20ISTART%20TIMER%20RESET%20OFF%20TALLY%20OFFISTOP.kicad_sch)
- [1978 - M490F - 490-01-006 - MACHINE CONTROLS REVISED.kicad_sch](KICAD/1978%20-%20M490F%20-%20490-01-006%20-%20MACHINE%20CONTROLS%20REVISED.kicad_sch)
- [1978 - M490F - 490-02-007 - RIIE IOOK.kicad_sch](KICAD/1978%20-%20M490F%20-%20490-02-007%20-%20RIIE%20IOOK.kicad_sch)
- [1978 - M490F - 490-02-007 - STEREO INPUT MODULE.kicad_sch](KICAD/1978%20-%20M490F%20-%20490-02-007%20-%20STEREO%20INPUT%20MODULE.kicad_sch)
- [1978 - M490F - 7-112-02-001 - ALL CAPACITORS.kicad_sch](KICAD/1978%20-%20M490F%20-%207-112-02-001%20-%20ALL%20CAPACITORS.kicad_sch)
- [1978 - M490F - 7-112-02-001 - CHANNEL AMPLIFIER SCHEMATIC ISSUL.kicad_sch](KICAD/1978%20-%20M490F%20-%207-112-02-001%20-%20CHANNEL%20AMPLIFIER%20SCHEMATIC%20ISSUL.kicad_sch)
- [1978 - M490F - Stereo Input Module p29.kicad_sch](KICAD/1978%20-%20M490F%20-%20Stereo%20Input%20Module%20p29.kicad_sch)
- [1978 - M490F - Stereo Input Module p30.kicad_sch](KICAD/1978%20-%20M490F%20-%20Stereo%20Input%20Module%20p30.kicad_sch)
- [1978 - M490F - Stereo Input Module p33.kicad_sch](KICAD/1978%20-%20M490F%20-%20Stereo%20Input%20Module%20p33.kicad_sch)
- [1983 - M490F - Stereo Input Module p29.kicad_sch](KICAD/1983%20-%20M490F%20-%20Stereo%20Input%20Module%20p29.kicad_sch)
- [1983 - M490F - Stereo Input Module p33.kicad_sch](KICAD/1983%20-%20M490F%20-%20Stereo%20Input%20Module%20p33.kicad_sch)
- [19xx - M490F - INTEGRATED CIRCUIT DATA 74C76 DUAL J-K FLIP-FLOP WITH CLEAR AND PRESET.kicad_sch](KICAD/19xx%20-%20M490F%20-%20INTEGRATED%20CIRCUIT%20DATA%2074C76%20DUAL%20J-K%20FLIP-FLOP%20WITH%20CLEAR%20AND%20PRESET.kicad_sch)
- [M490F.kicad_sym](KICAD/M490F.kicad_sym)

---
Archive: Anthony Peter Kuzub · [WBSps.ca](https://WBSps.ca) · [WBSps.Kuzub.com](https://WBSps.Kuzub.com)
