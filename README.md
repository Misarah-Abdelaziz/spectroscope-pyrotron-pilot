# Dataset Directory Structure

The dataset is organised hierarchically according to vegetation type, fuel type, combustibility treatment, experimental replicate, and data category.

```text
spectroscope-pyrotron-pilot/
│
├── Native_Forest_Eucalypt/
│   ├── Canopy/
│   │   ├── Low_Combustibility/
│   │   │   ├── Euc_Can_LC_R1_YYYYMMDD/
│   │   │   ├── Euc_Can_LC_R2_YYYYMMDD/
│   │   │   └── ...
│   │   └── High_Combustibility/
│   │       ├── Euc_Can_HC_R1_YYYYMMDD/
│   │       └── ...
│   │
│   └── Litter/
│       ├── Low_Combustibility/
│       └── High_Combustibility/
│
└── Grass_Ryegrass/
    └── Pasture/
        ├── Low_Combustibility/
        └── High_Combustibility/
```

Each replicate folder contains three data categories:

```text
Replicate/
│
├── Fire_Behaviour/
├── GHG/
└── Spectral/
```

# Directory Hierarchy

The dataset follows the hierarchy below:

| Level | Description |
|--------|-------------|
| **Vegetation Type** | Two vegetation types were investigated. |
| **Fuel Type** | Fuel component collected from each vegetation type. |
| **Combustibility Treatment** | Fuel prepared under either Low or High combustibility conditions. |
| **Replicate** | Individual experimental replicate (R1–R4). |
| **Data Category** | Measurements collected for each experiment. |

# Experimental Design

| Vegetation Type | Fuel Type | Combustibility Treatment |
|-----------------|-----------|--------------------------|
| Native forest (Eucalypt) | Canopy | Low |
| Native forest (Eucalypt) | Canopy | High |
| Native forest (Eucalypt) | Litter | Low |
| Native forest (Eucalypt) | Litter | High |
| Grass (Ryegrass) | Pasture | Low |
| Grass (Ryegrass) | Pasture | High |

Each treatment contains **four experimental replicates (R1–R4)**.

# Data Categories

Each replicate contains the following subfolders.

## Fire_Behaviour

Contains measurements describing free-spreading fire behaviour, including quantities such as:
- Rate of spread
- Flame characteristics
- Fire progression
- Other fire behaviour outputs

## GHG

Contains greenhouse gas and particulate emissions measured during combustion, including:
- CO₂
- CO
- CH₄
- VOCs
- Other emission products (where applicable)

## Spectral

Contains hyperspectral measurements collected before and/or after burning, including spectral reflectance data across the **400–2500 nm** wavelength range and associated processed products.

# Example

```text
Native_Forest_Eucalypt/
└── Canopy/
    └── High_Combustibility/
        └── Euc_Can_HC_R1_20250221/
            ├── Fire_Behaviour/
            ├── GHG/
            └── Spectral/
```

This folder corresponds to:
- **Vegetation Type:** Native forest (Eucalypt)
- **Fuel Type:** Canopy
- **Combustibility:** High
- **Replicate:** R1
- **Experiment date:** 21 February 2025
