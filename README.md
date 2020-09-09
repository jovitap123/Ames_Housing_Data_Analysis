# Project 2 - Ames Housing Data and Kaggle Challenge

## Problem Statement

A leading real estate company, Zillow, wants to develop a model to predict housing prices based on Ames housing data collected from 2006 to 2010. To test the final model, a dataset of houses with unknown sale prices is used to validate accuracy. An accurate house price predicting model is key to staying ahead of other competitors like Redfin, Homesnap and NeighborhoodScout and attracting new customers to use the platform.

## Executive Summary

The following questions were answered using the finalized model:
- Which features appear to add the most value to a home?
- Which features hurt the value of a home the most?
- What are things that homeowners could improve in their homes to increase the value?
- What neighborhoods seem like they might be a good investment?
- Do you feel that this model will generalize to other cities? How could you revise your model to make it more universal OR what date would you need from another city to make a comparable model?

## Data Dictionary 

A data dictionary is created for quick reference of the column names
Source of information : http://jse.amstat.org/v19n3/decock/DataDocumentation.txt

|Feature|Type|Description|
|---|---|---|---|
|**Id**|*Discrete*|Identification number| 
|**PID**|*Nominal*|Parcel identification number - can be used with city web site for parcel review|
|**MS.SubClass**|*Nominal*| Identifies the type of dwelling involved in the sale|
|**MS.Zoning**|*Nominal*|Identifies the general zoning classification of the sale|
|**Lot.Frontage**|*Continuous*|Linear feet of street connected to property|
|**Lot.Area**|*Continuous*|Lot size in square feet|
|**Street**|*Nominal*|Type of road access to property|
|**Alley**|*Nominal*|Type of alley access to property|
|**Lot Shape**|*Ordinal*|General shape of property|
|**Land Contour**|*Nominal*|Flatness of the property|
|**Utilities**|*Ordinal*|Type of utilities available|
|**Lot Config**|*Nominal*|Lot Configuration|
|**Land Slope**|*Ordinal*|Slope of property|
|**Neighborhood**|*Nominal*|Physical locations within Ames city limits (map available)|
|**Condition 1**|*Nominal*|Proximity to various conditions|
|**Condition 2**|Nominal*|Proximity to various conditions (if more than one is present)|
|**Bldg Type**|*Nominal*|Type of dwelling|
|**House Style**|*Nominal*|Style of dwelling|
|**Overall Qual**|*Ordinal*|Rates the overall material and finish of the house|
|**Overall Cond**|*Ordinal*|Rates the overall condition of the house|
|**Year Built**|*Discrete*|Original construction date|
|**Year Remod Add**|*Discrete*|Remodel date (same as construction date if no remodeling or additions|
|**Roof Style**|*Nominal*|Type of roof|
|**Roof Matl**|*Nominal*|Roof material|
|**Exterior 1st**|*Nominal*|Exterior covering on house|
|**Exterior 2nd**|*Nominal*|Exterior covering on house (if more than one material)|
|**Mas Vnr Type**|*Nominal*|Masonry veneer type|
|**Mas Vnr Area**|*Continuous*|Masonry veneer area in square feet|
|**Exter Qual**|*Ordinal*|Evaluates the quality of the material on the exterior|
|**Exter Cond**|*Ordinal*|Evaluates the present condition of the material on the exterior|
|**Foundation**|*Nominal*|Type of foundation|
|**Bsmt Qual**|*Ordinal*|Evaluates the height of the basement|
|**Bsmt Cond**|*Ordinal*|Evaluates the general condition of the basement|
|**Bsmt Exposure**|*Ordinal*|Refers to walkout or garden level walls|
|**BsmtFin Type 1**|*Ordinal*|Rating of basement finished area|
|**BsmtFin SF 1**|*Continuous*|Type 1 finished square feet|
|**BsmtFin Type 2**|*Ordinal*|Rating of basement finished area (if multiple types)|
|**BsmtFin SF 2**|*Continuous*|Type 2 finished square feet|
|**Bsmt Unf SF**|*Continuous*|Unfinished square feet of basement area|
|**Total Bsmt SF**|*Continuous*|Total square feet of basement area|
|**Heating**|*Nominal*|Type of heating|
|**Heating QC**|*Ordinal*|Heating quality and condition|
|**Central Air**|*Nominal*|Central air conditioning|
|**Electrical**|*Ordinal*|Electrical system|
|**1st Flr SF**|*Continuous*|First Floor square feet|
|**2nd Flr SF**|*Continuous*|Second floor square feet|
|**Low Qual Fin SF**|*Continuous*|Low quality finished square feet (all floors)|
|**Gr Liv Area**|*Continuous*|Above grade (ground) living area square feet|
|**Bsmt Full Bath**|*Discrete*|Basement full bathrooms|
|**Bsmt Half Bath**|*Discrete*|Basement half bathrooms|
|**Full Bath**|*Discrete*|Full bathrooms above grade|
|**Half Bath**|*Discrete*|Half baths above grade|
|**Bedroom AbvGr**|*Discrete*|Bedrooms above grade (does NOT include basement bedrooms)|
|**Kitchen AbvGr**|*Discrete*|Kitchens above grade|
|**Kitchen Qual**|*Ordinal*|Kitchen quality|
|**TotRms AbvGrd**|*Discrete*|Total rooms above grade (does not include bathrooms)|
|**Functional**|*Ordinal*|Home functionality (Assume typical unless deductions are warranted)|
|**Fireplaces**|*Discrete*|Number of fireplaces|
|**Fireplace Qu**|*Ordinal*|Fireplace quality|
|**Garage Type**|*Nominal*|Garage location|
|**Garage Yr Blt**|*Discrete*|Year garage was built|
|**Garage Finish**|*Ordinal*| Interior finish of the garage|
|**Garage Cars**|*Discrete*|Size of garage in car capacity|
|**Garage Area**|*Continuous*|Size of garage in square feet|
|**Garage Qual**|*Ordinal*|Garage quality|
|**Garage Cond**|*Ordinal*|Garage condition|
|**Paved Drive**|*Ordinal*|Paved driveway|
|**Wood Deck SF**|*Continuous*|Wood deck area in square feet|
|**Open Porch SF**|*Continuous*|Open porch area in square feet|
|**Enclosed Porch**|*Continuous*|Enclosed porch area in square feet|
|**X3Ssn Porch**|*Continuous*|Three season porch area in square feet|
|**Screen Porch**|*Continuous*|Screen porch area in square feet|
|**Pool Area**|*Continuous*|Pool area in square feet|
|**Pool QC**|*Ordinal*|Pool quality|
|**Fence**|*Ordinal*|Fence quality|
|**Misc Feature**|*Nominal*|Miscellaneous feature not covered in other categories|
|**Misc Val**|*Continuous*|$Value of miscellaneous feature|
|**Mo Sold**|*Discrete*|Month Sold (MM)|
|**Yr Sold**|*Discrete*|Year Sold (YYYY)|
|**Sale Type**|*Nominal*|Type of sale|
|**Sale Condition**|*Nominal*|Condition of sale|
|**SalePrice**|*Continuous*|Sale price|


## Conclusions and Recommendations

This model would not general well with other cities as it was developed on data only from one city, Ames and over a relatively short period of time of four years. In addition, it also included sales from 2008 - 2009 when the Housing Crash took place and given that it a unique economic phase, it wouldn't represent trends over the rest of the years accurately. In order to reduce the significance of this phase, a larger amount of data over a longer period of time should be collected so the sale prices average out better.

It is a challenging endevour to develop a model that will generalize for more cities as a lot of other external factors influence housing prices as well like average income of the city, average age of the population of the city, availabilty of educational institutes like universities and colleges etc. However, the model definitely shows insight on key features that increase value of the house and those that are not significant.