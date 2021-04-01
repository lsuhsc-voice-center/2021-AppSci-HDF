# Supplementary material for Applied Science manuscript: "Development of parameters towards voice bifurcations"

## Abstract

Pathological vocal folds are known to exhibit multiple oscillation patterns, depending on tissue imbalance, subglottal pressure level, and other factors. This includes mid-phonation changes due to bifurcations in the underlying voice source system. Knowledge of when changes in oscil-lation patterns occur is helpful in the assessments of voice disorders, and the knowledge could be transformed into useful objective measures. Mid-phonation bifurcations can occur in rapid suc-cession; hence, a fast classification of oscillation pattern is critical to minimize averaging of data across bifurcations. This paper proposes frequency-ratio based short-term measures, named harmonic disturbance factor (HDF) and biphonic index (BI), towards the detection of the bifurca-tions. For the evaluation of HDF and BI, a frequency selection algorithm for glottal source signals is devised, and its efficacy is demonstrated with the glottal area waveforms of four cases, repre-senting the wide range of oscillatory behaviors. The HDF and BI exhibit clear transitions when the voice bifurcations are apparent in the spectrograms. The presented proof-of-concept experiment outcomes warrant a larger scale study to formalize the parameters of the frequency selection algorithm.

## Repository Content

This repository contains the data used for the preparation of the manuscript. Source code to reproduce the figures will be added later.

## Data File

Data is found in `data/case_data.h5` file which is in HDF5 file format with the following sturucture:

```
    case_data.h5
    ├── 0 [attributes: fs_gaw, fs_snd]
    │   ├── gaw
    │   └── snd
    ├── 1 [attributes: fs_gaw, fs_snd]
    │   ├── gaw
    │   └── snd
    ├── 2 [attributes: fs_gaw, fs_snd]
    │   ├── gaw
    │   └── snd
    └── 3 [attributes: fs_gaw, fs_snd]
        ├── gaw
        └── snd
```

The 0-based top-level group's numbering corresponds to the 1-based case numbering in the manuscript (0 = Case 1, 2 = Case 2, etc.).
In each case group, the `gaw` and `snd` datasets are the glottal area waveform and acoustic waveform, respectively. 
Their sampling rates (`fs_gaw` and `fs_snd`) can be found in the attributes of the case group.

