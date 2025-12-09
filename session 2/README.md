Session 2 – UDP Measurements & Extended Analysis

Session 2 includes a second dataset obtained under a different measurement window.  
It replicates the full pipeline of Session 1 but with independent measurement files and plots.

Contents

```
session2/
├── audio/
│   ├── song1_DPCM_Samples
│   ├── song1_DPCM_Subs
│   ├── song1_AQ-DPCM_Samples
│   ├── song1_AQ-DPCM_Subs
│   ├── song1_AQ-DPCM_M
│   ├── song1_AQ-DPCM_B
│   ├── song2_DPCM_Samples
│   ├── song2_DPCM_Subs
│   ├── song2_AQ-DPCM_Samples
│   ├── song2_AQ-DPCM_Subs
│   ├── song2_AQ-DPCM_M
│   ├── song2_AQ-DPCM_B
│   └── (any other sound output files)
│
├── data/
│   ├── E####_DELAY.txt
│   ├── E####_NO_DELAY.txt
│   ├── ITHAKICOPTER.json
│   ├── V0103.json
│   ├── generator_DPCM_Samples
│   ├── generator_DPCM_Subs
│   └── (other raw data if needed)
│
├── plots/
│   ├── *.png     ← όλα τα MATLAB-generated plots (G1–G21)
│
├── parameters.txt
└── README.md
```

RTT Statistical Metrics

From "parameters.txt":

- **Mean RTT:** 2.05 × 10³ ms  
- **Variance:** 3.37 × 10⁵  
- **Adaptive filtering parameters:**  
  - a = 0.8  
  - bt = 0.9  
  - c = 3  

Used for SRTT/σ/RTO computation in MATLAB.

MATLAB Output

All plots generated from this dataset follow the same naming convention as Session 1 and are stored in the `plots/` directory.

