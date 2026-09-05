# 🌲 TreeSense Imaging Legacy (v1)

> **⚠️ LEGACY ARCHIVE NOTICE**  
> This repository contains the original college prototype of **TreeSense Imaging**. It is preserved for historical reference only.  
>  
> The new version will be available at:  
> 👉 **[https://github.com/vipulchaturvedi/treesense-imaging](https://github.com/vipulchaturvedi/treesense-imaging)** (Please use that repository for newer features and future maintenance).

## Smart India Hackathon: TreeSense Imaging

## Image Analytics for Tree Enumeration
The project aims to address the challenge of accurately enumerating trees in forest areas earmarked for diversion due to developmental projects by developing an image analytics system utilizing satellite imagery or aerial photographs to automate tree enumeration. Traditional methods are time-consuming and prone to errors, making it crucial to develop an automated solution.

## Overview
The project includes a website with a landing page and a dashboard offering the following tools:

- **Tree Count:** Allows accurate tree counting within designated forest areas.
- **Green Cover Estimator:** Estimates green cover percentage.
- **Tree Species Identifier:** Identifies tree species.
- **Optimal Pathing:** [Computes the optimal path between two points within the area.](https://github.com/lag25/ForestPathPlanner)
- **Historical Data:** Provides historical data for analysis and comparison.

## Features
- Landing Page: Showcases project overview with easy onboarding.
- Dashboard: Offers toggle switches to access various tools.
- Interface: User-friendly interface for easy interaction and exploration of results.
- Integration: Seamless integration with forest management systems.
- Visualization: Generates maps, reports, and visual representations of tree enumeration data.

## Project Structure

```text
├── Dataset/             # YOLO format aerial tree detection dataset (train/val/test)
├── PythonScripts/       # Prototyping notebooks (Thresholding, Training, Pathing)
│   ├── BinaryImageThresholding.ipynb
│   ├── ModelTraining.ipynb
│   └── StructuredOptimalPathing (1).ipynb
├── screenshots/         # UI captures of the v1 legacy system
└── treesense/           # Primary application source (Static Web App)
    ├── index.html       # Landing page
    ├── predict.html     # Analysis dashboard frame
    ├── object_detection.html    # Client-side ONNX tree detection
    ├── object_segmentation.html # Canopy cover estimator
    ├── optimal_path.html        # Path planning prototype
    ├── historical_data.html     # Weather & climate charts
    ├── web_model/       # Converted TF.js model shards
    └── src/assets/      # CSS styles and JavaScript logic
```

## Screenshots
<center>

![Landing Page](screenshots/landing_page.png)

![Dashboard](screenshots/dashboard.png)

![Tree Count](screenshots/tree_count.png)

![Green Cover Estimator](screenshots/green_cover_estimator.png)

![Optimal Pathing](screenshots/optimal_pathing.png)

![Historical Data](screenshots/historical_data.png)

</center>

## Getting Started
To start using the tools, visit the website and navigate to the dashboard [here.](https://treesense-legacy.vipulchaturvedi.com/predict)

## 🛠️ Installation & Usage (npm Workflow)

### Prerequisites
* [Node.js](https://nodejs.org/) (v16 or higher)

### 1. Clone the Repository
```bash
git clone https://github.com/vipulchaturvedi/treesense-imaging-legacy.git
cd treesense-imaging-legacy/treesense
```

```bash
npm install
```

```bash
npm run build
npm start
```

Visit http://localhost:3000 in your browser.

## License
This project is licensed under GNU AGPLv3
