# PCB Edge Clamp

Parametric 3D-printable edge clamp: screw it to your enclosure, it holds the PCB by its edges. No mounting holes needed on the board.

<img width="400" alt="PCB Edge Clamp" src="https://github.com/user-attachments/assets/bb5d4741-06ad-4f4a-9f2e-f5d87899753e" />
<img width="400" alt="PCB Edge Clamp Usage" src="https://github.com/user-attachments/assets/79da93b8-623b-4444-a9e7-d48175df1f06" />

## Files

| File | Use |
|---|---|
| `PCB_Edge_Clamp.3mf` | Ready to print (default parameters for M2) |
| `PCB_Edge_Clamp.stl` | Import into any 3D software |
| `PCB_Edge_Clamp.FCStd` | FreeCAD source, fully parametric |

## Printing

- Print the piece lying on its side (flat profile on the smooth bed): no support is needed and the hook is stronger.
- Tested with default printing settings: PLA 0.2 mm layers.

## Customizing in FreeCAD

1. Open `PCB_Edge_Clamp.FCStd`.
2. Click on `VarSet` in the model tree.
3. Edit the values.
5. Check the `check` cell: it must read `OK`.
6. Select the Body, then **File -> Export** as STL or 3MF.

| Parameter | Default | Description |
|---|---|---|
| `pcb_thickness` | 2 mm | PCB thickness |
| `width` | 5 mm | Width of the clamp |
| `screw_hole_d` | 2.4 mm | Screw clearance hole (M2) |

If the screw hole is too large for the clamp width, the model shows an error on recompute and takes the clamp width in fallback.
