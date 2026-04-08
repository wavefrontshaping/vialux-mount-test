# ViALUX DMD Mount Stability Comparison

Comparative analysis of different mounting strategies for ViALUX DMDs in holographic setups. DMDs are not originally designed for interferometric applications and can suffer from mechanical vibrations transmitted through the rigid flat cable connecting the DMD board to the PCB (including fan vibrations). This project evaluates the new dedicated ViALUX mount against homemade solutions.

## Tested configurations

- **Mirror** (reference)
- **Custom mount** (homemade)
- **Custom mount + Foam** (homemade with vibration damping)
- **ViALUX mount** (commercial, recently released by ViALUX)
- **ViALUX mount + LS** (with locking screws)
- **ViALUX mount + LS + Foam** (with locking screws and foam damping)

## Method

Phase stability is measured via interferometric fringe analysis. For each configuration, 5 runs of ~180 s at ~40 fps are recorded. Analysis includes:
- Temporal phase standard deviation
- Power spectral density (Welch's method) with peak detection

## Structure

- `Data_analysis.ipynb` — Main analysis notebook
- `data/` — Raw measurement data (`.npz`)
- `latex/` — Report/paper source (LaTeX)
- `out/` — Generated figures (SVG + PDF)

## Report

- [Full PDF report](latex/Vialux_mount_test_2026.pdf) — Detailed write-up including experimental setup, methodology, results, and discussion.
- [Online version on wavefrontshaping.net](https://www.wavefrontshaping.net/post/id/91)

## Authors

Antoine Loquet and Sébastien M. Popoff  
Institut Langevin, ESPCI Paris, PSL University, CNRS, France
