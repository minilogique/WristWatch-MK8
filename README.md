WristWatch extruder with MK8 filament gear.

![alt_text](https://github.com/minilogique/ww-extruder-for-idga/blob/main/images/2.png)

![alt text](https://github.com/minilogique/ww-extruder-for-idga/blob/main/images/1.png)

Comparison between BMG teeth and MK8 teeth that grip the filament. Also 0.5mm smaller diameter for MK8 at the filament path measured from the tips of the teeth.

![alt text](https://github.com/minilogique/WristWatch-MK8/blob/main/images/IMG_5759.JPG)

Look it push 95A TPU at 250C at 41mm3/s without an issue at https://www.youtube.com/shorts/knSDY8lV37g



Assembly goes just like with any BMG gearset and any WristWatch extruder, just the main body is different from the IDGA/RIDGA version and you can reuse IDGA smooth bearing idler as a whole. When installing the gear to the main body, leave the drive gear loose and after pushing filament through it, wiggle the gear on a proper spot on the shaft and only then tighten it.

Use threadlocker where needed. Be wary that it's far for perfectly centered like Bondtech or FYSETC billet gears, however it comes in wayyyy cheaper compared to both offerings (16+€ and they include idler gear aswell, just the main gear with shaft cannot be purchased separately, only comes as a set).

 [!BOM]
> 50T reduction gear for Sherpa/WW/CW/Hex with 5x28mm shaft (about 5.5€)
> MK8 drive gear for 1.75mm filament (2.7€ single or about 3€/5pc (about 0.60€/pc) if you can find like that)
> 2x MR85 smooth bearing without and edges etc (4.7€/10pc or about 0.50€ per piece) and a flathead M3x16 bolt and one tiny radius M3 washer
Main hardware (same as for A4T WW BMG/RIDGA/IDGA)
> 2 M3 thin square nuts
> 2 M3x20 
> 1 M3x12 
> 1 M3x16
> 1 M3x25
> 1 M3 thin washer
> 1 extruder spring
For smooth idler
> 1 685-2RS bearing
> 1 flathead M3x16
> 1 M3 thin washer


Prices for the main drive gear parts with shipping are about 7€ making it less than half what others cost. Now why shouldn't you get the BMG clones instead for a bit extra and be done with it? Well, those are actually larger in diameter when measured the filament drive radiuses and also eccentric which means even more deviation in filament drive radius. Look at the second picture where I have BMG next to MK8, both are meant for 1.75mm filament. Billet versions are at least 14€ or twice the price, but usually closer to 20€.

When measured, my OEM Bondtech RIDGA from WW extruder I replaced was 7.5mm from the tips of the filament teeth while MK8 is at 7mm in diameter. HOWEVER the teeth on MK8 drive gear are visibly deeper. While the original RIDGA is "rotation_distance: 4.45" it now should be set to "rotation_distance: 4.05". That equals do about 10% more torque compared to BMG/OEM Bondtech gearset.

Considering that the rotation_distance got reduced by almost 10%, then the torque actually got increased by a significant amount. Proof for it is in the last picture where I used ASA at 290C through Goliath hotend with TC 0.5mm nozzle without CHT geometry and if the meltzone got saturated, the 1.75mm filament that went in came out at 1.6mm through 0.5mm nozzle. Idler tension has to be a bit higher compared to some other extruders. Let the teeth dig in. For the torque look at the last photo where it pushed so much filament that it did not fully melt, rather was still in glass transition so it "rebuilt" itself after extruder from the nozzle.
