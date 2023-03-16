[![NSF-1948997](https://img.shields.io/badge/NSF-1948997-blue.svg)](https://nsf.gov/awardsearch/showAward?AWD_ID=1948997) [![NSF-1948994](https://img.shields.io/badge/NSF-1948994-blue.svg)](https://nsf.gov/awardsearch/showAward?AWD_ID=1948994) [![NSF-1948857](https://img.shields.io/badge/NSF-1948857-blue.svg)](https://nsf.gov/awardsearch/showAward?AWD_ID=1948857)

# Read and visualize point cloud and raster topography data using Matlab
Chelsea Scott: cpscott1@asu.edu(corresponding author)

This repository contains code to read and visualize point cloud and raster topography data in Matlab. There are three scripts: 

- point_cloud_lasdata.m: Use this script and the Mathwork's file exchange lasdata (https://www.mathworks.com/matlabcentral/fileexchange/48073-lasdata) to load point cloud topography into Matlab. This is recommended if you do not have access to the Matlab's lidar toolbox. The point cloud must be a .las file. 

- point_cloud_matlab.m: Use this script with Matlab's Lidar Toolbox (https://www.mathworks.com/products/lidar.html) to load and visualize lidar point cloud by attribute, for example RBG color (when available) and classification. 

- read_visualize_raster.m: Use this script to load in and visualize raster datasets such as digital elevation models. Also, use this script to make hillshades (requires Mathwork's file exchange: https://www.mathworks.com/matlabcentral/fileexchange/14863-hillshade) and to make gradient maps (requires Mathwork's file exchange: https://www.mathworks.com/matlabcentral/fileexchange/18655-gradient8?s_tid=srchtitle). 

There are two ways to obtain the data: 

1) Download the topography data files (pre-processed via OpenTopography):

- Point cloud data in las format (for point_cloud_lasdata.m):
https://object.cloud.sdsc.edu/v1/AUTH_opentopography/www/education/MatlabTopo/Utah_state_capitol.las

- Point cloud data in laz format (for point_cloud_matlab.m):
https://object.cloud.sdsc.edu/v1/AUTH_opentopography/www/education/MatlabTopo/Utah_state_capitol.laz

- Geotif (for read_visualize_raster.m):
https://object.cloud.sdsc.edu/v1/AUTH_opentopography/www/education/MatlabTopo/Utah_grabens.tif

2) Generate and download the point cloud (.las or .laz files) or DEM (.tif files) data via the OpenTopography portal on demand. Note that in the Matlab scripts, the topography data files from OpenTopography are renamed with local significance. 

- Salt Lake City(https://doi.org/10.5069/G9TH8JNQ): 
https://portal.opentopography.org/lidarDataset?opentopoID=OTLAS.122014.26912.1&minX=-111.88989256858865&minY=40.77602500627361&maxX=-111.88666950298132&maxY=40.77977572159702

- Canyonlands National Park: (https://doi.org/10.5069/G9X34VNQ): 
https://portal.opentopography.org/lidarDataset?opentopoID=OTLAS.072020.6341.1&minX=-109.92892645717178&minY=38.10798288429967&maxX=-109.90619966646437&maxY=38.12079524373647
