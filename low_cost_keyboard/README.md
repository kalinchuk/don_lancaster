# Low Cost Keyboard

The "low cost keyboard" by Don Lancaster was featured in the [February 1973 issue of the Radio Electronics magazine](low_cost_keyboard_2_73.pdf). The article starts on page 54.

This keyboard was built in the YouTube video titled [Building Don Lancaster's ASCII Keyboard](https://youtu.be/akgyQJSSxYs).

## PCB

The artwork in the article was used to create PCBs of the "low cost keyboard".

<img width="704" alt="Low Cost Keyboard Artwork" src="https://github.com/user-attachments/assets/ba0e399e-865e-4879-a29e-6433dd137040">

I made two different versions of the PCB - one original version and the other modified for modern key switches. The original PCBs are available for at [https://www.kalinchuk.com/product-page/don-lancaster-s-low-cost-keyboard-pcb-original](https://www.kalinchuk.com/product-page/don-lancaster-s-low-cost-keyboard-pcb-original). The modern variant PCBs are available at [https://www.kalinchuk.com/product-page/don-lancaster-s-low-cost-keyboard-pcb-modern](https://www.kalinchuk.com/product-page/don-lancaster-s-low-cost-keyboard-pcb-modern). You can also use the [Original Gerber](original_gerber.zip) or [Modern Gerber](modern_gerber.zip) files to fabricate the PCBs yourself.

## Parts

Refer to the article for the parts required to build the original keyboard. I decided to use the modern variant of the PCB so that I could use MX key switches.

If you're building the modern variant, the keyboard only needs key switches, key caps and wire for jumpers. In my build, I used [key stabilizers](https://www.amazon.com/gp/product/B096JWNKVG) for the space bar. The key switches are standard MX switches and the key caps are standard caps. I used a [set of standard key caps](https://www.amazon.com/gp/product/B0BLMJQRSG) for my build.

Another builder used [a different set of keycaps](https://www.amazon.com/dp/B0BK3HK7SR), again available from Amazon.

One additional (and optional) part is the Amphenol 143-022-01 connector. You can use this connector or you can solder wires directly to the PCB when connecting to an ASCII encoder.

## Final Product

Below, you will find the final, assembled PCB. The only thing left to do is to customize the key caps.

<img width="704" alt="Low Cost Keyboard Artwork" src="https://github.com/user-attachments/assets/d926b169-8336-40e7-9e40-23ed25c599d3">

If you used the second set of keycaps, you can print [the BMP file](keys.bmp), making sure that each surrounding square border is 0.5" on each side. The [P-touch key label file](keys.lbx) is also provided.

![second keyboard](keyboard2.png)

## Bugs

The original artwork contains a bug in the jumper wires section which makes the "@" and ":" keys behave incorrectly. This can be fixed by swapping the jumper wires 25 & 26 (from the right). This issue has been fixed in the updated Gerbers.

<img width="400" alt="Jumper wires bug" src="https://github.com/user-attachments/assets/1dc1808b-464e-4924-ac58-e38e4389967f"/>
