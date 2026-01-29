# WristWatch Extruder with MK8 Filament Gear

![Extruder Image 1](https://github.com/minilogique/ww-extruder-for-idga/blob/main/images/2.png)
![Extruder Image 2](https://github.com/minilogique/ww-extruder-for-idga/blob/main/images/1.png)

Comparison between BMG teeth and MK8 teeth that grip the filament.  
MK8 has a **0.5 mm smaller effective diameter** at the filament path (measured from tooth tips).

![Teeth Comparison](https://github.com/minilogique/WristWatch-MK8/blob/main/images/IMG_5759.JPG)

Demonstration of pushing **95A TPU at 250 °C at 41 mm³/s**:  
https://www.youtube.com/shorts/knSDY8lV37g

---

## Assembly Notes

Assembly is identical to any **BMG gearset** or **WristWatch extruder**.  
Only the **main body** differs from the IDGA/RIDGA version.  
The **IDGA smooth bearing idler** can be reused as-is.

**Drive gear installation:**

1. Leave the drive gear loose on the shaft.  
2. Push filament through the extruder.  
3. Wiggle the gear into correct alignment.  
4. Tighten the set screw only after alignment is perfect.

Use threadlocker where needed.  
MK8 gears are not perfectly centered like Bondtech/FYSETC billet gears, but they are dramatically cheaper.

---

# Bill of Materials (BOM)

## Main Drive Gear Components

| Item | Notes | Approx. Price |
|------|--------|----------------|
| 50T reduction gear (Sherpa/WW/CW/Hex) | 5×28 mm shaft | ~5.5 € |
| MK8 drive gear (1.75 mm) | plastic hollowed gears are perfectly fine | 2.7 € single, or ~3 €/5 pcs (~0.60 €/pc)
| 2× MR85 smooth bearings | smooth type, no edges | ~4.7 €/10 pcs (~0.50 €/pc)
| 1× M3×16 flathead bolt | flathead is low profile and fits better | cents |
| 1× small-radius M3 washer | — | cents |

**Total cost with shipping: ~7 €**

---

## Main Hardware  
*(Same as A4T WW BMG / RIDGA / IDGA)*

- 2 × M3 thin square nuts  
- 2 × M3×20  
- 1 × M3×12  
- 1 × M3×16  
- 1 × M3×25  
- 1 × M3 thin washer  
- 1 × extruder spring  

---

## Smooth Idler Hardware

- 1 × 685‑2RS bearing  
- 1 × M3×16 flathead bolt  
- 1 × M3 thin washer  

---

# Performance Notes

- BMG clones have a **larger filament drive radius** and are often **more eccentric**, causing inconsistent extrusion.  
- MK8 diameter at tooth tips: **7.0 mm**  
- OEM Bondtech RIDGA: **7.5 mm**  
- MK8 teeth are **deeper**, improving grip.

### Rotation Distance

- Original RIDGA: `rotation_distance: 4.45`  
- MK8 setup: `rotation_distance: 4.05`  

This ~10% reduction increases torque by roughly the same amount.

### Real‑World Torque Evidence

Using ASA at **290 °C** through a **Goliath hotend** with a **0.5 mm non‑CHT nozzle**, the extruder pushed filament so hard that:

- 1.75 mm filament entered  
- 1.6 mm filament exited (melt zone saturated)  
- Filament remained in glass transition and “rebuilt” itself after extrusion

Idler tension should be slightly higher — **let the teeth bite in**.

---
