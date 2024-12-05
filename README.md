Automated Process Analyzing the Risk of HABS through ECOSTRESS LST Temperature
Requests ECOSTRESS LST data once a week and define's data request time frame
Downloads and Analyzes the data utilizing Zonal Statistics: Mean, Median, Standard Deviation, Max, Min
Connects to Google Cloud API Key Drive and Spreadsheet, which will link to ArcGIS dashboard
API Satellite Download Code Logic Derived from work by Quentin Dehaene, utilized with permission
  Reference the original logic here: https://github.com/ghulley/urban-umbrella/blob/main/ECOSTRESS%20Sharpening/Sharpening_S2/Sharpening_ECOSTRESS_API.ipynb
Improvements to be made:
  Analyze LST product not Cloud Mask
  Improve Cloud Mask Logic ==> Make sure the overpass is not used if more than 40% clouds detected
  Improve connection to drive to output clipped tif
  Improve data classification products in transfer to spreadsheet, have it automatically assign risk level
NOTE: This current version of the code is slightly modified so I can input a start date (so I can properly test it over and over) I have the logic to reassign the weekly automatic run
