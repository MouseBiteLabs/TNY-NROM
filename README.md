# TNY-NROM
This is a custom NROM board for the TinyTendo handheld console by <a href="https://github.com/Redherring32">Redherring32</a>. This board replicates <a href="https://www.nesdev.org/wiki/NROM">standard NROM NES boards</a> - the simplest board type, used for many of the earliest NES games like Duck Hunt, Balloon Fight, and one of the most popular NES games that created millions of gamers and cemented Nintendo as a top-tier video game company for decades to come... <a href="https://nescartdb.com/profile/view/1076/chubby-cherub">Chubby Cherub</a>!

NROM games support up to 32 KB space for the PRG ROM and up to 8 KB for the CHR ROM. Since these boards use the 39SF040 for both, you should use FamiROM or some other utility to duplicate the ROM files to completely fill up the entire space on the Flash chip.

<a href="https://www.infiniteneslives.com/inlretro.php">You can use INL's programmer to load the PRG and CHR ROMs.</a>

# Board Characteristics

- Thickness: 1.6 mm
- Surface Finish: ENIG
- Chamfered edges (45°)

# Bill of Materials

Capacitors should be at least 16V rated.

| Reference Designator  | Part Number/Value | Footprint  |
| ------------- | ------------- | ------------- |
| U2  | <a href="https://www.mouser.com/ProductDetail/Microchip-Technology/SST39SF040-70-4C-WHE?qs=Oo69DRhzroe%2FJKrgAmUE5Q%3D%3D">39SF040</a>  | TSOP32  |
| U3  | <a href="https://www.mouser.com/ProductDetail/Microchip-Technology/SST39SF040-70-4C-WHE?qs=Oo69DRhzroe%2FJKrgAmUE5Q%3D%3D">39SF040</a>  | TSOP32  |
| C1  | 22 uF (tantalum) | 1206  |
| C2  | 100 nF (ceramic) | 0603  |
| C3  | 100 nF (ceramic) | 0603  |
| R1  | 47 kΩ (ceramic) | 0603  |

# H/V Pads

NROM games usually will have H and V pads on the PCB, you can find the original game in <a href="https://nescartdb.com/">NESCartDB</a> to find out which you should solder. FamiROM should also tell you as well - bridge the middle pad to the left for Vertical mirroring (H), bridge to the right for Horizontal mirroring (V). Yes, it is "backwards" but <a href="https://www.youtube.com/watch?v=UepNwgFJ83k&ab_channel=DisplacedGamers">there is a reason for it</a>.

# Revision History

## TNY-NROM-02

- Updated cart edge pinout
- Flipped location of PRG and CHR chips
- Changed footprint of PRG and CHR to slimmer TSOP32 package as defined in the datasheet
- Add keyhole in middle of board, off-center

## TNY-NROM-01

- Initial version

# License:
Licensed under the TAPR Open Hardware License (www.tapr.org/OHL)

©MouseBiteLabs 2022
