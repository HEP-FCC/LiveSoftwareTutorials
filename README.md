# Live Software Tutorials

This repository collects hands-on software tutorials for FCC and DRDCalo
activities. It includes an FCC workflow covering the full chain from event
**Gen**eration through fast/parametric **Sim**ulation with Delphes to physics
**Analysis**, together with entry points for the DD4hep and Gaudi tutorials
maintained in the
[DRDCalo SoftwareTutorials repository](https://github.com/DRDCalo/SoftwareTutorials).

## Tutorial areas

- [DD4hep](DD4Hep/): detector-description and simulation exercises.
- [Gaudi](Gaudi/): Gaudi and Key4hep algorithms, steering, and data-processing
  exercises.
- [Generation](Gen/): event generation and showering/decay.
- [Simulation](Sim/): fast detector simulation with Delphes.
- [Analysis](Analysis/): physics selections, histogram production, and plotting.

The `DD4Hep` and `Gaudi` directories link to their corresponding tutorial
material in `DRDCalo/SoftwareTutorials`, keeping a single maintained copy of
the source code and exercises.

## Generation-to-analysis physics cases

- **FCC-ee (full path):** e+e- -> mu mu H, H -> b b (WHIZARD + Pythia + Delphes IDEA card),
  analysed as Z(-> mu mu) H with a recoil-mass measurement and a H -> bb dijet mass.
- **FCC-hh (shorter, advanced transfer):** HH -> b b gamma gamma, reusing the FCC-ee
  material with less hand-holding, extending the physics objects covered to photons.

## Structure

The repository is organized into the following top-level directories. The
generation, simulation, and analysis stages are split by collider, with
worked solutions nested inside each collider directory.

```
DD4Hep/          Link to the DD4hep tutorial in DRDCalo/SoftwareTutorials
Gaudi/           Link to the Gaudi tutorial in DRDCalo/SoftwareTutorials
Gen/
  ee/            FCC-ee generation (WHIZARD -> HEPMC) and showering/decay (Pythia)
    solutions/   Worked solution, for offline use
  hh/            FCC-hh generation, starting from existing LHE
    solutions/
Sim/
  ee/            Delphes fast simulation, FCC-ee IDEA card
    solutions/
  hh/            Delphes fast simulation, FCC-hh card
    solutions/
Analysis/
  ee/            Stage1 (tagger + ntuple production) and Stage2 (selections/plots) for FCC-ee
    solutions/
  hh/            Stage1/Stage2 for FCC-hh
    solutions/
```

## Format

The generation-to-analysis sections are introduced with brief slides, after
which students work through the Markdown material directly in this repository
(VSCodium with suitable extensions is recommended for an all-in-one setup).
Students present their solutions, and reference solutions are provided for
offline use.

The linked DD4hep and Gaudi areas provide their own presentations, build
instructions, source code, and exercises in `DRDCalo/SoftwareTutorials`.

## Branches

Specific schools/dates are tracked as branches or tags off `main`.

## License

Copyright (c) 2026 CERN. The documentation and material in this repository
is licensed under the
[Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)](https://creativecommons.org/licenses/by-sa/4.0/)
license — see [LICENSE](LICENSE).
