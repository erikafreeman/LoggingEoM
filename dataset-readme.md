# Dataset Documentation: HarvestData_STAll_Chem_tmod.csv

## Overview
This dataset contains chemical and environmental measurements from four headwater catchments in northern Ontario, Canada, collected between 2019-2021 as part of a study investigating logging impacts on stream dissolved organic matter (DOM).

## Dataset Specifications
- **Format**: Comma-separated values (CSV)
- **Rows**: 59 observations
- **Columns**: 53 variables
- **Time Period**: 2019-2021
- **Sampling Frequency**: Monthly during ice-free seasons
- **File Size**: [Size to be added] MB
- **Missing Data Code**: NA

## Site Information
- **Location**: Northeast of Lake Superior, Ontario, Canada
- **Catchment Size Range**: 0.115 to 0.140 km²
- **Forest Type**: Hardwood-dominated, hemi-boreal
- **Treatment Groups**: 
  - Control sites (C1, C2): Unlogged
  - Treatment sites (H1, H2): Logged in September 2020
  - Paired design: H1-C1, H2-C2

## Variable Descriptions

### Identifiers and Temporal Variables
| Variable | Unit | Description |
|----------|------|-------------|
| Unnamed: 0.1 | - | Row identifier |
| Unnamed: 0 | - | Secondary row identifier |
| Site | - | Catchment identifier (H1, H2, C1, C2) |
| date_adjusted | YYYY-MM-DD | Sampling date |
| order | integer | Sample order |
| t_mod | integer | Modified time index |

### Optical Properties
| Variable | Unit | Description |
|----------|------|-------------|
| fi | - | Fluorescence Index |
| hix | - | Humification Index; indicates humic substance content |
| mhix | - | Modified Humification Index |
| bix | - | Biological Index |
| a254 | abs/cm | Absorbance at 254nm |
| a300 | abs/cm | Absorbance at 300nm |
| E2_E3 | - | Ratio of absorbance at different wavelengths |
| S275_295 | nm⁻¹ | Spectral slope between 275-295nm |
| S350_400 | nm⁻¹ | Spectral slope between 350-400nm |
| SR | - | Slope ratio |

### Carbon and Nutrients
| Variable | Unit | Description |
|----------|------|-------------|
| TOC_conc2 | mg/L | Total Organic Carbon concentration |
| DOC | mg/L | Dissolved Organic Carbon |
| DIC | mg/L | Dissolved Inorganic Carbon |
| NO2.NO3 | mg/L | Combined Nitrite and Nitrate |
| NH4 | mg/L | Ammonium |
| SRP | μg/L | Soluble Reactive Phosphorus |
| TP | μg/L | Total Phosphorus |
| TN | mg/L | Total Nitrogen |

### Physical Parameters
| Variable | Unit | Description |
|----------|------|-------------|
| pH | - | pH value |
| cond | μS/cm | Conductivity |
| alk | mg/L CaCO₃ | Alkalinity |

### Major Ions
| Variable | Unit | Description |
|----------|------|-------------|
| Ca | mg/L | Calcium |
| K | mg/L | Potassium |
| Mg | mg/L | Magnesium |
| Na | mg/L | Sodium |
| SO4 | mg/L | Sulfate |
| Cl | mg/L | Chloride |
| SiO2 | mg/L | Silica |

### Trace Metals
| Variable | Unit | Description |
|----------|------|-------------|
| Al | μg/L | Aluminum |
| Fe | μg/L | Iron |
| Mn | μg/L | Manganese |
| Zn | μg/L | Zinc |
| Cd | μg/L | Cadmium |
| Cu | μg/L | Copper |
| Ni | μg/L | Nickel |
| Pb | μg/L | Lead |

## Quality Control
- All water samples filtered through 0.45 μm glass fiber filters
- Samples for DOM analysis stored at 4°C in dark conditions
- Analytical blanks and standards run every 10 samples
- Duplicate samples analyzed for 10% of measurements
- Detection limits available upon request

## Collection Methods
1. **Water Sampling**:
   - 500mL grab samples collected monthly
   - Samples taken from channel heads of streams
   - Filtered on-site or within 24 hours
   - Preserved according to analytical requirements

2. **Chemical Analysis**:
   - DOM quantified using Shimadzu TOC-L analyzer
   - Optical properties measured via fluorescence spectroscopy
   - Major ions and metals analyzed at Great Lakes Forestry Centre

## Usage Notes
1. Time series analysis should account for:
   - Seasonal variations in stream chemistry
   - Ice-free season sampling only
   - Treatment effect beginning September 2020

2. Data includes pre-treatment (2019-Sept 2020) and post-treatment (Sept 2020-2021) periods

3. Some variables may show high temporal variability due to:
   - Storm events
   - Seasonal changes
   - Treatment effects

## Data Processing
- Raw data cleaned and formatted in R
- Quality control flags removed for final dataset
- Time standardization applied
- Missing values coded as NA

## Access and Permissions
[To be completed based on project requirements]

## Known Issues or Limitations
1. Sampling limited to ice-free seasons
2. Some parameters show seasonal gaps
3. Storm event sampling may be underrepresented

## Updates and Versions
- Version: 1.0
- Last Updated: [Date]
- Update History: Initial release

## Contact
For questions about this dataset, please contact:
- **Primary Contact**: Erika C Freeman (erika.freem@gmail.com)
- **Data Manager**: [Name and contact to be added]

## References
Relevant publications using this dataset:
1. Freeman EC, et al. (2025) Logging disrupts the ecology of molecules in headwater streams. [Journal Information Pending]
