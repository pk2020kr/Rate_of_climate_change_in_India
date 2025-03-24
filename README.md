# Rate of Climate Change in India: Temperature and Rainfall Analysis


## Description
This project analyzes historical climate data in India, focusing on maximum temperatures, minimum temperatures, and rainfall patterns from 1951 to 2024. The analysis aims to investigate climate trends and changes over time, providing insights into the rate and nature of climate change across different regions of India.

## Structure
The project consists of the following main components:

1. **Data Collection and Processing**: Loading and processing of gridded temperature and rainfall data from the Indian Meteorological Department (IMD)
2. **Temporal Analysis**: Examination of temperature and rainfall trends over time
3. **Spatial Analysis**: Geographic visualization of climate patterns across India
4. **Statistical Analysis**: Quantitative assessment of climate change metrics
5. **Visualization**: Generation of plots and maps to illustrate key findings

## Requirements
- Python 3.11
- imdlib
- geopandas
- numpy
- pandas
- matplotlib
- seaborn
- prophet

## Data Description
The project utilizes three main types of climate data:
- **tmin/**: Directory containing minimum temperature gridded data files (GRD format) from 1951-2024
- **tmax/**: Directory containing maximum temperature gridded data files (GRD format) from 1951-2024
- **rain/**: Directory containing rainfall gridded data files (GRD format) from 1951-2024
- **co_test/**: Sample CSV extracts for specific coordinates Ex_(26.60°N, 80.84°E)

The GRD files are Indian Meteorological Department (IMD) gridded data containing daily climate observations. Each file represents one year of data.

## Installation Instructions
To set up your environment and install the required dependencies:

1. install all libyaries
# Download from IMD in .GRD format (Around 2GB)
#data = imd.get_data('tmax', 2017, 2024,'yearwise') #(variable, start_yr, end_yr, fn_format, file_dir)
#data = imd.get_data('tmin', 2017, 2024,'yearwise') #(variable, start_yr, end_yr, fn_format, file_dir)
#data = imd.get_data('rain',2017, 2024,'yearwise') #(variable, start_yr, end_yr, fn_format, file_dir)


2. Run the cells sequentially to:
   - Load temperature and rainfall data
   - Process and analyze the data
   - Generate visualizations
   - Examine climate change trends

3. The notebook can be modified to analyze specific regions or time periods by adjusting parameters in the data loading cells.

4. To select specific coordinates for analysis:
   - Use the NASA POWER Data Access Viewer (https://power.larc.nasa.gov/data-access-viewer/) to identify desired latitude and longitude
   - Modify the coordinate parameters in the notebook accordingly

## Examples
The analysis provides several key outputs:
- Time series plots showing temperature and rainfall trends
- Spatial maps visualizing climate patterns across India
- Statistical charts quantifying the rate of climate change
- Seasonal analysis of temperature and precipitation changes

## Output Explanation
The notebook generates various visualizations and analysis results:
- Long-term trends in maximum and minimum temperatures across India
- Changes in rainfall patterns and intensity
- Identification of regions experiencing more rapid climate change
- Seasonal variation in climate metrics
- Statistical significance of observed changes

## Data Sources
This project utilizes data from the following sources:

1. **India Meteorological Department (IMD) Gridded Dataset**
   - Daily gridded rainfall and temperature (minimum and maximum) data
   - Temporal coverage: 1951-01-01 to 2024-12-31
   - Accessed using the imdlib Python package
   - Documentation: https://imdlib.readthedocs.io/en/latest/Usage.html#reading-imd-datasets

2. **Coordinate Selection Tool**
   - NASA POWER Data Access Viewer for selecting specific lat/lon coordinates
   - Tool URL: https://power.larc.nasa.gov/data-access-viewer/

The imdlib package is capable of downloading gridded rainfall and temperature data directly, making it convenient for climate data analysis in India.

## Limitations
- The analysis is constrained by the spatial and temporal resolution of the IMD gridded data

## References
- Indian Meteorological Department (IMD) gridded data documentation
- imdlib Python package: https://imdlib.readthedocs.io/
- NASA POWER Data Access Viewer: https://power.larc.nasa.gov/data-access-viewer/
- Climate change assessment methodologies

*Note: This README provides an overview of the project structure and functionality. For detailed methods and findings, please refer to the notebook itself.* 
