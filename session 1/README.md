Session 1 – UDP Measurements & Telemetry Collection

Session 1 includes the first complete set of measurements for:
- Echo packets (with and without delay)
- Camera image retrieval
- Temperature sensor packets
- DPCM and AQ-DPCM audio extraction
- UAV telemetry (IthakiCopter)
- Vehicle OBD-II sensor decoding

Contents

```
session1/
├── audio/
│   ├── generator_DPCM_Samples
│   ├── generator_DPCM_Subs
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
│   ├── *.png   ← MATLAB plots (G1–G21)
│
├── parameters.txt
└── README.md
```

MATLAB Analysis (Session 1)

The MATLAB script produces:
- RTT vs time plots (G1, G3)
- Throughput over 8-second windows (G2, G4)
- RTT histograms (G5–G8)
- RTO/SRTT/σ estimation (R1)
- DPCM & AQ-DPCM waveform and histogram analysis (G9–G18)
- UAV telemetry plots (G19–G20)
- Vehicle OBD-II sensor plots (G21)

RTT Statistical Metrics

Documented inside `parameters.txt`:

- **Mean RTT:** 1.66 × 10³ ms  
- **Variance:** 1.08 × 10⁵  
- **Adaptive filtering parameters:**  
  - a = 0.8  
  - bt = 0.9  
  - c = 3  


These parameters were used in MATLAB for SRTT, σ, and RTO estimation.
