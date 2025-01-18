# TV Typewriter

Don Lancaster's TV Typewriter was featured in the [September 1973 issue of the Radio Electronics magazine](Radio-Electronics-1973-09.pdf). The article contained the first part of the TV Typewriter construction manual. The remaining parts were released in the [full version of the construction manual](TVTypewriterConstructionManual.pdf)

The TV Typewriter was introduced in the YouTube video titled [Building Don Lancaster's TV Typewriter](https://youtu.be/Z4RsOHaQ3xM) and built and tested in subsequent videos.

[Part 1 (Intro)](https://youtu.be/Z4RsOHaQ3xM)

[Part 2 (Mainframe)](https://www.youtube.com/watch?v=5wwCebJK5xs)

[Part 3 (Timing)](https://www.youtube.com/watch?v=ewfh5tOWrp8)

[Part 4 (Memory)](https://www.youtube.com/watch?v=_3tp-KLXC_w)

[Part 5 (Cursor)](https://www.youtube.com/watch?v=rcFiic5D9TA)

## PCB

The artwork in the construction manual was used to create PCBs of the TV Typewriter which contains 4 boards - 1 mainframe PCB, 1 cursor PCB, 1 timing PCB and 1 memory PCB (with the ability to expand to 2).

<img width="704" alt="TV Typewriter Mainframe PCB Artwork" src="https://github.com/user-attachments/assets/b9a12074-099b-4dbf-b769-d500d17c3cf2">


The PCB set is available for sale at [https://www.kalinchuk.com/product-page/don-lancaster-s-tv-typewriter-pcb-set](https://www.kalinchuk.com/product-page/don-lancaster-s-tv-typewriter-pcb-set). If you would like to fabricate the PCBs yourself, the Gerber files will be made available soon.

<img width="704" alt="TV Typewriter PCBs" src="https://github.com/user-attachments/assets/17f919be-95dd-4b9a-a2ed-570dae4ce916">

## Parts

Refer to the construction manual for the parts required to build the TV Typewriter. Most 7400 ICs can be substituted with a 5400 IC. Below, you will find the specific or hard-to-find parts for each PCB and the source I used for each part.

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

<img width="704" alt="Memory PCB" src="https://github.com/user-attachments/assets/1ca245b3-6c37-4605-b74e-9dacf30279a2">

### Cursor

All of the components on the Cursor board are fairly easy to find. If you can't find a component on sites like DigiKey or Mouser, you can still find them on eBay.

#### PCB

<img width="704" alt="Cursor PCB" src="https://github.com/user-attachments/assets/07df1832-1d08-49b2-bbf1-108ad6f4ae31">

### Timing

Most of the components on the Timing board are easy to find. The hardest part to find is the 4.261 MHz crystal oscillator.

| Part       | Spec        | Source                   |
| ---------- | ----------- | ------------------------ |
| IC1                  | Motorola MC4024          | [eBay](https://www.ebay.com/itm/335377355646) |
| IC2-IC3, IC5         | 8288 divide by twelve    | [eBay](https://www.ebay.com/itm/335642427110) |
| P1-P60     | Molex 26-60-2101 | [DigiKey](https://www.digikey.com/en/products/detail/molex/0026602101/3159571) |
| S01-S06    | Molex 09-52-3103 | [Radwell](https://www.radwell.com/Buy/ASEA%20BROWN%20BOVERI/BALDOR%20RELIANCE/TB0057A00?parentitemid=3649397) |
| XTAL 1     | 4,561.920 KHz    | I used [4.5 MHz](https://www.ebay.com/itm/125806912675) for testing but a more precise frequency is required. You can try connecting the crystal and a trimmer capacitor in parallel to increase the frequency slightly (such as the 3-30 pF used on the Mainframe board). I will update this once I find a more suitable oscillator. For additional alternatives, see the "XTAL Tuning & Alternatives" section below. |

#### PCB

<img width="704" alt="Timing PCB" src="https://github.com/user-attachments/assets/08995b5f-6f7b-4f1f-a2c5-ac3835a9ebe4">

#### XTAL Tuning & Alternatives

If using a crystal that is not an exact 4.561920 MHz, a trimmer capacitor can be applied to tune the frequency slightly. Keep in mind that a trimmer can only alter the frequency by a few kilohertz but it could be a difference between working and not working.

In this example, I have a 3-30pF trimmer connected in parallel while testing:

<img width="500" alt="Tuning Crystal" src="https://github.com/user-attachments/assets/c82647e3-a381-4a81-831c-c44361a8d76c">

An alternative approach is to use a programmable oscillator that is installed on a daughter board and connected to the Timing board that way. This will generate a more precise frequency but requires a breakout board. I used [EPSON SG-8002CA-PTB](https://www.digikey.com/en/products/detail/epson/SG-8002CA-PTB/275195) programmable oscillator from DigiKey. When ordering from DigiKey, specify in the notes the frequency - 4.561920 MHz. Build a small breakout board using the following circuit:

<img width="500" alt="XTAL Breakout Circuit" src="https://github.com/user-attachments/assets/81e4be9c-bf41-46ff-ab87-d7b351447743" />

The breakout board will look something similar to this:

<img width="500" alt="XTAL Breakout Board" src="https://github.com/user-attachments/assets/d6b1409d-a32e-4923-bfb2-c42cbb934aeb" />

The +5v line connects to a nearby jumper wire which is +5v. The GND connects to the XTAL's 3rd pin (used as shield from stray capacitances and connects to GND). The output pin connects to pin 3 of IC1 of the Timing board.

## Final Product

Coming soon

## Bugs I Encountered

While building the TV Typewriter, I encountered some bugs that needed fixing.

1) The keyboard "@" key produced an "8" on the screen (and ":" produced "B").

   This turned out to be a bug on the original artwork of the "low cost keyboard" PCB. See [this](https://github.com/kalinchuk/don_lancaster/tree/main/low_cost_keyboard#bugs) for more information.

2) Bad video output. The video output on the monitor made all the characters smear into each other.

   My monitor was faulty. Switching to a good TV (that can be adjusted) produced much crispier characters. I eventually fixed the issue with my monitor which turned out to be a bad contrast knob.

3) Pressing "T" produced "D" (and other mismatched characters).

   The trace between the bottom connector and the top connector of bus pin 4 was broken on the Memory board which prevented that KBD signal from reaching the Memory board. This was probably because of all the swapping of boards while debugging. I fixed this by soldering a wire from the bottom connector to the top connector of the Memory board.

4) The middle section of the screen always produced "@"s in the same location.

   I had two faulty 2524V shift registers that needed replacement.

5) Forward cursor was not operating properly - after character input, the cursor would sometimes stay in the same place, move forward or even move backward.

   The only difference between the "move forward" circuit and the "move backward" circuit is the addition of C4 of the Cursor board when "move forward" is selected. This capacitor extends the timing a bit and having it off, even by a little, affects the operation of the cursor. After experimenting with that capacitor by trying different values, I found that my capacitor had drifted by over 1,100 pF and needed adjustment.

6) The 12V zener diode on the Mainframe board got very hot.

   The 12V circuit may be pulling too much current (maybe the KBD?) and heating up the zener diode. I replaced the 1W diode with a 3W one (that's all I had but 2W would probably be fine too).

## Issues

The first batch of PCBs had the following issues that needed correction:

1) The 5v voltage regulator footprint on the Mainframe was slightly too small. Correction: Drill out with 1/16" drill bit.
2) The RF tuner (trimmer capacitor) footprint on the Mainframe was too small. Correction: Use a drill to enlarge it slightly.
3) The coil footprint on the Mainframe was slightly too small. Correction: Use a drill bit large enough for the coil to enlarge it.
4) The power switch footprint on the Mainframe might be too small if using lower guage wire. Correction: Use 1/16" drill bit to enlarge it.
5) IC7 pin 12 of the Memory board has a short with a passing trace. Correction: Remove the short using a small knife or other method.
