#### Task 3:Spatial visualization
#### UHF42 Boiler Emissions Choropleth

This choropleth map displays the average boiler emissions throughout the UHF42 regions in New York City. The regions are shaded according to their emission intensity, with darker colors indicating higher values. The map has been reprojected to Web Mercator for uniform rendering, and tooltips display the name of each region and the precise emission level when hovered over. This static map effectively serves as a clear spatial reference for identifying patterns of emission concentration across healthcare zones.

![UHF42 Boiler Emissions Choropleth](images3/BoilerEmissions.png)

#### UHF42 Annual Vehicle Miles Traveled 

This choropleth map illustrates the average boiler emissions in the UHF42 regions of New York City. The regions are colored based on their emission intensity, where darker shades signify higher emissions. The map has been reprojected to Web Mercator for consistent viewing, and tooltips provide the region name and specific emission levels when hovered over. This static representation effectively serves as a clear visual framework for analyzing emission concentration trends across healthcare areas.

![UHF42 Annual Vehicle Miles Traveled](images3/AnnualVehiclesTraveled.png)

#### NYC Hospitalization Rates by UHF42 Region (Dropdown)

This choropleth map illustrates the hospitalization rates per 100,000 residents within the UHF42 areas of NYC. Users can utilize a dropdown menu to toggle between various health conditions, such as respiratory and cardiovascular diseases for both adults and children. The map employs a color gradient to indicate the intensity of hospitalizations, and tooltips offer region-specific values and context for different population groups when hovering over the map.

![NYC Hospitalization Rates by UHF42 Region](images3/Hospitalizationrates.png)

#### Community District (CD) and UHF42 Air Pollutants (Horizontal Comparison)

This dual choropleth visualization illustrates the concentrations of pollutants (PM2.5, NO2, and O3) across two geographic levels: Community District (CD) and UHF42. Users can use dropdown menus to independently choose the pollutant of interest for each map. This format facilitates straightforward spatial comparisons between the two levels of detail, allowing for insights into whether trends observed in fine-scale (CD) data correspond with larger regional patterns (UHF42). Tooltips provide information on the type of pollutant, the name of the district or region, and the concentration values.

![Community District (CD) and UHF42 Air Pollutants](images3/CDandUHF42Airpollutantshorizontalconcat.png)

#### Community District-Level Air Pollutants (PM2.5, NO2, and Ozone)

*Description*:  
This visualization combines two choropleth maps aimed at illustrating the spatial and temporal differences in air pollutants throughout NYC Community Districts (CD). It features an interactive faceted map for PM2.5 and NO2 with a time slider, along with a distinct seasonal map for Ozone accessed through a dropdown menu. This arrangement enables users to analyze pollutant distributions over various years and seasons while maintaining temporal accuracy across different types of pollutants.

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
- Ozone (O3) data was only available with seasonal figures (like “Summer 2017”) and not as annual averages, which rendered it unsuitable for the time slider applied to PM2.5 and NO2. To resolve this issue, we created a *distinct choropleth* for O3 that incorporates a dropdown filter for seasonal choice.  
- This design decision maintains clarity in temporal comparisons and avoids misinterpretations arising from differing time formats.  

By distinguishing these views while maintaining a cohesive encoding and layout, users can investigate temporal-spatial trends among pollutants in an organized and understandable manner.

*GIF Demonstrations*

*PM2.5 & NO2 with Time Slider:*  
![CD Annual PM2.5 and NO2](images3/CDPM2.5NO2withtime.gif)

*Ozone Seasonal Dropdown:*  
![CD Seasonal Ozone](images3/CDO3withtime.gif)
