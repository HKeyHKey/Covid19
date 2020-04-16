## Daily number of deaths per département:

Data file '2020-04-10_deces_sexe_age_lieu_csv.zip' downloaded from https://insee.fr/fr/information/4470857 and data file 'Departements.csv' extracted from https://www.insee.fr/fr/statistiques/fichier/4265429/ensemble.zip

``R CMD BATCH R_commands_deces_INSEE``

## Daily number of Covid19-attributed deaths per département:

``wget https://www.eficiens.com/corostats/openstats/open_stats_coronavirus.csv;R CMD BATCH R_commands_deces_par_Covid19``

## Daily number of emergency hospitalization for Covid19 symptoms:

Data file 'sursaud-covid19-quotidien-2020-04-16-10h47-departement.csv' downloaded from https://www.data.gouv.fr/fr/datasets/donnees-des-urgences-hospitalieres-et-de-sos-medecins-relatives-a-lepidemie-de-covid-19/#_

``R CMD BATCH R_commands_sante_publique_France``
