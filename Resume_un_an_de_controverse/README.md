##Data download:##

``wget -O Donnees_hospitalieres_au_10052021.csv https://www.data.gouv.fr/fr/datasets/r/63352e38-d353-4b54-bfd1-f1b3ee1cabd7``


##Geographical contour download:##

From https://www.data.gouv.fr/fr/datasets/contours-des-departements-francais-issus-d-openstreetmap/ (on March 24, 2020).


##Map tracing:##

``Rscript R_commands_Covid_hospital_lethality_per_department Donnees_hospitalieres_au_10052021.csv``
