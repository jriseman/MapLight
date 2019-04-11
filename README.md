# MapLight
James Riseman created this project in conjunction with MapLight.org - they referred good data sources to James.
You can see an overview of the project here: https://docs.google.com/presentation/d/1fyOguTdImeoSvWBXMPHJkQ1iNyXVh_w8Zpth9qsONMY/edit?usp=sharing
The initial Federal Election Commission data for 2010-2018 was downloaded from here: https://maplight.org/data_guide/download-federal-money-and-politics-data-set/
These data sets were broken out to files with 500K rows each. I aggregated them by time period in the file EDA_initial_aggregation.ipynb
These files get very big (up to 8.5M rows), so it's good to only work with one at a time on a local machine. I named them:
  df_comp10.csv
  df_comp12.csv
  df_comp14.csv
  df_comp16.csv
  df_comp18.csv
You'll have to re-create them from the aforementioned .ipynb file to proceed.
I then grouped the data sets by the field "DonorOrganization" and the field "DonorCommitteeNameNormalized" into more manage-able files.
This was done with EDA_DonorGroups.ipynb
