## Data download: ##
``wget -O Donnees_hospitalieres_au_09032021.csv https://www.data.gouv.fr/fr/datasets/r/63352e38-d353-4b54-bfd1-f1b3ee1cabd7``

Geographical contours: downloaded from https://www.data.gouv.fr/fr/datasets/contours-des-departements-francais-issus-d-openstreetmap/ (100 m resolution, 2014 version), © contributors of OpenStreetMap under ODbL licence.

## Map of Covid-19 lethality in hospitals, département by département: ##
``Rscript R_commands_cartes_departements Donnees_hospitalieres_au_09032021.csv``

## Mortality of hospitalized Covid-19 patients, département by département: ##
``Rscript R_commands_mortalite_hospitaliere Donnees_hospitalieres_au_09032021.csv``
