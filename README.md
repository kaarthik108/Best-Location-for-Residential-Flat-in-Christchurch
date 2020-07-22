# Best-Location-for-Residential-Flat-in-Christchurch
The main aim of this project is to determine the best location in Christchurch city to build a residential flat or any business development based on the airport noise factor and away from the main roads in order to avoid busy traffic also where the place Is situated in a clean air zone with priority given to greenfield areas.

# Introduction
Christchurch one of the largest cities in New Zealand is located on the east coast of New Zealand’s South Island with a population of 350,000 known as the Garden city with outstanding leisure and wide range of other facilities. Christchurch Airport is one of the busiest operating networks with approximately 200,000 flights per year which serves as the base for both NZ and America flights to the Antarctic which now had developed 50dBA Ldn airport noise contour, leaving the city with noise difficulties with the developing traffic in roads and pollution as a result. Analysis was done keeping the constraints in mind and determining the best location for a future residential plant to live in a less polluted area with more green space and away from all those noise factors. As this would be highly beneficial for people who wants to live in a calm and peaceful location and supporting the health and well-being of our communities

# Dataset and Resource
Christchurch map was clipped from the New Zealand map data which was taken from stats nz. The roads data was also clipped from the entire New Zealand roads which was taken from Linz. Land Use Recovery Plan - Greenfield Priority Areas data was downloaded from Canterbury maps. Additionally, clean air zone data was also collected from the Canterbury maps open data.

# Method (Spatial Analysis)
• All the necessary data (Airport noise contour, Clean air zone, Greenfield priority areas, Major roads) was loaded into the ArcMap for the Spatial Analysis.
• First and foremost, the Christchurch map was clipped from the New Zealand map to start with the analysis. To make sure proper clip, the city boundary data was used. Then the Major roads data was clipped from the country road map to show only for Christchurch city.
• We then create a buffer zone for the airport contour with a distance of 3 km to make sure the decibels are at lower to zero peak as shown in Fig.01.
• Another Buffer was created with distance up to 500 meters for the major road (Halswell Road) that is near to the greenfield towards south east Halswell as this area being a possible location that intersects with the Greenfield priority areas and away from the airport noise contour which is then exported as ‘Halswellroadbuffer’.
• Here we do Union for the Airport noise contour, Major road and the greenfield to assign values for suitable and non-suitable areas.
• We edit the attribute table of the airport contour by adding a field ‘Priority’ with type as short integer. For the buffer distance of both airport contour ‘3km’ and major road ‘500m’ the value ‘0’ is assigned as these are not suitable areas. While for rest of the areas value ‘1’ is assigned as they become suitable areas.
• Color code was given to areas to differentiate suitable and non-suitable areas from the symbology tab of the ‘Suitable site’ layer from the table of contents.
• We could observe from Fig.02 the intersection areas i.e. suitable areas with clean air zone and Greenfield areas which is away from noise contour and major roads to be in the south east part of Christchurch.

# Limitations
• Since most of the Land use greenfield priority areas where situated inside the Airport noise buffer contour and close to the major roads, it was hard to do the analysis leaving behind major portion of the Greenfields.
• Unable to track the major roads as they don’t have specific values in attributes table and hence had to manually select a major road away from the noise buffer which is close to Greenfields to eradicate non suitable areas.

# Conclusion
After Analysis, we could observe that areas Sparks road ‘Halswell’, ‘Wigram’, ‘Awatea’, ‘South Halswell’, ‘Marshlands’, ‘papanui’ are the best location in Christchurch to build future residential site for a peaceful and healthy living supporting the well-being of our communities eradicating the constraint factors.


