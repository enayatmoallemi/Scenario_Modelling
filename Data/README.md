# Data sets used for the generation results/figures

The 'Vensim_calibration' folder contains the following datasets:
* 'GDP_Pop_Edu_calibration' contains all data and files required for the calibration of population, GDP, and education in FeliX under the projections of IIASA and OECD to be used in Vensim. Within this folder:
** 'GDP_Pop_Edu_calibration_final_results.xlsx' shows a summary of calibration results for population, GDP, and education under each SSP.
** `SSP_dataset_import_to_Vensim_conversion_formats.frm` is  FoRM file used to tell Vensim how to import tab delimited and spreadsheet files. This is used for converting the SSP spreadsheets into Vensim datasets for calibration.
** `SSP1_calibration_uncertain_parameters.voc` to `SSP5_calibration_uncertain_parameters.voc`:  Vensim Optimization Control file (including the definition of the uncertainty ranges to search over during calibration), used to specify how to optimize a model. This is a text file (Pro/DSS only). This file is not currently used in the current version of analysis.
** `SSPs_calibration_payoff_definition.vpd`:  Vensim Payoff Definition. Used to define the payoff for optimization (text file Pro/DSS only). This file is not currently used in the current version of analysis.
** The rest of calibration result files generated by vensim.
* 'SSP1_calibrated_all_parameters' to 'SSP5_calibrated_all_parameters' are the calibrated value of model parameters under each SSP to be used as input data when running the model in Vensim.
* `SSP1_Felix.vdfx` to 'SSP5_FeliX.vdfx' are the SSP 1 to SSP5 projections with the FeliX model (for the  value in 'SSP1_calibrated_all_parameters') to be used for comparing FeliX projection with other projections in Vensim.
* `SSP1_Felix.xlsx` to 'SSP5_FeliX.xlsx' are the SSP 1 to SSP5 projections with the FeliX model (for the  value in 'SSP1_calibrated_all_parameters') (same as SSPs_Felix.vdfx, but in CSV format).
* `Export_vdfx_files_to_excel_v19.lst`: LiST file containing a set of variables to be saved from the Vensim simulation runs and converted into to a CSV file.


The 'IIASA_SSP_dataset' folder contains SSP data from other IAMs projections, downloaded from the [IIASA Database](https://tntcat.iiasa.ac.at/SspDb/dsd?Action=htmlpage&page=about).
* `SSP_GDP.xlsx`: This lists the GDP projection under different SSPs. This was used as input data for generating the calibration plots.
* `SSP_Population.xlsx`: This lists the population projection under different SSPs. This was used as input data for generating the calibration plots.
* `SSP_Scenarios.xlsx`: This lists the projection of energy, land-use, climate, etc. under different SSPs using the SSP IAMs. This was used as input data for generating the calibration plots.
* `Historical_Felix.xlsx`: This lists the histircal data (1900-2020) that were generated by the FeliX model.
