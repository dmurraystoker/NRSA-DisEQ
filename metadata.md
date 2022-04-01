Metadata for “Environmental filtering and habitat (mis)matching of riverine invertebrate metacommunities”
================
Murray-Stoker, D. K. M. Murray-Stoker, F. P. Kong, and F. Amanat.

# NRSA-DisEQ

Metadata associated with the manuscript:

Murray-Stoker, D. K. M. Murray-Stoker, F. P. Kong, and F. Amanat. Environmental filtering and habitat (mis)matching of riverine invertebrate metacommunities.

# Metadata


## Invertebrate Data (Raw)

### Raw Invertebrate Data

file = EPA-NRSA\_0809-invertebrates-RAW.csv

Raw invertebrate data collected by the USEPA. Data are in a long format. Please note that we only retain the following columns from the raw data to help with data processing. Data were collated from [nrsa0809bentctsmet.txt](https://www.epa.gov/sites/production/files/2016-11/nrsa0809bentctsmet.txt).

| Variable      | Description                                               |
|:--------------|:----------------------------------------------------------|
| UID           | Unique site visit identifier assigned by the USEPA        |
| SITE\_ID      | Site identification code assigned by the USEPA            |
| DATE\_COL     | Date of field collection                                  |
| TARGET\_TAXON | Taxonmic name at target hierarchical taxonomic level      |
| TOTAL300      | Total of a given taxon out of a subsample of300 organisms |


### Filtered Invertebrate Data

file = NRSA-invertebrates-rel\_abund.25.csv

Site-by-taxa abundance matrix of all taxa with a relative abundance above 0.25%.

Each column represents a taxon, and values represent the abundance of that taxon at the site. The relative abundance data was generated after processing the raw invertebrate data.




## Trait Matrices


### Categorical

file = taxa\_by\_traits-categorical.csv

Taxa-by-trait matrix where each taxon is given a trait modality for each of the functional traits. This taxa-by-trait categorical matrix was used for calculating functional trait diversity. Trait descriptions follow [Poff et al. 2006](https://www.journals.uchicago.edu/doi/full/10.1899/0887-3593%282006%29025%5B0730%3AFTNONA%5D2.0.CO%3B2).

| Variable           | Description                                                                 |
|:-------------------|:----------------------------------------------------------------------------|
| taxon              | Name (primarily genus) of the respective taxon                              |
| dispersal          | Adult female dispersal distance; high = > 1 km, low = < 1 km                |
| flying.strength    | Adult flying strength; none = no flying ability, weak, or strong            |
| size               | Size at maturity; small = < 9 mm, medium = 9-16 mm, large = > 16 mm         |
| rheophily          | Rheophilic/flow preference; depositional, depositional_erosional, erosional |
| thermal.preference | Thermal preference; cold = cool stenothermal/cool eurythermal, cool_warm = cool/warm eurythermal, warm = warm eurythermal    |
| FFG                | Functional feeding group/trophic habit; CG = collector-gatherer, CF = collector-filterer, HB = herbivore, PR = predator      |
| tolerance          | Tolerance to polution; sensitive, medium, or tolterant                      |


### Binary

file = taxa\_by\_traits-binary.csv

Taxa-by-traits matrix where each cell represents the presence (1) or absence (0) of a given functional trait. The binary trait matrix was used to calculate functional trait abundances.

| Variable               | Description                                                                |
|:-----------------------|:---------------------------------------------------------------------------|
| taxon                  | Name (primarily genus) of the respective taxon                             |
| dispersal.low          | Adult female dispersal distance < 1 km                                     |
| dispersal.high         | Adult female dispersal distance > 1 km                                     |
| flying.strength.none   | Adult flying strength = none; no adult flying stage                        |
| flying.strength.weak   | Adult flying strength = weak; unable to fly in light breeze                |
| flying.strength.strong | Adult flying strength = strong                                             |
| size.small             | Size at maturity = < 9 mm                                                  |
| size.medium            | Size at maturity = 9-16 mm                                                 |
| size.large             | Size at maturity = > 16 mm                                                 |
| depositional           | Rheophilic preference for only depositional areas                          |
| depositional.erosional | Rheophilic preference for both depositional and erosional areas            |
| erosional              | Rheophilic preference for erosional areas                                  |
| cold                   | Thermal preference for cold stenothermal/cool eurythermal water            |
| cool.warm              | Thermal preference for wool/warm eurythermal water                         |
| warm                   | Thermal preference for warm eurythermal water                              |
| CG                     | Collector-gather functional feeding group                                  |
| CF                     | Collector-filterer functional feeding group                                |
| HB                     | Herbivore functional feeding group                                         |
| PR                     | Predator functional feeding group                                          |
| sensitive              | Sensitive pollution tolerance                                              |
| medium                 | Intermediate pollution tolerance                                           |
| tolerant               | High pollution tolerance                                                   |




## Environmental Data


### Landscape Data

file = NRSA-landscape.csv

Landscape data for the sites survey during the NRSA 2008-2009. Descriptions are derived from the metadata provided by the USEPA for each data file. Original variable names are provided in square brackets. Data were collated from [land.csv](https://www.epa.gov/sites/default/files/2015-09/land.csv).

| Variable              | Description                                                                                                             |
|:----------------------|:------------------------------------------------------------------------------------------------------------------------|
| UID                   | Unique site visit ID [UID]                                                                                              |
| mean.annual.flow      | Mean annual flow in cubic feet per second (cfs) at bottom of flowline as computed by Unit Runoff Method [MAFLOWU]       |
| dam.count             | Count of dams located within NHDPlus 10 km navigated subcatchment [NHD10_DAMS_CNT]                                      |
| dam.density           | Density of dams located within NHDPlus 10 km navigated subcatchment [NHD10_DAMS_DEN]                                    |
| basin.area            | Area of NHDPlus navigated cumulative basin in square kilometers [NHDWAT_AREA_SQKM]                                      |
| max.basin.elevation   | Maximum elevation value in meters (NED 30m resolution) within NHDPlus navigated cumulative basin [NHDWAT_NEDELEV_MAX]   |
| mean.basin.elevation  | Mean elevation value in meters (NED 30m resolution) within NHDPlus navigated cumulative basin [NHDWAT_ELEV]             |
| min.basin.elevation   | Minimum elevation value in meters (NED 30m resolution) within NHDPlus navigated cumulative basin [NHDWAT_NEDELEV_MIN]   |
| range.basin.elevation | Range of elevation values in meters (NED 30m resolution) within NHDPlus navigated cumulative basin [NHDWAT_NEDELEV_RANGE]   |
| pct.canopy.cover      | Mean percent tree canopy (NLCD2001 tree canopy) within NHDPlus navigated cumulative basin [NHDWAT_PCT_CANOPY]               |
| pct.ISC               | Mean percent impervious surface (NLCD2006 Impervious Surface) within NHDPlus navigated cumulative basin [NHDWAT_PCT_IMPERV] |
| tmax.annual           | Average maximum annual temperature in degrees Celsius (PRISM 1997-2000) at the sample site [TMAX_ANN]                   |
| tmax.july             | Average maximum July temperature in degrees Celsius (PRISM 1997-2000) at the sample site [TMAX_JULY]                    |
| tmin.annual           | Average minimum annual temperature in degrees Celsius (PRISM 1997-2000) at the sample site [TMIN_ANN]                   |
| tmin.july             | Average minimum July temperature in degrees Celsius (PRISM 1997-2000) at the sample site [TMIN_JULY]                    |
| pct.ag                | % of NHDPlus navigated cumulative basin area classified as agriculture in NLCD                                          |
| pct.urb               | % of NHDPlus navigated cumulative basin area classified as either residential, commercial, or developed in NLCD         |
| pct.for               | % of NHDPlus navigated cumulative basin area classified as forest in NLCD                                               |
| pct.wet               | % of NHDPlus navigated cumulative basin area classified as wetland in NLCD                                              |
| pct.shrub             | % of NHDPlus navigated cumulative basin area classified as shrub or grassland in NLCD                                   |



### Physical Habitat Data

file = NRSA-physical\_habitat.csv

Physical habitat data for the sites survey during the NRSA 2008-2009. Descriptions are derived from the metadata provided by the USEPA for each data file. Original variable names are provided in square brackets. Data collated from [phabmet.csv](https://www.epa.gov/sites/default/files/2015-09/phabmed.csv).

| Variable         | Description                                                                      |
|:-----------------|:---------------------------------------------------------------------------------|
| UID              | Unique site visit ID [UID] |
| site.ID          | Site identification code [SITE_ID] |
| site.lat         | X-site GPS latitude decimal degrees [XLAT_DD] |
| site.long        | X-site GPS longitude decimal degrees [XLON_DD] |
| strahler.order   | Strahler stream order from RF3 stream data |
| ecoregion        | NARS 9-level reporting region (2015), based on aggregated Omernik Level III ecoregions: CPL = Coastal Plains; NAP = Northern Appalachians; NPL = Northern Plains; SAP = Southern Appalachians; SPL  = Southern Plains; TPL = Temperate Plains; UMW = Upper Midwest; WMT = Western Mountains; XER = Xeric West [AGGR_ECO9_2015] |
| HUC8             | 8-digit HUC catalog unit number [HUC8] |
| reach.length     | Sample reach length (m) [REACHLEN] |
| bed.stability    | log10(Streambed Critical Diameter-at Bankfull - mm) [LDMB_BW5] |
| pct.bedrock      | Bed surface % bedrock [PCT_BDRK] |
| pct.bigrock      | Bed surface % larger than gravel (64mm) [PCT_BIGR] |
| pct.hardpan      | Bed surface % hardpan [PCT_HP] |
| pct.fine         | Bed surface % fines < 0.06mm [PCT_FN] |
| pct.sand         | Bed surface percent sand or smaller (< 2.0mm) [PCT_SAFN] |
| pct.fine.gravel  | Bed surface fine gravel or smaller (< 16mm) [PCT_SFGF] |
| pct.coarse.gravel | Bed surface coarse gravel or smaller (< 64mm) [PCT_SFG] |
| pct.riffle       | Percent fast water habitat [PCT_FAST] |
| pct.pool         | Percent of reach with pool or glide habitat [PCT_SLOW] |
| mean.thalweg.depth | Mean thalweg depth (cm), converted from raw data in m [XDEPTH_CM] |
| mean.width       | Mean wetted width (m) [XWIDTH] |
| sinuosity        | Sinuosity of sample reach [SINU] |
| LWD.reach        | Wood volume (m3) per 100m channel [LWDEQVOLM100] |
| embeddedness     | Mean streambed embeddedness (%) [EMBED] |
| ALG.cover        | Filamentous algae Mean areal cover [XFC_ALG] |
| AQM.cover        | Aquatic macrophyte mean areal cover [XFC_AQM] |
| LWD.cover        | Large woody debris areal cover [XFC_LWD] |
| NAT.cover        | Sum of non-anthropogenic areal cover types [XFC_NAT] |



### Water Chemistry Data

file = NRSA-water\_chemistry.csv

Water chemistry data for the sites survey during the NRSA 2008-2009. Descriptions are derived from the metadata provided by the USEPA for each data file. Original variable names are provided in square brackets. Data were collated from [chem.csv](https://www.epa.gov/sites/default/files/2015-09/chem.csv).

| Variable  | Description                                         |
|:----------|:----------------------------------------------------|
| UID       | Unique site visit ID [UID]                          |
| Al        | Total dissolved aluminum mg/L [AL]                  |
| ANC       | Acid neutralizing capacity ueq/L [ANC]              |
| Ca        | Calcium mg/L [CA]                                   |
| Cl        | Chloride mg/L [CL]                                  |
| cond      | Specific conductance μS/cm [COND]                   |
| DOC       | Dissolved organic carbon mg/L [DOC]                 |
| K         | Potassium mg/L [K]                                  |
| Mg        | Magnesium mg/L [MG]                                 |
| sodium    | Sodium mg/L [SODIUM]                                |
| NH4       | Ammonia as nitrogen mg/L [NH4]                      |
| NO2       | Nitrite as nitrogen mg N/L [NO2]                    |
| NO3       | Nitrate as nitrogen mg N/L [NO3]                    |
| total.N   | Total nitrogen μg/L [NTL]                           |
| pH.lab    | Laboratory measured pH [PHLAB]                      |
| total.P   | Total phosphorous μg/L [PTL]                        |
| SiO2      | Silica mg/L [SIO2]                                  |
| SO4       | Sulfate mg/L [SO4]                                  |
| TSS       | Total suspended solids mg/L [TSS]                   |
| turb      | Turbity NTU [TURB]                                  |






