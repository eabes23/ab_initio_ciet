# Raw grids

Each file is a 481 × 481 comma-separated matrix in eV, with no header or row names.

- `ox_surface.txt`: oxidized (CO₂) diabatic free energy
- `red_surface.txt`: reduced (CO₂⁻) diabatic free energy, at zero driving force
- `H_OR_surface.txt`: electronic coupling H_OR (not squared)

**Rows (top to bottom) correspond to q̃, the electron-transfer coordinate.** q̃ = (row − 100)/281:
- q̃ = 0 (oxidized minimum) at row 100
- q̃ = 1 (reduced minimum) at row 381

**Columns (left to right) correspond to ξ̃, the ion-transfer coordinate.** ξ̃ decreases from left to right:
- the leftmost column is closest to the electrode (z ≈ 1.7 Å)
- ξ̃ = 1 at z = 2.35 Å
- ξ̃ = 0 at z = 5.06 Å
- the rightmost column is farthest from the electrode (z ≈ 5.7 Å)

Here z is the distance of the carbon atom from the electrode, and ξ̃ = (5.06 − z)/2.71.
