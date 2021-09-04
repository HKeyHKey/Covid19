## Data download (on September 4, 2021): ##

``wget -O data_on_04092021.csv https://www.data.gouv.fr/fr/datasets/r/f335f9ea-86e3-4ffa-9684-93c009d5e617``

## Plot tracing: ##

``Rscript R_commands_deaths_vs_cases data_on_04092021.csv``

Resulting files: 'Determination_of_offset.pdf' for offset determination (positive cases to hospitalization, to transfer to ICU, to deaths); 'Comparison_\*.pdf' for the dynamics of symptom aggravation (how many positive cases translate into hospitalization, how many ICU transfers translate into death,...).
