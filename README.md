# ICARUS - Tree Phenotyping Tool

![软件图标](icon.ico)

ICARUS is a 3D reconstruction and phenotyping analysis tool based on RGB images captured by mini drones, specifically designed for plant phenomics research.

## Features

- 🚁 Integrated solution with DJI Mavic 3M drone and DJI Terra software
- 🌳 3D point cloud reconstruction and plant phenotypic feature extraction
- 📊 Supports multiple phenotypic parameter calculations:
-  Plant height
-  Canopy projection area
-  Maximum canopy diameter
-  Underbranch height, etc.
- 🔍 K-Means clustering algorithm for plant organ segmentation
- ⚡ Batch processing for large-scale data analysis

## Quick Start

### System Requirements
- OS: Windows 8/8.1/10/11 (x64)
- Recommended: Windows 11 Professional (x64)

### Installation Steps
1. Download the latest executable file
2. Ensure the following files are in the same directory:
   - `Icarus.exe`  (main program)
   - `plotter.exe`
   - `icon.ico`
3. Double-click`lcarus.exe`to run the program

### Basic Workflow
1. Load point cloud file  (`Load File`)
2. (Optional) Edit point cloud using Meshlab  (`Edit File`)
3. Apply point cloud filtering (`Denoise`)
4. Perform K-Means clustering segmentation (`K-Clustering`)
5. Calculate and export phenotypic data (`Measure`)


## Parameter Description

### Parameter Description
- `voxel size`: Downsampling parameter (default: 0.03)
- `alpha`: Boundary extraction value (default: 30)
  
### Undercanopy Height Calculation Parameters
- `n`: Number of point cloud groups (recommended in units of 1000)
- `deta`: Branching judgment ratio (default: 0.5)
  
## Batch Processing

Supports batch processing of point cloud data for the same tree species:
- Select`Menu` > `Batch processing`
- Choose single-file or multi-file processing
- Choose single-file or multi-file processing`\\Icarus\\OUTPUT\\`directory

## FAQ

❓ **Average nearest neighbor distance and K_Value show NA in the output table**
> Possible cause: Denoise operation was not performed before Measure

❓ **Underbranch height shows NA or is inaccurate**
> Adjust the n or deta values, or check if the tree shape is suitable for this software

## Development Team

- **lab**: State Key Laboratory of Plant Environmental Resilience, College of Biological Sciences, China Agricultural University, Beijing 100193, China.
- **Developers**: Dai Shicheng, Chen Yuqian
- **Team Members**: Chen Yuqian, Dai Shicheng, Tian Yuan, Xiang Zichen

## License
This project has applied for software copyright registration in the People's Republic of China (Registration No. 2025SR0560649)

---

💡 **Tip**: It is recommended to test parameters on a small number of samples before batch processing to find optimal settings.


