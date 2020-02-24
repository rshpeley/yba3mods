# yba3mods
Mods to the Traynor yba3 bass guitar amp.

### Mike's mods
The files `yba3-mikes-mods-final` in the Docs folder are the final revision of the mods I made to Mike's mid 1967 Traynor YBA-3 amp. The notes in the schematic explain what changes were made, and why, but don't go into much detail.

The early Traynor Custom Special heads were very robust and can be pushed further than a Marshall or Fender head. With a bit of work they lend themselves well to high gain and high speaker load mods with KT88 style tubes.

This Custom Special amp head is a mid-year 1967 model which is a mix of '67 and '68 models. The first stage has the bias resistor and capacitor of the '68. It has the choke of the '67 head with preamp power supplied through the choke (leading to more sag at higher power levels than the '68 to '70 models). It was wired for 6CA7 power tubes (the original including suppressor grid negative bias) and has a cooling fan.

The YC-810 Big B cabinet dates from about 1967 and consists of 8 RSC/Jensen 10" speakers wired in series parallel to give a cabinet impedance of 4 ohms. This cabinet has been a favourite with guitarists. 

#### Provenance
1967: rental amp at Musonic in West Hill, Ontario, Canada.
1967-1969: gigging amp for bassist Bob Fleming of the band Leather.
1970-1972: gigging amp for guitarist John Rolls of the band Bond.
1973-1975: occassional gigging and jamming amp for guitarist Michael Gwynne of Blues Innovation
1976-2019: rarely used
2019: serviced and modified by R. Shpeley

The following mods were performed and documentation can be found on GitHub at
https://github.com/rshpeley/yba3mods

####Power Supply
1. The 2 wire power cord was replaced with a three wire power cord for safety. The AC ground filter cap now connects from neutral AC to ground to absorb transients from the leakage inductance of the power transformer when the amp is switched off.
2. The ground switch was not required and was removed.
3. AC and power supply grounds were made to one common point.
4. Added a 390K 2W standby resistor which leaks a small current while in standby mode to limit the power supply cap surge current and to reform power capacitor dielectrics when the amp is in standby mode. 
5. The standby resistor can also be used to reform the power supply caps if the amp hasn't been used for more than a year. To do this remove all the tubes, put the standby switch into standby mode (with the switch handle in the down position) and turn on AC power. Leave it powered up for at least 8 hours. If you switch on the standby switch without the tubes in the circuit you're going to severely stress some caps. __Don't do that__. Remember to turn off the amp and put the tubes back in before you power it on again.
6. The '68 preamp stage power wiring was modified to the '68 to '70 revision to isolate the preamp from transient and high frequency sag effects allowing the phase inverter to be overdriven better at higher playing volumes. 
7. The power inductor of the '67 and the better filtering of the '68 to '70 power wiring makes for very low hum levels.
8. The stacked power supply caps in the original design results in a cascade failure if one of the caps in the string fails short (i.e. the cap shorts out). They were replaced by 2 banks of paralleled higher voltage sprague atom caps.

####Preamp 
1. Ceramic caps were replaced with silver mica or orange drop polyester film/foil types. Most ceramic caps are microphonic. Tap on them with a screwdriver when the amp is on at low volume to see for yourself.
2. Input jack ground connections have been isolated at the front panel to reduce hum pickup in this section.
3. Cathode bypass electrolytic caps were replaced with sprague atoms.

####Phase Inverter/Power Stage
1. The power tubes were wired for the option to reduce output power in half by running only 2 tubes, V4/V7 or V5/V6 groups, to better match 8 ohm cabinets. Independent group screen resistors shown in Note 4 on schematic 3 permits these tube groups to work.
2. Each power tube grid and screen have their own resistors to increase output stage high frequency stability.
3. Four 1 ohm cathode resistors have been added to measure the bias current of each output tube when setting power stage bias currents. 
4. The power tube grid bias resistors have been lowered in value to 100K to improve bias stability.
5. A presence switch added on the back panel (in place of the ground switch) provides optional presence feedback to the phase inverter (Marshall mod) to decrease speaker damping and increase output at mid to high frequencies. 
6. Thyrector transient suppressors across the output transformer were removed and replaced by reverse biased rectifiers to ground. Both of these methods reduce the high voltages produced from output transformer leakage inductance when a cabinet is disconnected from the output, but when one fails the rectifiers are easier to replace.
7. Power tube suppressor grids were wired to ground instead of negative bias.
8. The power tube bias voltage range was adjusted to allow biasing the output tubes with grounded suppressor grids.

####A note on the suppressor grid wired to -bias
The 6CA7 power pentode was available as either a true pentode or a beam power tube. It's not clear if Pete Traynor tested his suppressor grid wiring with Mullard/Philips EL34 pentodes or American 6CA7 beam power tubes. The negative bias voltage on the beam forming (suppressor) has very little effect on the characteristics of 6CA7 beam tube, but it substantially increases screen current in the EL34 pentodes. 

With negative bias on the suppressor, the EL34 style tube is at its screen dissipation limit with no signal. When a signal is applied screen dissipation exceeds its design limit which leads to early output tube failure. The solution is to either cut back output tube bias to 50% of plate dissipation (which makes the amp sound deader) or to ground the suppressor grids as done by Marshall. The non-linear effect of the -bias on the suppressor grid can alternately be achieved by increasing the screen resistance value, which also helps to prolong output tube life.

####Further mods

The second stage of the V1 tube (currently unused) can be wired as a gain stage similar to Train Wreck amps. KT88s, 6550 and similar tubes can be used in place of the 6CA7s (remove pin 1 wiring and mod bias voltage).

### Have mods to contribute?
If you've made mods to the YBA-3 and would like to post them here, just clone this repository, make your changes to the svg schematic files and create a pull request.

Or if you have a GitHub account just post your mods there.

### Have a question or suggestion?
Go to the GitHub Issues tab and open an issue.

If you're wondering how the amp sounds, Mike said it nailed the Marshall sound. Personally I think the YBA-3 has more power dynamics than the Marshall. Its distortion balance is more towards the preamp side giving the power stage a bit more dynamic room with its more robust Hammond power transformer. 

Overall, it's an impressive amp. It may even be better with KT88s.
