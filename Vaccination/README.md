## Data download: ##

File 'covid-19-resultats-issus-des-appariements-entre-si-vic-si-dep-et-vac-si.csv' downloaded from https://data.drees.solidarites-sante.gouv.fr/explore/dataset/covid-19-resultats-issus-des-appariements-entre-si-vic-si-dep-et-vac-si/export/?disjunctive.vac_statut on September 3, 2021.

File '20220113_covid-19-resultats-issus-des-appariements-entre-si-vic-si-dep-et-vac-si.csv' downloaded from the same page on January 13, 2022.

Nomenclature: according to https://drees.solidarites-sante.gouv.fr/sites/default/files/2021-05/DD79.pdf (page 27):

HC: conventional hospitalization

SC: critical care hospitalization

DC: death

Stratified by age: file 'Par_age_covid-19-resultats-par-age-issus-des-appariements-entre-si-vic-si-dep-et-vac-si.csv' downloaded from https://data.drees.solidarites-sante.gouv.fr/explore/dataset/covid-19-resultats-par-age-issus-des-appariements-entre-si-vic-si-dep-et-vac-si/download/?format=csv&timezone=Europe/Berlin&lang=fr&use_labels_for_header=true&csv_separator=%3B at various dates (see below).

## Plot tracing (before third dose policy: September 2021 data): ##

Data downloaded on September 8, 2021.

``R CMD BATCH R_commands_vaccination_data``

Resulting graphs: 'Hospitalisation_conventionnelle_for_various_vaccination_statuses.pdf', 'Hospitalisation_soins_critiques_for_various_vaccination_statuses.pdf' and 'Décès_hospitaliers_for_various_vaccination_statuses.pdf'.

``R CMD BATCH R_commands_by_age_and_vaccination_status``

Resulting graphs: 'Hospitalisation_conventionnelle_pour_\*.pdf' and 'Soins_critiques_pour_\*.pdf'.

## Plot tracing (during third dose policy: January 2022 data): ##

Data downloaded on January 13, 2022.

``R CMD BATCH R_commands_vaccination_data_January2022``

Resulting graphs: 'Hospitalisation_conventionnelle_for_various_vaccination_statuses_under_3_dose_scheme.pdf', 'Hospitalisation_soins_critiques_for_various_vaccination_statuses_under_3_dose_scheme.pdf' and 'Décès_hospitaliers_for_various_vaccination_statuses_under_3_dose_scheme.pdf'.

## Plot tracing (stratified by age class, and focusing on hospitalization, critical care and death _for_ Covid: April 2022 data): ##

Data file downloaded on April 23, 2022 from [the DREES website](https://data.drees.solidarites-sante.gouv.fr/explore/dataset/covid-19-resultats-par-age-issus-des-appariements-entre-si-vic-si-dep-et-vac-si/download/?format=csv&timezone=Europe/Berlin&lang=fr&use_labels_for_header=true&csv_separator=%3B) (file renamed '20220423_covid-19-resultats-par-age-issus-des-appariements-entre-si-vic-si-dep-et-vac-si.csv'), then:

``R CMD BATCH R_commands_by_age_and_vaccination_status_April2022``

Resulting graphs: 'Hospitalisation_conventionnelle_pour_Covid_pour_age_\*\_stratifie_par_statut_vaccinal.pdf', 'Soins_critiques_pour_Covid_pour_age_\*\_stratifie_par_statut_vaccinal.pdf' and 'Décès_hospitalier_pour_Covid_pour_age_\*\_stratifie_par_statut_vaccinal.pdf'.
