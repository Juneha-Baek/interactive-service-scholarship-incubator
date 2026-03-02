# Interactive Service Scholarship Incubator (ISSI)

Interactive visualization platform for analyzing predicted concept relationships in service research networks through 2030.

🔗 **Live Demo:** https://interactive-service-scholarship-incubator.vercel.app/

📄 **User Guide:** [Download PDF](./docs/ISSI_User_Guide.pdf)

---

## Overview

This platform visualizes link prediction results from service research papers, predicting which concept pairs are likely to be connected by 2030. Using hierarchical concept extraction and network analysis, the system helps identify emerging research priorities and interdisciplinary opportunities.

**Methodology:**

1. Concept extraction from research papers
2. Semantic embedding (allenai/specter)
3. K-means clustering for community detection
4. Community labeling via GPT-4o-mini
5. Link prediction modeling

---

## Key Features

| Feature | Description |
|---------|-------------|
| **Top Predicted Pairs** | Ranked concept pairs with prediction scores, metadata, and hierarchical child concepts |
| **Community Network** | Interactive force-directed graph comparing predicted vs. current connections |
| **Community Ranking** | Matrix analysis categorizing pairs as Accelerating/Stabilizing/Consolidating/Exploring |

## Project Structure

```
src/
├── components/
│   ├── ConceptPairItem.jsx
│   ├── NetworkGraph.jsx
│   ├── CommunityRanking.jsx
│   └── Tooltip.jsx
├── utils/
│   └── dataProcessors.js
└── App.jsx
```

---

## Data Sources

| Dataset | Description |
|---------|-------------|
| **FT50 Data** | 5,725 papers from FT50 journals + 811 papers from JSR |
| **Service Data** | 4,976 papers from Top 8 Service Research journals |

---

## Documentation

- **User Guide (PDF):** [Download](./docs/ISSI_User_Guide.pdf)
- **In-app Tooltips:** Hover over ⓘ icons for detailed explanations

---

## 👥 Team

**KAIST College of Business** × **ASU W. P. Carey School of Business**

---

## 📄 License

© 2025 Interactive Service Scholarship Incubator (ISSI). All Rights Reserved.