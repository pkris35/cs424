#### Task 3:Spatial visualization
#### UHF42 Boiler Emissions Choropleth

This choropleth map displays the average boiler emissions throughout the UHF42 regions in New York City. The regions are shaded according to their emission intensity, with darker colors means higher values. The map has been reprojected to Web Mercator for uniformity, and tooltips display the name of each region and the precise emission level when hovered over. This map effectively gives us as a clear spatial map for identifying patterns of emission concentration across UHF42 healthcare zones.

![UHF42 Boiler Emissions Choropleth](images3/BoilerEmissions.png)

#### UHF42 Annual Vehicle Miles Traveled 

This choropleth map illustrates the average boiler emissions in the UHF42 regions of New York City. The regions are colored based on their emission intensity, where darker shades means higher emissions. The map has been reprojected to Web Mercator for consistentcy, and tooltips give the region name and specific emission levels when hovered over. This representation effectively provides us a clear visualization for analyzing emission concentration trends across the NYC.

![UHF42 Annual Vehicle Miles Traveled](images3/AnnualVehiclesTraveled.png)

#### NYC Hospitalization Rates by UHF42 Region (Dropdown)

This choropleth map illustrates the hospitalization rates per 100,000 residents within the UHF42 areas of NYC. we can utilize a dropdown menu to select between various health conditions, such as respiratory and cardiovascular diseases for both adults and children. The map has a color gradient to indicate the intensity of hospitalizations, and tooltips give region-specific values and context for different population groups when hovering over the map.

![NYC Hospitalization Rates by UHF42 Region](images3/Hospitalizationrates.png)

#### Community District (CD) and UHF42 Air Pollutants (Horizontal Comparison)

This dual choropleth visualization illustrates the concentrations of pollutants (PM2.5, NO2, and O3) across two geographic levels: Community District (CD) and UHF42. Users can use dropdown menus to choose the pollutant they want to see for each map. This format gives straightforward spatial comparisons between the two levels of detail, allowing for insights into whether trends observed in fine (CD) data correspond with more granular data using (UHF42). Tooltips gives the information on the type of pollutant, the name of the district or region, and the concentration values.

![Community District (CD) and UHF42 Air Pollutants](images3/CDandUHF42Airpollutantshorizontalconcat.png)

#### Community District-Level Air Pollutants (PM2.5, NO2, and Ozone)

*Description*:  
This visualization combines two choropleth maps which are giving us the the spatial and temporal differences in air pollutants throughout NYC Community Districts (CD). It has an interactive faceted map for PM2.5 and NO2 with a time slider, along with a distinct seasonal map for Ozone accessed through a dropdown menu. This gives users to analyze pollutant distributions over various years and seasons while maintaining temporal accuracy across different types of pollutants.

*Attributes Being Visualized*

*Choropleth Map 1 – Annual Pollutants (PM2.5 and NO2)*  
- *Color Fill*: Districts are shaded based on the concentration of the selected pollutant; darker shades represent higher pollution.  
- *X-Axis (Facet)*: Pollutant name (PM2.5 or NO2).  
- *Slider*: Filters the map by year (2014–2022).  
- *Tooltip*: Shows Community District name, pollutant, and pollutant value.

*Choropleth Map 2 – Ozone (O3)*  
- *Color Fill*: Seasonal Ozone concentration, displayed using a consistent color scale.  
- *Dropdown*: Allows selection of the season (e.g., “Summer 2016”, “Fall 2017”).  
- *Tooltip*: Displays selected season, pollutant level, and district name.

*Interaction Mechanisms and Methods*  
*Mechanisms*:  
- Dropdown selection  
- Year slider  
- Hover tooltip  

*Methods*:  
- The PM2.5 and NO2 map employs *facet encoding* along with a *time slider* to enable users to select specific years, facilitating the exploration of yearly variations in pollutants by district and type.  
- Ozone (O3) data was only available with seasonal figures (like “Summer 2017”) and not as annual averages, which made it unsuitable for the time slider applied to PM2.5 and NO2. To resolve this issue, we created a *different choropleth* for O3 that has a dropdown filter for choice.  
- This design decision maintains clarity in temporal comparisons and avoids mistakes arising from differing time formats.  

By dividing these views while maintaining a good encoding and layout, we can see temporal-spatial trends in pollutants in an organized and understandable way.

*PM2.5 & NO2 with Time Slider:*  
![CD Annual PM2.5 and NO2](images3/CDPM2.5NO2withtime.gif)

*Ozone Seasonal Dropdown:*  
![CD Seasonal Ozone](images3/CDO3withtime.gif)


## Task 4: Linked Spatial Visualization  
**[View Visualization](https://pkris35.github.io/cs424/linked_spatial_visualization_final1.html)**

### The attributes being visualized
- Spatial: UHF42 regions of New York City.
- Quantitative: Average boiler emissions per region.
- Categorical: Borough each region belongs to.
- Temporal: Time Period of emissions data.

This visualization was designed to explore geographic and temporal patterns in emissions. By combining spatial and non-spatial views, users can observe how emissions vary across regions and over time, and how these trends differ between boroughs.

### interaction techniques and methods implemented
- Region selection via click filters the scatter plot and bar chart.
- Hovering over a region highlights it with a border.
- Selecting a borough from the bar chart filters the map and scatter plot.
- Opacity encoding visually separates selected from non-selected elements.

### The design 
- Borough-based color encoding was applied consistently to both the scatter and bar chart.
- A choropleth map was chosen for spatial representation.
- Layout: the map is placed on the left; scatter and bar charts are stacked on the right for vertical comparison.

### The experimentation process using Vega-Lite
We initially used a quantitative color scale for emissions but switched to borough-based categorical colors for consistency. 



