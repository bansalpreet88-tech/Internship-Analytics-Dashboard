# Internship Analytics Dashboard - Road Accident Analysis

An interactive visual analytics project analyzing UK Road Accident data to understand temporal, environmental, and spatial patterns of traffic accidents and severity drivers.

## 📊 Overview

This project features an interactive **Tableau Dashboard** (`Book1.twb`) supported by data engineering and visual analytics workflows. It integrates multiple dimensions of accident data to help uncover key insights into traffic safety.

### Key Dimensions & Features Analyzed
- **Temporal Trends**: Accident volume over time (Month/Year) and peak risk hours throughout the day.
- **Severity Breakdown**: Distribution of Fatal, Serious, and Slight accidents with severity color indicators.
- **Environmental Factors**: Analysis of weather conditions and road types correlated with accident frequency.
- **Geographic Visualizations**: Interactive map plotting accident severity locations.
- **Day vs. Hour Heatmap**: Visualizing high-density accident timeframes across weekdays.

---

## 📁 Repository Structure

```
├── AccidentsBig.csv          # Primary Road Accident Dataset
├── AccidentsBig.csv.zip      # Compressed Dataset Archive
├── Book1.twb                 # Tableau Dashboard Workbook
├── updated sheet/
│   ├── AccidentsBig.csv      # Updated Data Sheet
│   └── nxtstep.txt           # Dashboard Build Guide & Guide Steps
└── README.md                 # Project Overview & Documentation
```

---

## 🛠️ Prerequisites & Setup

1. **Tableau Desktop / Tableau Public**: Open `Book1.twb` to explore or edit the interactive dashboards.
2. **Dataset**: `AccidentsBig.csv` contains the underlying records used by the calculated fields and worksheets.

---

## 🎯 Calculated Fields & Implementation Summary

- **Hour**: `DATEPART('hour', [Time])`
- **Severity Label**: Classified into `Fatal`, `Serious`, and `Slight`.
- **Urban/Rural Label**: Classified into `Urban` and `Rural` zones.
- **Month/Year & Day of Week**: Extracted date dimensions for temporal cross-filtering.
