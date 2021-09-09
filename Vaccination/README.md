## Data download: ##

File 'covid-19-resultats-issus-des-appariements-entre-si-vic-si-dep-et-vac-si.csv' downloaded from https://data.drees.solidarites-sante.gouv.fr/explore/dataset/covid-19-resultats-issus-des-appariements-entre-si-vic-si-dep-et-vac-si/export/?disjunctive.vac_statut on September 3, 2021.

Nomenclature: according to https://drees.solidarites-sante.gouv.fr/sites/default/files/2021-05/DD79.pdf (page 27):

HC: conventional hospitalization

SC: critical care hospitalization

DC: death

Stratified by age: file 'Par_age_covid-19-resultats-par-age-issus-des-appariements-entre-si-vic-si-dep-et-vac-si.csv' downloaded from https://data.drees.solidarites-sante.gouv.fr/explore/dataset/covid-19-resultats-par-age-issus-des-appariements-entre-si-vic-si-dep-et-vac-si/download/?format=csv&timezone=Europe/Berlin&lang=fr&use_labels_for_header=true&csv_separator=%3B on September 8, 2021.

## Plot tracing: ##

``R CMD BATCH R_commands_vaccination_data``

Resulting graphs: 'Hospitalisation_conventionnelle_for_various_vaccination_statuses.pdf', 'Hospitalisation_soins_critiques_for_various_vaccination_statuses.pdf' and 'Décès_hospitaliers_for_various_vaccination_statuses.pdf'.

``R CMD BATCH R_commands_by_age_and_vaccination_status``

Resulting graphs: 'Hospitalisation_conventionnelle_pour_\*.pdf' and 'Soins_critiques_pour_\*.pdf'.
