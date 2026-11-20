Fork of the original project at https://github.com/AndBu/YAIFM/blob/main/README.md

Changes:

This project uses all the 3D models except:
a) The switch holder
b) Lid (PCB)
c) Motor holder for the switch holder
d) PCB holder

I did not use the switch at all, but instead altered the code to learn the top and bottom limits based on that blind and the encoder counts and flash them to the microcontroller. It seems repeatable up and down for now.

A different (similar type, but specifics matter) N20 motor was used: a brushed motor with a metal gearbox and encoder. In this case, it was: https://www.amazon.co.uk/dp/B0F8N6THR5?ref=ppx_yo2ov_dt_b_fed_asin_title&th=1

<img width="1059" height="1649" alt="image" src="https://github.com/user-attachments/assets/a5e98525-e5e9-42dc-be80-347920c015a2" />

Electronics are a work in progress, and no enclosure has been built yet.

<img width="1200" height="1600" alt="WhatsApp Image 2026-11-20 at 11 19 39" src="https://github.com/user-attachments/assets/58942a6b-7199-4525-b1f9-6348894760e9" />
<img width="1200" height="1600" alt="WhatsApp Image 2026-11-20 at 11 21 23" src="https://github.com/user-attachments/assets/f9ee6ff0-0f27-4680-bdaa-20cb5be54bef" />

The motor is a little noisy, but lowering the speed makes it okay. This is not perfect, but I did not want to use a switch—it was too clunky for me.

What is great is the neat mechanical integration into the blind roller. Most projects use external motors. I found that the small steppers used in this project https://www.thingiverse.com/thing:4889111/files to be too weak and not very quiet. Also, these steppers can slip when unpowered. The brushed DC motor with gearbox doesn't slip under power-down, which means the blind stays put. Home Assistant Cover Card is great, as it includes sensors for how far the blind has travelled, etc.

<img width="736" height="408" alt="image" src="https://github.com/user-attachments/assets/ad331743-ee63-4953-8550-1e5d3deca720" />

My YAML is included in the files and implements the code for learning limits without a switch.

# Disclaimer

The information contained in this repository is for general information purposes only. The information is provided by the contributors, who make no representations or warranties of any kind, express or implied, about the completeness, accuracy, reliability, suitability or availability for any purpose, including but not limited to information, products, services, or related graphics. Any reliance you place on such information is therefore strictly at your own risk.

Also, the contributors are not affiliated with any of the shops or brands linked and discussed here. While they might have successfully tested the components in their own designs, they do not recommend any specific component from any manufacturer or shop in particular. Information about shops or products or manufacturers, including but not limited to links, is for illustrative purposes only. Manufacturers or distributors of electrical components are known to change a product's specification without notice.
