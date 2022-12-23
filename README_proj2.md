# Saving LGBT+ Youth in Iowa
## Author: Revathi Satkuna

## Problem Statement
A board member of an educational policy team for the state of California has entrusted the nonprofit you work at to build an LGBT+ youth center in the town of Ames, Iowa. They wish to build and foster a place for LGBT youth so that if there needed to be a place to flee, to get life-saving medical treatment, there would be a direct liaison between the LGBT youth in Iowa to California. Since this is a nonprofit and you want to save money on the building itself and allocate more resources towards the services you provide, how and where should you find your house?
## Datasets
### Provided Data
* [`train.csv`](./datasets/train.csv): Ames Housing Data Set ([source](https://www.kaggle.com/competitions/dsi-1010-regression-challenge/data) | 
* [`test.csv`](./datasets/test.csv): Generate Predictions with this DataSet based on Model Created ([source](https://www.kaggle.com/competitions/dsi-1010-regression-challenge/data) 
* [`sample_sub_reg.csv`](./datasets/sample_sub_reg.csv): Format of Sample Submission to Kaggle  ([source](https://www.kaggle.com/competitions/dsi-1010-regression-challenge/data) | 
### Generated Data
* [`Z_train.csv`](./datasets_f/Z_train.csv): Cleaned and scaled training data with predictor variables 
* [`Z_test.csv`](./datasets_f/Z_test.csv): Cleaned test data with predictor variables 
* [`y_train.csv`](./datasets_f/y_train.csv): Cleaned and scaled training data with target variable
* [`y_test.csv`](./datasets_f/y_test.csv): Cleaned test data with target variable 
* [`numZ_train.csv`](./datasets_f/numZ_train.csv): Cleaned and scaled training data for numerical (continuous and discrete) features with predictor variables  
* [`numZ_test.csv`](./datasets_f/numZ_test.csv): Cleaned test data for numerical (continuous and discrete) features with predictor variables 
* [`test.csv`](./datasets_f/test.csv): Test data to test models
* [`kagtest.csv`](./datasets_f/kag.csv): Test data to test models that I used just for the kaggle notebook

## Data Dictionary
|Feature|Type|Dataset|Description|
|---|---|---|---|
|id|float64|Z_train|Observation number|
|pid|float64|Z_train|Parcel identification number which can be used with city website for parcel review|
|ms_sub_class|float64|Z_train|Identifies the type of dwelling involved in the sale|
|lot_frontage|float64|Z_train|Linear feet of street connected to property|
|lot_area|float64|Z_train|Lot size in square feet|
|alley|float64|Z_train|Type of alley access to property|
|lot_shape|float64|Z_train|General shape of property|
|utilities|float64|Z_train|Type of utilities available|
|land_slope|float64|Z_train|Slope of property|
|overall_qual|float64|Z_train|Rates overall material and finish of the house|
|year_remod/add|float64|Z_train|Remodel date same as construction date if no remodeling or additions|
|mas_vnr_area|float64|Z_train|Masonry veneer area in square feet|
|exter_qual|float64|Z_train|Evaluates the quality of the material on the exterior|
|exter_cond|float64|Z_train|Evaluates the present condition of the material on the exterior|
|bsmt_qual|float64|Z_train|Evaluates the height of the basement|
|bsmt_cond|float64|Z_train|The average household income of a student's family per school district|
|bsmt_exposure|float64|Z_train|Refers to walkout or garden level walls|
|bsmt_fin_type_1|float64|Z_train|Rating of basement finished area|
|bsmt_fin_sf_1|float64|Z_train|Type 1 finished square feet|
|bsmt_fin_type_2|float64|Z_train|Rating of basement finished area if multiple types|
|bsmt_fin_sf_2|float64|Z_train|Type 2 finished square feet|
|bsmt_unf_sf|float64|Z_train|Unfinished square feet of basement area|
|total_bsmt_sf|float64|Z_train|Total square feet of basement area
|heating_qc|float64|Z_train|Heating quality and condition|
|electrical|float64|Z_train|Electrical system|
|1st_flr_sf|float64|Z_train|First floor square feet|
|2nd_flr_sf|float64|Z_train|Second floor square feet|
|low_qual_fin_sf|float64|Z_train|Low quality finished square feet for all floors|
|gr_liv_area|float64|Z_train|Above grade ground living area square feet|
|bsmt_full_bath|float64|Z_train|Basement full bathrooms|
|bsmt_half_bath|float64|Z_train|Basement half bathrooms|
|full_bath|float64|Z_train|Full bathrooms above grade|
|half_bath|float64|Z_train|Half bathrooms above grade|
|bedroom_abv_gr|float64|Z_train|Bedrooms above grade does not include basement bedrooms|
|kitchen_abv_gr|float64|Z_train|Kitchens above grade|
|kitchen_qual|float64|Z_train|Kitchen quality|
|tot_rms_abv_grd|float64|Z_train|Total rooms above grade does not include bathrooms|
|functional|float64|Z_train|Home functionality and assume typical unless deductions are warranted|
|fireplaces|float64|Z_train|Number of fireplaces|
|fireplace_qu|float64|Z_train|Fireplace quality|
|garage_yr_blt|float64|Z_train|Year garage was built|
|garage_finish|float64|Z_train|Interior finish of the garage|
|garage_cars|float64|Z_train|Size of garage in car capacity|
|garage_area|float64|Z_train|Size of garage in square feet|
|garage_qual|float64|Z_train|Garage quality|
|garage_cond|float64|Z_train|Garage condition|
|paved_drive|float64|Z_train|Paved driveway|
|wood_deck_sf|float64|Z_train|Wood deck area in square feet|
|open_porch_sf|float64|Z_train|Open porch area in square feet|
|enclosed_porch|float64|Z_train|Enclosed porch area in square feet|
|3ssn_porch|float64|Z_train|Three season porch area in square feet|
|screen_porch|float64|Z_train|Screen porch area in square feet|
|pool_area|float64|Z_train|Pool area in square feet|
|fence|float64|Z_train|Fence quality|
|misc_val|float64|Z_train|Cash value of miscellaneous feature|
|mo_sold|float64|Z_train|Month sold|
|yr_sold|float64|Z_train|Year sold|
|ms_zoning_FV|float64|Z_train|General zoning classification Floating Village Residential|
|ms_zoning_RH|float64|Z_train|General zoning classification Residential High Quality|
|ms_zoning_RL|float64|Z_train|General zoning classification Residential Low Density|
|ms_zoning_RM|float64|Z_train|General zoning classification Residential Medium Density|
|street_Pave|float64|Z_train|Street pavement|
|land_contour_HLS|float64|Z_train|Flatness of property hillside|
|land_contour_Low|float64|Z_train|Flatness of property depression|
|land_contour_Lvl|float64|Z_train|Flatness of property near flat level|
|lot_config_CulDSac|float64|Z_train|lot configuration culdesac|
|lot_config_FR2|float64|Z_train|lot configuration frontage on 2 sides of property|
|lot_config_FR3|float64|Z_train|lot configuration on 3 sides of property|
|lot_config_Inside|float64|Z_train|lot configuration inside lot|
|neighborhood_Blueste|float64|Z_train|Physical locations within Ames city limits Bluestem|
|neighborhood_BrDale|float64|Z_train|Physical locations within Ames city limits Briardale|
|neighborhood_BrkSide|float64|Z_train|Physical locations within Ames city limits Brookside|
|neighborhood_ClearCr|float64|Z_train|Physical locations within Ames city limits Clear Creek|
|neighborhood_CollgCr|float64|Z_train|Physical locations within Ames city limits College Creek|
|neighborhood_Crawfor|float64|Z_train|Physical locations within Ames city limits Crawford|
|neighborhood_Edwards|float64|Z_train|Physical locations within Ames city limits Edwards|
|neighborhood_Gilbert|float64|Z_train|Physical locations within Ames city limits Gilbert|
|neighborhood_Greens|float64|Z_train|Physical locations within Ames city limits Greens|
|neighborhood_IDOTRR|float64|Z_train|Physical locations within Ames city limits Iowa DOT and Rail Road|
|neighborhood_MeadowV|float64|Z_train|Physical locations within Ames city limits Meadow Village|
|neighborhood_Mitchel|float64|Z_train|Physical locations within Ames city limits Mitchell|
|neighborhood_NAmes|float64|Z_train|Physical locations within Ames city limits North Ames|
|neighborhood_NWAmes|float64|Z_train|Physical locations within Ames city limits Northwest Ames|
|neighborhood_NoRidge|float64|Z_train|Physical locations within Ames city limits Northridge|
|neighborhood_NridgHt|float64|Z_train|Physical locations within Ames city limits Northridge Heights|
|neighborhood_OldTown|float64|Z_train|Physical locations within Ames city limits Oldtown|
|neighborhood_SWISU|float64|Z_train|Physical locations within Ames city limits South and West of Iowa State University|
|neighborhood_Sawyer|float64|Z_train|Physical locations within Ames city limits Sawyer|
|neighborhood_SawyerW|float64|Z_train|Physical locations within Ames city limits Sawyer West|
|neighborhood_Somerst|float64|Z_train|Physical locations within Ames city limits Somerset|
|neighborhood_StoneBr|float64|Z_train|Physical locations within Ames city limits Stone Brook|
|neighborhood_Timber|float64|Z_train|Physical locations within Ames city limits Timberland|
|neighborhood_Veenker|float64|Z_train|Physical locations within Ames city limits Veenker|
|condition_1_Feedr|float64|Z_train|Proximity to various condition adjacent to feeder street|
|condition_1_Norm|float64|Z_train|Proximity to various condition normal|
|condition_1_PosA|float64|Z_train|Proximity to various condition adjacent to positive offsite feature|
|condition_1_PosN|float64|Z_train|Proximity to various condition near positive off site feature park greenbelt etc|
|condition_1_RRAe|float64|Z_train|Proximity to various condition adjacent to eastwest railroad|
|condition_1_RRAn|float64|Z_train|Proximity to various condition Adjacent to NorthSouth Railroad|
|condition_2_Norm|float64|Z_train|Proximity to various condition Normal|
|bldg_type_2fmCon|float64|Z_train|type of building two family conversion originally built as one family dwelling|
|bldg_type_Duplex|float64|Z_train|type of building duplex|
|bldg_type_Twnhs|float64|Z_train|Type of building townhouse inside unit|
|bldg_type_TwnhsE|float64|Z_train|Type of building townhouse end unit|
|house_style_1.5Unf|float64|Z_train|Style of dwelling one and a half story second level unfinished|
|house_style_1Story|float64|Z_train|Style of dwelling one story|
|house_style_2.5Unf|float64|Z_train|Style of dwelling two and a half story unfinished second level|
|house_style_2Story|float64|Z_train|Style of dwelling two story|
|house_style_SFoyer|float64|Z_train|Style of dwelling split foyer|
|house_style_SLvl|float64|Z_train|Style of dwelling split level|
|roof_style_Gable|float64|Z_train|Type of roof Gable|
|roof_style_Gambrel|float64|Z_train|Type of roof Gambrel Barn|
|roof_style_Hip|float64|Z_train|Type of roof Hip|
|roof_style_Mansard|float64|Z_train|Type of roof Mansard|
|roof_matl_Tar|float64|Z_train|Roof material Gravel and Tar|
|&Grv|float64|Z_train|Grave misteak|
|exterior_1st_BrkFace|float64|Z_train|External covering on house brick face|
|exterior_1st_CemntBd|float64|Z_train|External covering on house cement board|
|exterior_1st_HdBoard|float64|Z_train|External covering on house hard board|
|exterior_1st_MetalSd|float64|Z_train|External covering on house metal siding|
|exterior_1st_Plywood|float64|Z_train|External covering on house plywood|
|exterior_1st_Stucco|float64|Z_train|External covering on house stucco|
|exterior_1st_VinylSd|float64|Z_train|External covering on house vinyl siding|
|exterior_1st_Wd Sdng|float64|Z_train|External covering on house wood siding|
|exterior_1st_WdShing|float64|Z_train|External covering on house wood shingles|
|exterior_2nd_BrkFace|float64|Z_train|External covering on house brick face|
|exterior_2nd_CmentBd|float64|Z_train|External covering on house cement board|
|exterior_2nd_HdBoard|float64|Z_train|External covering on house hard board|
|exterior_2nd_ImStucc|float64|Z_train|External covering on house imitation stucco|
|exterior_2nd_MetalSd|float64|Z_train|External covering on house metal siding|
|exterior_2nd_Plywood|float64|Z_train|External covering on house plywood|
|exterior_2nd_Stucco|float64|Z_train|External covering on house stucco|
|exterior_2nd_VinylSd|float64|Z_train|External covering on house vinyl siding|
|exterior_2nd_Wd Sdng|float64|Z_train|External covering on house wood siding|
|exterior_2nd_Wd Shng|float64|Z_train|External covering on house wood shingles|
|mas_vnr_type_BrkFace|float64|Z_train|Masonry veneer type brick face|
|mas_vnr_type_None|float64|Z_train|Masonry veneer type none|
|mas_vnr_type_Stone|float64|Z_train|Masonry veneer type Stone|
|foundation_CBlock|float64|Z_train|Type of foundation cinder block|
|foundation_PConc|float64|Z_train|Type of foundation poured concrete|
|foundation_Slab|float64|Z_train|Type of foundation slab|
|foundation_Stone|float64|Z_train|Type of foundation stone|
|foundation_Wood|float64|Z_train|Type of foundation wood|
|heating_GasW|float64|Z_train|Type of heating gas hot water or steam heat|
|heating_Grav|float64|Z_train|Type of heating gravity furnace|
|central_air_Y|float64|Z_train|Central air conditioning yes|
|garage_type_Attchd|float64|Z_train|Garage type attached|
|garage_type_Basment|float64|Z_train|Garage type basement|
|garage_type_BuiltIn|float64|Z_train|Garage type builtin|
|garage_type_CarPort|float64|Z_train|Garage type car port|
|garage_type_Detchd|float64|Z_train|Garage type detached from home|
|sale_type_CWD|float64|Z_train|Type of sale Cash warranty deed|
|sale_type_ConLD|float64|Z_train|Type of sale Contract low down|
|sale_type_ConLI|float64|Z_train|Type of sale contract low interest|
|sale_type_ConLw|float64|Z_train|Type of sale contract low down payment and low interest|
|sale_type_New|float64|Z_train|Type of sale new home just constructed and sold|
|sale_type_Oth|float64|Z_train|Type of sale other|
|sale_type_WD|float64|Z_train|Type of sale warranty deed conventional|
|id|float64|Z_test|Observation number|
|pid|float64|Z_test|Parcel identification number which can be used with city website for parcel review|
|ms_sub_class|float64|Z_test|Identifies the type of dwelling involved in the sale|
|lot_frontage|float64|Z_test|Linear feet of street connected to property|
|lot_area|float64|Z_test|Lot size in square feet|
|alley|float64|Z_test|Type of alley access to property|
|lot_shape|float64|Z_test|General shape of property|
|utilities|float64|Z_test|Type of utilities available|
|land_slope|float64|Z_test|Slope of property|
|overall_qual|float64|Z_test|Rates overall material and finish of the house|
|year_remod/add|float64|Z_test|Remodel date same as construction date if no remodeling or additions|
|mas_vnr_area|float64|Z_test|Masonry veneer area in square feet|
|exter_qual|float64|Z_test|Evaluates the quality of the material on the exterior|
|exter_cond|float64|Z_test|Evaluates the present condition of the material on the exterior|
|bsmt_qual|float64|Z_test|Evaluates the height of the basement|
|bsmt_cond|float64|Z_test|The average household income of a student's family per school district|
|bsmt_exposure|float64|Z_test|Refers to walkout or garden level walls|
|bsmt_fin_type_1|float64|Z_test|Rating of basement finished area|
|bsmt_fin_sf_1|float64|Z_test|Type 1 finished square feet|
|bsmt_fin_type_2|float64|Z_test|Rating of basement finished area if multiple types|
|bsmt_fin_sf_2|float64|Z_test|Type 2 finished square feet|
|bsmt_unf_sf|float64|Z_test|Unfinished square feet of basement area|
|total_bsmt_sf|float64|Z_test|Total square feet of basement area
|heating_qc|float64|Z_test|Heating quality and condition|
|electrical|float64|Z_test|Electrical system|
|1st_flr_sf|float64|Z_test|First floor square feet|
|2nd_flr_sf|float64|Z_test|Second floor square feet|
|low_qual_fin_sf|float64|Z_test|Low quality finished square feet for all floors|
|gr_liv_area|float64|Z_test|Above grade ground living area square feet|
|bsmt_full_bath|float64|Z_test|Basement full bathrooms|
|bsmt_half_bath|float64|Z_test|Basement half bathrooms|
|full_bath|float64|Z_test|Full bathrooms above grade|
|half_bath|float64|Z_test|Half bathrooms above grade|
|bedroom_abv_gr|float64|Z_test|Bedrooms above grade does not include basement bedrooms|
|kitchen_abv_gr|float64|Z_test|Kitchens above grade|
|kitchen_qual|float64|Z_test|Kitchen quality|
|tot_rms_abv_grd|float64|Z_test|Total rooms above grade does not include bathrooms|
|functional|float64|Z_test|Home functionality and assume typical unless deductions are warranted|
|fireplaces|float64|Z_test|Number of fireplaces|
|fireplace_qu|float64|Z_test|Fireplace quality|
|garage_yr_blt|float64|Z_test|Year garage was built|
|garage_finish|float64|Z_test|Interior finish of the garage|
|garage_cars|float64|Z_test|Size of garage in car capacity|
|garage_area|float64|Z_test|Size of garage in square feet|
|garage_qual|float64|Z_test|Garage quality|
|garage_cond|float64|Z_test|Garage condition|
|paved_drive|float64|Z_test|Paved driveway|
|wood_deck_sf|float64|Z_test|Wood deck area in square feet|
|open_porch_sf|float64|Z_test|Open porch area in square feet|
|enclosed_porch|float64|Z_test|Enclosed porch area in square feet|
|3ssn_porch|float64|Z_test|Three season porch area in square feet|
|screen_porch|float64|Z_test|Screen porch area in square feet|
|pool_area|float64|Z_test|Pool area in square feet|
|fence|float64|Z_test|Fence quality|
|misc_val|float64|Z_test|Cash value of miscellaneous feature|
|mo_sold|float64|Z_test|Month sold|
|yr_sold|float64|Z_test|Year sold|
|ms_zoning_FV|float64|Z_test|General zoning classification Floating Village Residential|
|ms_zoning_RH|float64|Z_test|General zoning classification Residential High Quality|
|ms_zoning_RL|float64|Z_test|General zoning classification Residential Low Density|
|ms_zoning_RM|float64|Z_test|General zoning classification Residential Medium Density|
|street_Pave|float64|Z_test|Street pavement|
|land_contour_HLS|float64|Z_test|Flatness of property hillside|
|land_contour_Low|float64|Z_test|Flatness of property depression|
|land_contour_Lvl|float64|Z_test|Flatness of property near flat level|
|lot_config_CulDSac|float64|Z_test|lot configuration culdesac|
|lot_config_FR2|float64|Z_test|lot configuration frontage on 2 sides of property|
|lot_config_FR3|float64|Z_test|lot configuration on 3 sides of property|
|lot_config_Inside|float64|Z_test|lot configuration inside lot|
|neighborhood_Blueste|float64|Z_test|Physical locations within Ames city limits Bluestem|
|neighborhood_BrDale|float64|Z_test|Physical locations within Ames city limits Briardale|
|neighborhood_BrkSide|float64|Z_test|Physical locations within Ames city limits Brookside|
|neighborhood_ClearCr|float64|Z_test|Physical locations within Ames city limits Clear Creek|
|neighborhood_CollgCr|float64|Z_test|Physical locations within Ames city limits College Creek|
|neighborhood_Crawfor|float64|Z_test|Physical locations within Ames city limits Crawford|
|neighborhood_Edwards|float64|Z_test|Physical locations within Ames city limits Edwards|
|neighborhood_Gilbert|float64|Z_test|Physical locations within Ames city limits Gilbert|
|neighborhood_Greens|float64|Z_test|Physical locations within Ames city limits Greens|
|neighborhood_IDOTRR|float64|Z_test|Physical locations within Ames city limits Iowa DOT and Rail Road|
|neighborhood_MeadowV|float64|Z_test|Physical locations within Ames city limits Meadow Village|
|neighborhood_Mitchel|float64|Z_test|Physical locations within Ames city limits Mitchell|
|neighborhood_NAmes|float64|Z_test|Physical locations within Ames city limits North Ames|
|neighborhood_NWAmes|float64|Z_test|Physical locations within Ames city limits Northwest Ames|
|neighborhood_NoRidge|float64|Z_test|Physical locations within Ames city limits Northridge|
|neighborhood_NridgHt|float64|Z_test|Physical locations within Ames city limits Northridge Heights|
|neighborhood_OldTown|float64|Z_test|Physical locations within Ames city limits Oldtown|
|neighborhood_SWISU|float64|Z_test|Physical locations within Ames city limits South and West of Iowa State University|
|neighborhood_Sawyer|float64|Z_test|Physical locations within Ames city limits Sawyer|
|neighborhood_SawyerW|float64|Z_test|Physical locations within Ames city limits Sawyer West|
|neighborhood_Somerst|float64|Z_test|Physical locations within Ames city limits Somerset|
|neighborhood_StoneBr|float64|Z_test|Physical locations within Ames city limits Stone Brook|
|neighborhood_Timber|float64|Z_test|Physical locations within Ames city limits Timberland|
|neighborhood_Veenker|float64|Z_test|Physical locations within Ames city limits Veenker|
|condition_1_Feedr|float64|Z_test|Proximity to various condition adjacent to feeder street|
|condition_1_Norm|float64|Z_test|Proximity to various condition normal|
|condition_1_PosA|float64|Z_test|Proximity to various condition adjacent to positive offsite feature|
|condition_1_PosN|float64|Z_test|Proximity to various condition near positive off site feature park greenbelt etc|
|condition_1_RRAe|float64|Z_test|Proximity to various condition adjacent to eastwest railroad|
|condition_1_RRAn|float64|Z_test|Proximity to various condition Adjacent to NorthSouth Railroad|
|condition_2_Norm|float64|Z_test|Proximity to various condition Normal|
|bldg_type_2fmCon|float64|Z_test|type of building two family conversion originally built as one family dwelling|
|bldg_type_Duplex|float64|Z_test|type of building duplex|
|bldg_type_Twnhs|float64|Z_test|Type of building townhouse inside unit|
|bldg_type_TwnhsE|float64|Z_test|Type of building townhouse end unit|
|house_style_1.5Unf|float64|Z_test|Style of dwelling one and a half story second level unfinished|
|house_style_1Story|float64|Z_test|Style of dwelling one story|
|house_style_2.5Unf|float64|Z_test|Style of dwelling two and a half story unfinished second level|
|house_style_2Story|float64|Z_test|Style of dwelling two story|
|house_style_SFoyer|float64|Z_test|Style of dwelling split foyer|
|house_style_SLvl|float64|Z_test|Style of dwelling split level|
|roof_style_Gable|float64|Z_test|Type of roof Gable|
|roof_style_Gambrel|float64|Z_test|Type of roof Gambrel Barn|
|roof_style_Hip|float64|Z_test|Type of roof Hip|
|roof_style_Mansard|float64|Z_test|Type of roof Mansard|
|roof_matl_Tar|float64|Z_test|Roof material Gravel and Tar|
|&Grv|float64|Z_test|Grave misteak|
|exterior_1st_BrkFace|float64|Z_test|External covering on house brick face|
|exterior_1st_CemntBd|float64|Z_test|External covering on house cement board|
|exterior_1st_HdBoard|float64|Z_test|External covering on house hard board|
|exterior_1st_MetalSd|float64|Z_test|External covering on house metal siding|
|exterior_1st_Plywood|float64|Z_test|External covering on house plywood|
|exterior_1st_Stucco|float64|Z_test|External covering on house stucco|
|exterior_1st_VinylSd|float64|Z_test|External covering on house vinyl siding|
|exterior_1st_Wd Sdng|float64|Z_test|External covering on house wood siding|
|exterior_1st_WdShing|float64|Z_test|External covering on house wood shingles|
|exterior_2nd_BrkFace|float64|Z_test|External covering on house brick face|
|exterior_2nd_CmentBd|float64|Z_test|External covering on house cement board|
|exterior_2nd_HdBoard|float64|Z_test|External covering on house hard board|
|exterior_2nd_ImStucc|float64|Z_test|External covering on house imitation stucco|
|exterior_2nd_MetalSd|float64|Z_test|External covering on house metal siding|
|exterior_2nd_Plywood|float64|Z_test|External covering on house plywood|
|exterior_2nd_Stucco|float64|Z_test|External covering on house stucco|
|exterior_2nd_VinylSd|float64|Z_test|External covering on house vinyl siding|
|exterior_2nd_Wd Sdng|float64|Z_test|External covering on house wood siding|
|exterior_2nd_Wd Shng|float64|Z_test|External covering on house wood shingles|
|mas_vnr_type_BrkFace|float64|Z_test|Masonry veneer type brick face|
|mas_vnr_type_None|float64|Z_test|Masonry veneer type none|
|mas_vnr_type_Stone|float64|Z_test|Masonry veneer type Stone|
|foundation_CBlock|float64|Z_test|Type of foundation cinder block|
|foundation_PConc|float64|Z_test|Type of foundation poured concrete|
|foundation_Slab|float64|Z_test|Type of foundation slab|
|foundation_Stone|float64|Z_test|Type of foundation stone|
|foundation_Wood|float64|Z_test|Type of foundation wood|
|heating_GasW|float64|Z_test|Type of heating gas hot water or steam heat|
|heating_Grav|float64|Z_test|Type of heating gravity furnace|
|central_air_Y|float64|Z_test|Central air conditioning yes|
|garage_type_Attchd|float64|Z_test|Garage type attached|
|garage_type_Basment|float64|Z_test|Garage type basement|
|garage_type_BuiltIn|float64|Z_test|Garage type builtin|
|garage_type_CarPort|float64|Z_test|Garage type car port|
|garage_type_Detchd|float64|Z_test|Garage type detached from home|
|sale_type_CWD|float64|Z_test|Type of sale Cash warranty deed|
|sale_type_ConLD|float64|Z_test|Type of sale Contract low down|
|sale_type_ConLI|float64|Z_test|Type of sale contract low interest|
|sale_type_ConLw|float64|Z_test|Type of sale contract low down payment and low interest|
|sale_type_New|float64|Z_test|Type of sale new home just constructed and sold|
|sale_type_Oth|float64|Z_test|Type of sale other|
|sale_type_WD|float64|Z_test|Type of sale warranty deed conventional|
|sale_price|float64|y_train|Sale price of house|
|sale_price|float64|y_test|Sale price of house|

## Brief Summary of Analysis
- We want to avoid neighborhoods where living there can actually increase the price of your house like Northridge Heights, Stone Brook, and Crawford.
- We also want to avoid spacious places, where the overall quality of the house is great, relatively new places and places with excellent exteriors and kitchens.  These would all increase the sale price of the house, with the area of the house increasing it the most, and we do not want that.


## Recommendations
- The neighborhoods we want to look at for our center are North Ames, Edwards, and Northwest Ames. These will be neighborhoods where having a house in that neighborhood would actually decrease the value of the house.
- Our dream home for our LGBT center would be a townhouse end unit, externally covered in plywood or hardboard, with a roof material being tar and gravel, adjacent to the east-west railroad, since all those factors hurt the price of the sale price of the home, and will make things cheaper for us.
- Since areas with lower home prices could be where there are more underserved community members, setting up an LGBT+ youth center could be beneficial to preventing common community ailments. Furthermore, minimizing the costs of buying a center can mean more is put towards other important things, like counseling and medical costs. This can be applied to other cities in other states where LGBT+ youth and adults are not given the proper resources they need to survive.  
- To make the model more applicable, I would have also brought in some statistics about LGBT+ youth, homelessness, HIV transmission rate, transgender youth and the intersections of all these areas  in Ames, Iowa, and maybe Iowa in general. These topics tend to be a commonality with the problems that the LGBT+ community faces countrywide.
