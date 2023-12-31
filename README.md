# Frandestein_keyboard
_Everything about my (first?) handwired custom split keyboard._

<img src="/images/01_top.jpg">

## How it started
Before making this, I was using a [Lily58L](https://www.reddit.com/r/MechanicalKeyboards/comments/n2makg/probably_its_not_the_prettiest_but_im_so_proud_of/) (mainly from Keycapsss.com), then a [CRKBD](https://www.reddit.com/r/MechanicalKeyboards/comments/sgetwt/i_see_a_keyboard_and_i_want_it_painted_black/) (again, mainly from Keycapsss.com). After using both of them (especially the Lily), I felt like I needed a more compact and minimalistic keyboard, so I ended up designing one by myself. I called it Frandestein because that's one of my other nicknames, but also because it was created taking inspiration from other keyboards and built with parts taken from other electronic accessories, so it reminded me of Frankenstein.

## Sources of inspire
For the layout, I took inspiration from the [CRKBD](https://github.com/foostan/crkbd) and the [Boardsource's Microdox](https://boardsource.xyz/store/5f2e7e4a2902de7151494f92).

For the designing and building processes, these videos were really helpful:
* [How to Design Mechanical Keyboard Plates and Cases](https://youtu.be/7azQkSu0m_U) by Joe Scotto
* [How to Design a Custom Mechanical Keyboard](https://youtu.be/iv__343ZwE0) by Mad Mod Labs
* [How to Build a Handwired Keyboard](https://youtu.be/hjml-K-pV4E) by Joe Scotto
* [Building Handwired Keyboards with Choc Switches](https://youtu.be/Qkx9M-AzznE) by Joe Scotto

## Designing process
I started with editing a _.json_ file of the CRKBD on [KLE](http://www.keyboard-layout-editor.com/) following the first two videos mentioned above to get the final layout I wanted (sorry, I forgot to save the final _.json_ file...). Then I imported it on kbplate.ai03.com, setting unit width and height to 18 and 17mm. Finally, I downloaded the _.dxf_ file.

Before importing it on Fusion360, I drew a rough sketch of a section view of the keyboard, to understand what would have been the minimum height it could get, considering Choc switch's height and the safest thickness of a 3D printed bottom plate, which I knew is 2mm. Here's the sketch:

<img src="/images/_01_sketch.jpg" width="500">

As you can see, I also kept note of the nice!nano's dimensions for the final designing process on Fusion, while on the bottom there's what I call [_the tetralobe_](/images/05_bottom_tetralobe.jpg) scheme: it will accommodate one of the four screws (indicated with a _+_ sign) to fix the bottom plate, a magnet (indicated with an _M_), and a little rubber feet (indicated with a _P_), while the fourth hole will accommodate the other half feet. I hope everything will be clearer with this video:

https://github.com/FranDes/Frandestein_keyboard/assets/16577794/49385803-7e35-41c4-909c-84a84e1e15bb

Finally, I modeled the keyboard on Fusion. [Here](/stl) you can find the _.stl_ files.

## Parts
These are the parts I used for this build:

**Original build**
* [3D printed case](/stl)
* [Pro Red Choc switches](https://splitkb.com/collections/switches-and-keycaps/products/kailh-low-profile-choc-switches?variant=39459382231117)
* [Blank MBK Choc Low Profile Keycaps](https://splitkb.com/collections/switches-and-keycaps/products/blank-mbk-choc-low-profile-keycaps)
* [2x nice!nano's v2](https://splitkb.com/products/nice-nano)
* [MCU sockets](https://www.aliexpress.us/item/32847506950.html)
* [2x MSK-12C02 ON/OFF switches](https://www.aliexpress.us/item/4001202080623.html)
* [2x 401235 Li-ion 3,7V 120mAh batteries](https://www.ebay.it/itm/202170224315)
* 2x reset buttons taken from a dead mouse
* 8x neodymium magnets (for the [carrying solution](https://github.com/FranDes/Frandestein_keyboard/assets/16577794/49385803-7e35-41c4-909c-84a84e1e15bb))
* [THT Diodes](https://splitkb.com/products/tht-diodes)
* Various wires taken from an old SCART cable

**Mods**
* 1mm plexiglass sheet
* [2x normally-closed reed switches](https://www.aliexpress.com/item/1005001688562983.html)


## Building process
Before building the keyboard, I made two little schemes to wire everything correctly. Given that my previous wireless keyboard was a CRKBD, I followed its wiring so that I didn't need to flash a new firmware.

Here are the schemes (_dall'alto_ and _dal basso_ mean _top view_ and _bottom view_):

<img src="/images/_02_scheme_left.jpg" width="500">

<img src="/images/_03_scheme_right.jpg" width="500">

## Final build

<img src="/images/01_top.jpg" width="500">

<img src="/images/02_top_left.jpg" width="500">

<img src="/images/03_controller_left.jpg" width="500">

<img src="/images/04_bottom.jpg" width="500">

<img src="/images/05_bottom_tetralobe.jpg" width="500">

<img src="/images/06_bottom_opened.jpg" width="500">

<img src="/images/07_bottom_left_opened.jpg" width="500">

<img src="/images/08_bottom_right_opened.jpg" width="500">

<img src="/images/09_reset_switch.jpg" width="500">

<img src="/images/10_onoff_switch.jpg" width="500">

## Mods

### Mod #1: Transparent bottom
The other day I bought a 1mm sheet of plexiglass to make a transparent bottom. Here's the final result:

<img src="/images/11_transparent_bottom.jpg" width="500">

<img src="/images/12_transparent_bottom_right.jpg" width="500">

### Mod #2: Reed switch for automatic on/off
A couple of weeks ago I learned about reed switches: they close (or open) the circuit when a magnet is near them. Here's how a normally-opened reed switch works:

<img src="https://images.squarespace-cdn.com/content/v1/5845aad637c5817b8945d213/1482454160872-HU1BIYDC17D45YKHJO6G/image-asset.gif">

So I thought it would have been cool to have the keyboard automatically turned off when it's in [carrying mode](https://github.com/FranDes/Frandestein_keyboard/assets/16577794/49385803-7e35-41c4-909c-84a84e1e15bb). I bought [normally-closed reed switches on AliExpress](https://www.aliexpress.com/item/1005001688562983.html) because the circuit should be open only when the keyboard is in carrying mode, while it should be closed the rest of the time. Here's what I received (Choc switch for reference):

<img src="/images/13_reed_switches_choc_comparison.jpg" width="500">

<img src="/images/14_reed_switch_zoom.jpg" width="500">

Instead of removing the two MSK-12C02 on/off switches I already installed, I just added the reed switches in series with them, so that I'm free to choose if I want to turn off the keyboard with the MSK-12C02 switch or by putting it in carrying mode. I hope this scheme (made with Paint :) ) will clarify what I did:

<img src="/images/17_reed_switch_mod_scheme.jpg" width="500">

This is the final result and a [live test](https://imgur.com/a/N7hXu72).

<img src="/images/15_reed_switch_mod_left.jpg" width="500">

<img src="/images/16_reed_switch_mod_right.jpg" width="500">

---

I hope you've found all this interesting. I'm here to answer any question.

Have a nice day :)
