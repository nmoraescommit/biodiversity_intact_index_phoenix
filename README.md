# Biodiversity Intactness Index Differences in Phoenix, Arizona (2017 - 2020)

## About
Rapid and significant urban land use development of Maricopa County (metropolitan Phoenix, Arizona) has impacted the biodiversity in the area. This project seeks to assess and visualize any BII loss in Phoenix, over the years of 2017 to 2020.

<img src="https://i0.wp.com/oncemoretotheshore.com/wp-content/uploads/2021/04/Camelback-Mountain_Phoenix_Robin-Catalano-travel-writer.jpg?w=1200&ssl=1" alt="Arizona Desert Scenery" width="700"/>

## Repository Structure

```bash
|── biodiversity_intact_index_phoenix
├── README.md
├── biodiversity_index_phoenix.ipynb 
└── .gitignore
   └── data
      ├── tl_2022_04_cousub.cpg
      ├── tl_2022_04_cousub.dbf
      ├── tl_2022_04_cousub.prj
      ├── tl_2022_04_cousub.shp
      ├── tl_2022_04_cousub.shp.ea.iso.xml
      ├── tl_2022_04_cousub.shp.iso.xml
      └── tl_2022_04_cousub.shx
```  
  
 ## Data Description and Access
 
 **1.Biodiversity Intactness Index (BII) Time Series**

Biodiversity intactness index data was accessed from [ Microsoft Planetary Computer STAC catalog](https://planetarycomputer.microsoft.com/dataset/io-biodiversity). I used the `pystac_client` API to access the `io-biodiversity` collection from the catalog, that intersected the area and time of relevance to this project. The datasets "estimate terrestrial Biodiversity Intactness as 100-meter gridded maps for the years 2017-2020". [(Microsoft Datasets| Biodiversity Intactness)](https://planetarycomputer.microsoft.com/dataset/io-biodiversity)

**2. Phoenix Subdivision Shapefile** 

Phoenix shapefile was dowloaded as a shapfilee from the [United States Census Bureau| TIGER/ Line Shapefiles](https://www.census.gov/cgi-bin/geo/shapefiles/index.php?year=2024&layergroup=Census+Tracts), and was saved to the data folder  To access, visit the link below and download the file `tl_2022_04_cousub.shp` to a data folder.
County subdivision census data from 2024 was used to filter to our area of interest. Data was downloaded as a shapefile and placed it into the data folder, where `os` was used to create an absolute filepath, and the `GeoPandas` package was used to read in the file via `gpd.read_file()`.

**3. Data Access**

All stored data required to run the `biodiv_index.ipynb` notebook is currently stored in the .gitignore in this repository. Currently, this data is only the Phoenix subdivision shapefiles.
 
### References:

- Microsoft Planetary Computer. (n.d.). IO biodiversity dataset. Retrieved December 3, 2024, from https://planetarycomputer.microsoft.com/dataset/io-biodiversity\n"
- U.S. Census Bureau. (2024). Arizona county subdivisions: tl_2024_04_cousub.shp [Shapefile dataset]. Retrieved from https://www.census.gov/cgi-bin/geo/shapefiles/index.php?year=2024&layergroup=County+Subdivisions \n",

## Acknowledgements

This repository was created as the final assignment for the graduate course EDS 220: Working with Environmental Datasets in the [Masters of Environmental Data Science (MEDS) program](https://bren.ucsb.edu/masters-programs/master-environmental-data-science), taught by [Dr. Carmen Galaz García](https://github.com/carmengg).