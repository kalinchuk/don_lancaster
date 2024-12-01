# TV Typewriter

Don Lancaster's TV Typewriter was featured in the [September 1973 issue of the Radio Electronics magazine](Radio-Electronics-1973-09.pdf). The article contained the first part of the TV Typewriter construction manual. The remaining parts were released in the [full version of the construction manual](TVTypewriterConstructionManual.pdf)

The TV Typewriter was introduced in the YouTube video titled [Building Don Lancaster's TV Typewriter](https://youtu.be/Z4RsOHaQ3xM) and built and tested in subsequent videos.

[Part 1 (Intro)](https://youtu.be/Z4RsOHaQ3xM)

[Part 2 (Mainframe)](https://www.youtube.com/watch?v=5wwCebJK5xs)

## PCB

The artwork in the construction manual was used to create PCBs of the TV Typewriter which contains 4 boards - 1 mainframe PCB, 1 cursor PCB, 1 timing PCB and 1 memory PCB (with the ability to expand to 2).

<img width="704" alt="TV Typewriter Mainframe PCB Artwork" src="https://github.com/user-attachments/assets/b9a12074-099b-4dbf-b769-d500d17c3cf2">


The PCB set is available for sale at [https://www.kalinchuk.com/product-page/don-lancaster-s-tv-typewriter-pcb-set](https://www.kalinchuk.com/product-page/don-lancaster-s-tv-typewriter-pcb-set). If you would like to fabricate the PCBs yourself, the Gerber files will be made available soon.

<img width="704" alt="TV Typewriter PCBs" src="https://github.com/user-attachments/assets/17f919be-95dd-4b9a-a2ed-570dae4ce916">

## Parts

Refer to the construction manual for the parts required to build the TV Typewriter. Below, you will find the specific or hard-to-find parts for each PCB and the source I used for each part.

### Mainframe

| Part       | Spec        | Source                   |
| ---------- | ----------- | ------------------------ |
| C6         | 3-30 pF trimmer    | [Electro Motive Mfg 83201B12](https://www.ebay.com/itm/234887932037) |
| C10        | N/A         | [300 ohm twin lead wire](https://www.ebay.com/itm/122434170705) cut at 8" from PCB and overlap the two by 2" by taping it over each other |
| F1         | Fuse holder         | [MPD BK-6004](https://www.digikey.com/en/products/detail/mpd-memory-protection-devices/BK-6004/2330523) |
| J1-J2      | Binding post        | [Pomona Electronics 3760-4](https://www.digikey.com/en/products/detail/pomona-electronics/3760-4/736553?so=88660697) |
| Q1         | 2N918               | [eBay](https://www.ebay.com/itm/116185007333) |
| IC1 Heat sink | 17.90°C/W | [Boyd Laconia 6025DG](https://www.digikey.com/en/products/detail/boyd-laconia-llc/6025DG/4974546) |
| S1-S4, S7-S8 | SWITCH ROCKER DPDT 5A 120V | [C&K 7201J1ZQE2](https://www.digikey.com/en/products/detail/c-k/7201J1ZQE2/66994) |
| S5-S6      | SWITCH ROCKER DPDT Momentary | [C&K 7208J1ZQE2](https://www.onlinecomponents.com/en/productdetail/littelfuse-c-k/7208j1zqe2-11106482.html) |
| S01-S06    | Molex 09-52-3103 | [Radwell](https://www.radwell.com/Buy/ASEA%20BROWN%20BOVERI/BALDOR%20RELIANCE/TB0057A00?parentitemid=3649397) |
| T1         | Signal 24-1A     | eBay (Signal Transformer 24-1A) |

#### PCB

<img width="704" alt="Mainframe PCB" src="https://github.com/user-attachments/assets/9d54dddc-cf2b-4144-98c9-25f026608931">

#### Power Transformer Connection

<img width="500" alt="Power Transformer Connection" src="https://github.com/user-attachments/assets/2c6cc732-dc15-414b-bba9-86786a139f2d">

#### Coil

<img width="500" alt="Coil" src="https://github.com/user-attachments/assets/aed0b7fe-f4b7-419b-bfd4-ecc7c4cb32da">

#### Gimmick Attenuator

<img width="500" alt="Gimmick attenuator" src="https://github.com/user-attachments/assets/b59c3fc3-8666-46e1-af4a-9982d15c3268">


### Memory

The hardest to find components on the Memory board are the Signetics 2524V shift registers. The rest of the components are fairly easy to find. eBay is a good source for most of the components.

| Part       | Spec        | Source                   |
| ---------- | ----------- | ------------------------ |
| IC1-IC6              | 2524 MOS 512-bit recirculating shift register (Signetics)   | [kalinchuk.com (while supplies last)](https://www.kalinchuk.com/product-page/signetics-2524v-shift-register-for-tv-typewriter) or eBay if they show up by chance |
| IC8                  | 2518 MOS 32-bit recirculating shift register (Signetics)    | eBay, i.e. [this listing](https://www.ebay.com/itm/254053777558) |
| IC9                  | 2513 character generator          | [eBay](https://www.ebay.com/itm/335361527128) |

#### PCB

Coming soon

### Cursor

Coming soon

### Timing

Most of the components on the Timing board are easy to find. The hardest part to find is the 4.261 MHz crystal oscillator.

| Part       | Spec        | Source                   |
| ---------- | ----------- | ------------------------ |
| IC1                  | Motorola MC4024          | [eBay](https://www.ebay.com/itm/335377355646) |
| IC2-IC3, IC5         | 8288 divide by twelve    | [eBay](https://www.ebay.com/itm/335642427110) |
| P1-P60     | Molex 26-60-2101 | [DigiKey](https://www.digikey.com/en/products/detail/molex/0026602101/3159571) |
| S01-S06    | Molex 09-52-3103 | [Radwell](https://www.radwell.com/Buy/ASEA%20BROWN%20BOVERI/BALDOR%20RELIANCE/TB0057A00?parentitemid=3649397) |
| XTAL 1     | 4,561.920 KHz    | I used [4.5 MHz](https://www.ebay.com/itm/125806912675) for testing but a more precise frequency is required. You can try connecting the crystal and a trimmer capacitor in parallel to increase the frequency slightly (such as the 3-30 pF used on the Mainframe board). I will update this once I find a more suitable oscillator. |

#### PCB

Coming soon

## Final Product

Coming soon

## Issues

The first batch of PCBs had the following issues that needed correction:

1) The 5v voltage regulator footprint on the Mainframe was slightly too small. Correction: Drill out with 1/16" drill bit.
2) The RF tuner (trimmer capacitor) footprint on the Mainframe was too small. Correction: Use a drill to enlarge it slightly.
3) The coil footprint on the Mainframe was slightly too small. Correction: Use a drill bit large enough for the coil to enlarge it.
4) The power switch footprint on the Mainframe might be too small if using lower guage wire. Correction: Use 1/16" drill bit to enlarge it.
5) IC7 pin 12 of the Memory board has a short with a passing trace. Correction: Remove the short using a small knife or other method.
