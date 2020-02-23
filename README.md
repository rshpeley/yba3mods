# yba3mods
Mods to the Traynor yba3 bass guitar amp.

### Mike's mods
The files `yba3-mikes-mods-final` are the final revision of the mods I made to Mike's mid 1967 Traynor YBA-3 amp. The notes in the schematic explain what changes were made, and why, but don't go into much detail.

These mods were:
1. The 2 wire power cord was replaced with a three wire power cord. The AC filter cap now connects from neutral AC to ground to absorb transients from the leakage inductance of the power transformer when the amp is switched off.
2. The stacked power supply caps in the original design results in a cascade failure if one of the caps in the string fails short (i.e. the cap shorts out). They were replaced by paralleled higher voltage caps. 
3. Added a 390K 2W standby resistor which leaks a small current while in standby mode to limit the power supply cap surge current when the amp is switched out of standby. It can also be used to reform the power supply caps if the amp hasn't been used for more than a year. To do this remove all the tubes, put the standby switch into standby mode (with the switch handle in the down position) and turn on AC power. Leave it for at least 8 hours. If you switch on the standby switch without the tubes in the circuit you're going to severely stress some caps. __Don't do that__. Remember to turn off the amp and put the tubes back in before you power it on again.  
4. Power tube suppressor grids are returned to ground instead of negative bias. I know what some people say about the suppressor grid bias to negative, but I found that quiescent screen grid current was just too high. Leaving it original was goimg to reduce the lifetimes of the power tubes, and frankly the power stage sounds more dynamic.
5. The bias voltage range was adjusted to allow biasing the output tubes with grounded suppressor grids.
6. The '68 preamp stage voltage wiring was used to reduce the input stage voltages and to provide better power filtering.
7. Ceramic caps were replaced with silver mica or orange drop polyester film/foil types. Most of these caps are microphonic (tap on them with a screwdriver when the amp is on but not too loud). 
8. A presence switch was added to lossen up the damping of the output stage in the mid to higher frequencies.
9. The power tube negative bias resistors were reduced in value to reduce the effect of control grid leakage. 
10. The thyrectors across the output transformer were removed and reverse biased rectifiers to ground were used in their place. Both of these methods reduce the high voltages produced from output transformer leakage inductance when a cabinet is disconnected from the output.
11. The power tubes were wired to allow operation in pairs instead of quads. V4/V7 or V5/V6 may be removed to reduce the output power of the amp when driving a higher impedance cabinet. Independent group screen resistors shown in Note 4 on schematic 3 permits these groupings to work.
12. Four 1 ohm cathode resistors allows power tube cathode currents to be independently measured when setting power stage bias currents.

### Have mods to contribute?
If you've made mods to the YBA-3 and would like to post them here, just clone this repository, make your changes to the svg schematic files and create a pull request.

Or if you have a GitHub account just post your mods there.

### Have a question or suggestion?
Go to the GitHub Issues tab and open an issue.

If you're wondering how the amp sounds, Mike said it nailed the Marshall sound. Personally I think the YBA-3 has more power dynamics than the Marshall. Its distortion balance is more towards the preamp side giving the power stage a bit more dynamic room with its more robust Hammond power transformer. 

The amp is also very quiet with virtually no hum without an instrument plugged in.

