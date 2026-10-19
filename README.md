# DASAnalysis

This repository is a focused snippet from my thesis research on distributed
acoustic sensing (DAS) strain coupling.

## Scope of this snippet

- Gravity-coupling test data processing and analysis
- Air-liner coupling test data processing and analysis

This repository section is intentionally limited and does **not** cover the full
thesis workflow. Tube-in-tube experiment work is excluded from this snippet.

## Units convention

For thesis-facing reporting in this snippet, use imperial units only:

- Distance: inches (in) or feet (ft)
- Pressure: pounds per square inch (psi)
- Time: seconds (s)

## What this code does

- Preprocesses DAS TDMS data into analysis-ready files
- Runs strain/displacement analysis for gravity and air-liner coupling cases
- Produces exploratory plots and transfer-ratio metrics for comparison across runs

## Cable layout and figure color labels

Four cables run through the PVC and are fusion-spliced into one continuous fiber
so a single interrogator records them at once:

- Simplex Singlemode Plenum (TLC S09SX01CZNPY12), used as the reference and
  Gorilla-taped to the PVC exterior
- BRUsens Acoustic
- BRUsens Strain V4
- AFL FIMT (1/8 in diameter, thixotropic gel fill; singlemode x1, multimode x2)

In the analysis figures, section labels (Reference, Yellow, Green, Blue, Steel)
mark 10-channel averages along that spliced fiber path.

Color mapping:

- Yellow = Simplex (reference)
- Green = BRUsens Acoustic
- Blue = BRUsens Strain V4
- Steel = AFL FIMT
