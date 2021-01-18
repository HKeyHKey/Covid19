Data file ('donnees-hospitalieres-covid19-2021-01-08-19h03.csv') downloaded on January 9, 2021 from https://www.data.gouv.fr/fr/datasets/donnees-hospitalieres-relatives-a-lepidemie-de-covid-19/#_ ; geographical contour file ('departements-20140306-100m-shp.zip') downloaded on March 24, 2020 from https://www.data.gouv.fr/fr/datasets/contours-des-departements-francais-issus-d-openstreetmap/ and unzipped; population data file 'Departements.csv' extracted from https://www.insee.fr/fr/statistiques/fichier/4265429/ensemble.zip ; then:

Plotting maps:

``Rscript R_commands_cartes_departements donnees-hospitalieres-covid19-2021-01-08-19h03.csv``

Correlation analysis between the two waves:

``Rscript R_commands_correlation_across_waves donnees-hospitalieres-covid19-2021-01-08-19h03.csv``

N.B.: In that dataset, patients are not assigned to a département based on their actual living place, but based on the location of the hospital where they are treated. Hence normalization by population size is approximate (especially for small départements like « Territoire de Belfort », which may host patients from neighboring départements, artificially increasing its lethality rate). See discussion (un French) on https://www.data.gouv.fr/fr/datasets/donnees-hospitalieres-relatives-a-lepidemie-de-covid-19/#discussion-6004c36285b126b6f08909af-1
