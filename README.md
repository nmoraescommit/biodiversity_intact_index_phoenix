# Biodiversity Intactness Index Differences in Phoenix, Arizona (2017 - 2020)

## About
Rapid and significant urban land use development of Maricopa County (metropolitan Phoenix, Arizona) has impacted the biodiversity in the area. This project seeks to assess and visualize any BII loss in Phoenix, over the years of 2017 to 2020.

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
  
 ## Data Access
 - The 2017 and 2020 BII (Biodiversity Intactness Index) Time Series data comes from the Microsoft Planetary Computer STAC catalog. I have also use the Census Bureau County Subdivisions shapefiles to retreive the Phoenix subdivision polyogon. Arizona. The data has been put into the .gitignore.
 
### References:
- Microsoft Planetary Computer. (n.d.). IO biodiversity dataset. Retrieved December 3, 2024, from https://planetarycomputer.microsoft.com/dataset/io-biodiversity\n"
- U.S. Census Bureau. (2024). Arizona county subdivisions: tl_2024_04_cousub.shp [Shapefile dataset]. Retrieved from https://www.census.gov/cgi-bin/geo/shapefiles/index.php?year=2024&layergroup=County+Subdivisions \n",