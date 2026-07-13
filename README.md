# Dataset Directory Structure

The dataset is organised hierarchically according to vegetation type, fuel type, combustibility treatment, experimental replicate, and data category.

```text
Bushfire-Fuel-Watch-Pilot-Data/
│
├── Native_Forest_Eucalypt/
│   ├── Canopy/
│   │   ├── High_Combustibility/
│   │   │   ├── Euc_Can_HC_R1_YYYYMMDD/
│   │   │   │   ├── Biochemistry/
│   │   │   │   ├── Fire_Behaviour/
│   │   │   │   │   ├── Exit_view/
│   │   │   │   │   ├── logger_data/
│   │   │   │   │   ├── stills/
│   │   │   │   │   └── top_view/
│   │   │   │   ├── GHG/
│   │   │   │   └── Spectral/
│   │   │   │       ├── Euc_Can_HC_R1_YYYYMMDD_hyper/
│   │   │   │       └── Euc_Can_HC_R1_YYYYMMDD_SWIR/
│   │   │   ├── Euc_Can_HC_R2_YYYYMMDD/
│   │   │   └── ...
│   │   └── Low_Combustibility/
│   │       ├── Euc_Can_LC_R1_YYYYMMDD/
│   │       └── ...
│   └── Litter/
│       ├── High_Combustibility/
│   │       ├── Euc_Lit_HC_R1_YYYYMMDD/
│   │       └── ...
│       └── Low_Combustibility/
│   │       ├── Euc_Lit_LC_R1_YYYYMMDD/
│   │       └── ...
└── Grass_Ryegrass/
    └── Pasture/
        ├── High_Combustibility/
            ├── Gra_Pas_HC_R1_YYYYMMDD/
            └── ...
        └── Low_Combustibility/
            ├── Gra_Pas_LC_R1_YYYYMMDD/
            └── ...
```
# Directory Hierarchy

The dataset follows the hierarchy below:

| Level | Description |
|--------|-------------|
| **Vegetation Type** | Two vegetation types were investigated, Native_Forest_Eucalypt and Grass_Ryegrass. |
| **Fuel Type** | Three Fuels were collected from those vegetation types, Canopy(Can), Litter(Lit) and Pasture(Pas). |
| **Combustibility Treatment** | Fuel prepared under either Low (LC) or High (HC) combustibility conditions. |
| **Replicate** | Individual experimental replicates (R#). |
| **Data Category** | Measurements collected for each experiment, Fire_Behaviour, GHG and Spectral. |

# Experimental Design

| Vegetation Type | Fuel Type | Combustibility Treatment | Replicates |
|-----------------|-----------|--------------------------|-----------|
| Native forest (Eucalypt) | Canopy | Low | R1-R4 |
| Native forest (Eucalypt) | Canopy | High | R1-R4 |
| Native forest (Eucalypt) | Litter | Low | R1-R6 |
| Native forest (Eucalypt) | Litter | High | R1-R4 |
| Grass (Ryegrass) | Pasture | Low | R1-R4 |
| Grass (Ryegrass) | Pasture | High | R1-R4 |

Each replicate contains the following subfolders.

## Biochemistry

Contains biochemical properties of the vegetation samples, including:
- Cellulose content
- Carbon content
- Chlorophyll a
- Chlorophyll b
- Carotenoids
- Leaf area
  
## Fire_Behaviour

Contains observations and measurements describing free-spreading fire behaviour collected during each combustion experiment.
- **Exit_view/** – Images and videos captured from the downstream (exit) view of the combustion wind tunnel.
- **top_view/** –  Videos captured from overhead cameras.
- **stills/** – Selected still images extracted from the experiment.
- **logger_data/** – Experimental logger outputs and associated sensor measurements.

## GHG

Contains greenhouse gas and particulate emissions measured during combustion, including:
- CO₂
- CO
- CH₄
- PM2.5

## Spectral

Contains hyperspectral imagery collected before and after burning to characterise fuel spectral properties over the 400–2500 nm wavelength range.

Each replicate contains two hyperspectral datasets:

- **hyper/** – Visible and Near-Infrared (VNIR) hyperspectral imagery.

- **SWIR/** – Short-Wave Infrared (SWIR) hyperspectral imagery.

These datasets include the raw and processed hyperspectral products associated with each experimental replicate.
