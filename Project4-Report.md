# De-identify Health Data for Visualization and Sharing Report
Rahel Worku

There are challenges when it comes to mapping health data while maintaining
confidentiality. With health data, there are links to each of the individuals where the data
came from and includes protected individual health information. As mentioned by Paul
Zandbergen in his article on ensuring confidentiality of health data, the health-related data
will contain geographic identifiers of its participants (Zandbergen, 2014). While this
geodata is beneficial in spatial analysis, it brings up challenges in maintain confidentiality
when displaying that data. There are privacy risks of individuals getting identified through
their health records and must be thoroughly masked to ensure privacy is upheld for
individuals. Otherwise, this would lead to an invasion of privacy for patients and legal
issues of data handling. HIPAA (Health Insurance Portability and Accountability Act) was
formed as a way of setting down strict guidelines when it comes to protecting patient
information. This goal of this act is to make sure individuals can’t be identified or
associated through their spatial data. This report goes over diSerent methods to de-
identifying data from its individuals to ensure protected information is safe, while still
creating helpful visualizations.

### Legal context of de-identification
HIPAA was made to enforce guidelines to de-identifying health data to ensure
people couldn’t be re-identified through just the data. Two methods of de-identification
include Safe Harbor and Expert Determination. Safe Harbor requires you to remove 18
specific identifiers from the dataset which includes the precise geospatial data of its
individuals. Expert Determinization requires the user who is knowledgeable to modify the
data enough to a point of reducing re-identification. Safe Harbor is less helpful than Expert
Determinization since it reduces data below the state level which puts a limit to the spatial
analysis you could do. Expert Determination though reduces the privacy risks of re-
identification and keeps the data useful for analysis.

### Map-based visualizations
The techniques used for map-based visualizations included heat maps and point
clustering. The heat maps represented the density of data in certain areas without
revealing specific geolocations of each point. The point clustering grouped data points of
individuals into clusters based on their proximity to each other. The strengths of both heat
maps and point clustering is that they can communicate the spatial distribution of data
without showing the exact locations of individuals. You can still interpret the data with
these visualizations and make sure specific individuals aren’t being pinpointed or exposed.
A weakness with these maps is when zoomed out a lot, the heat map and clusters turn into
large groupings that aren’t as eSective for analysis. Another weakness is that when zoomed
in greatly, you could possibly see individual points in the point cluster map which would
expose individual information.
### Small-cell suppression
The techniques used for small-cell suppression were hot spot analysis and
tessellation. The hotspot analysis tool showed the significant clusters of high and low
values of individuals in an area. Tessellation or Hexbins were used to aggregate data into
‘hexagon’ shapes to keep pinpoint geolocations of individuals hidden still. The strengths of
these techniques are how they identify spatial trends in the data without showing detailed
information of the data of people. Since the Hexbins could be modified so that areas with
low cases are not identifiable and instead puts focus on the locations with high case
counts. Weaknesses of these techniques is how careful you must be when setting up the
parameters so that sensitive information isn’t shown by accident. An example of this could
be with hexagons with very low case counts not being properly hidden which would lead to
re-identification.
### Generalization and aggregation
The techniques of generalization and aggregation were summarizing by zip
code/year, rounded coordinates, and merging adjacent zip codes. The summarization
technique groups data together by zip code and year and can be used to count cases within
zip codes for any year. The coordinate rounding gets rid of point data by moving cases to a
less precise location since the coordinates of each point is essentially rounded down.
Merging adjacent zip codes will merge the cases in a specific zip code to an adjacent zip
code if it contains too few cases and ensures individual cases can’t be identified. The
strengths of these techniques are how cases are managed to ensure there aren’t zip codes
with too few cases. There will still be enough spatial information shown in terms of patterns
in the data while hiding precise locations. The summarizing by zip code and year also helps
in comparing data patterns year by year for general patterns. Weaknesses include zip code
boundaries not reflecting meaningful demographic data patterns since how they were
chosen doesn’t have anything to do with representing the community or health patterns.
Merging zip codes or rounding coordinates have weaknesses where smaller local patterns
in the data would get lost after merging and rounding.

### References
Zandbergen, P.A., 2014. Ensuring Confidentiality of Geocoded Health Data: Assessing
Geographic Masking Strategies for Individual-Level Data. Advances in Medicine
2014, 1–14. https://doi.org/10.1155/2014/567049

Tutorial authors: Jared Shoultz, Este Geraghty, Paul McBride

Fictitious data: ESRI
