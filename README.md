# Microsoft_Global_Buildings_Downloader_for_QGIS
A simple Jupyter notebook that integrates with the QGIS Notebook Plugin to download building footprints from Microsoft's Global Buildings dataset based on your current canvas extent.

# About Microsoft Global Buildings Dataset
Microsoft's Global Buildings (MGB) dataset is a comprehensive collection of over 1 billion computer-generated building footprints covering most of the populated world. The dataset was created using deep learning models applied to Bing Maps satellite and aerial imagery.
Key Features:

🌍 Global coverage across Asia, Africa, Latin America, Caribbean, North America, Europe, and Oceania
🎯 High-quality AI-detected building polygons
📐 Accurate geometric representations with confidence scores
🆓 Free and open data released under ODbL license
📈 Continuously updated and expanded

Note: This is distinct from the Google-Microsoft Global Building Atlas, which focuses on building height and characteristics. MGB provides detailed 2D footprint geometries ideal for GIS analysis, urban planning, and mapping applications.
✨ Features

No coding required - Just run the notebook cells in sequence
Automatic extent detection - Uses your current QGIS canvas extent
CRS transformation - Automatically handles coordinate system conversions
Smart tile management - Downloads only the necessary data tiles
Progress tracking - See exactly what's being downloaded
One-click loading - Buildings automatically added to your QGIS project

🚀 Quick Start
Prerequisites:

QGIS 3.x
QGIS Notebook Plugin by Qiusheng Wu

Installation:

Install the QGIS Notebook Plugin from QGIS Plugin Manager
Download MGBdownloader.ipynb from this repository
Open the notebook in QGIS Notebook Plugin
Zoom to your area of interest in QGIS
Run all cells sequentially

That's it! Buildings will download and appear on your map.
📖 How It Works

Captures your canvas extent and transforms coordinates to EPSG:4326
Generates QuadKeys for the map tiles covering your area (zoom level 9)
Downloads building data from Microsoft's Global Buildings dataset
Filters buildings to your exact extent
Saves as GeoJSON and loads directly into QGIS

🙏 Acknowledgments
Special thanks to:

Qiusheng Wu (@giswqs) for creating the amazing QGIS Notebook Plugin that makes this workflow possible
Microsoft for releasing this incredible open dataset
The open source geospatial community for tools like GeoPandas, Shapely, and Mercantile

📚 Resources

Microsoft Global Buildings Dataset
QGIS Notebook Plugin
Dataset Links CSV

🐛 Troubleshooting
Getting 0 buildings?

Ensure you're zoomed to a populated area
Check that your area is covered in the Microsoft Global Buildings regions. Try with London or wellknown area
Try a test location like Seattle (-122.33, -122.25, 47.60, 47.65)
Verify your canvas is in a valid CRS

📄 License
This notebook is released under MIT License. The Microsoft Global Buildings dataset is licensed under ODbL.

🌟 Show Your Support
If this tool helped you, please star the repository and share it with others!
