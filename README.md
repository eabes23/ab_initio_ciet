# Raw grids

Each file is a 481 × 481 comma-separated matrix in eV, with no header or row names.

- `ox_surface.txt`: oxidized (CO₂) diabatic free energy
- `red_surface.txt`: reduced (CO₂⁻) diabatic free energy, at zero driving force
- `H_OR_surface.txt`: electronic coupling H_OR (not squared)

Indices below are 1-based.

**Rows (top to bottom) correspond to q̃, the electron-transfer coordinate, which increases down the rows:**

q̃ = (row − 100) / 281

- q̃ = 0 (oxidized minimum) at row 100
- q̃ = 1 (reduced minimum) at row 381

**Columns (left to right) correspond to ξ̃, the ion-transfer coordinate, which decreases across the columns:**

z  = 1.70038 + 0.0083459 × (col − 1)   (Å)
ξ̃  = (5.06 − z) / 2.71

Here z is the distance of the carbon atom from the electrode, so z increases from left to right.

- column 1: z = 1.700 Å, ξ̃ = 1.240 (closest to the electrode)
- ξ̃ = 1 at column 79 (z = 2.351 Å)
- ξ̃ = 0 at column 404 (z = 5.064 Å)
- column 481: z = 5.706 Å, ξ̃ = −0.239 (farthest from the electrode)

The region bounded by (q̃, ξ̃) = (0, 0) and (1, 1) is therefore rows 100–381 and columns 79–404.
