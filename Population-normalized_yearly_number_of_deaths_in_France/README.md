## Source of data: ##
Monthly death toll in France (starting in 1994): from https://www.insee.fr/fr/statistiques/serie/001641603#Telechargement
Total French population (includes extramarine territories in 1982 and later): from https://archined.ined.fr/download/publication/AXWs9WivkgKZhr-blhHr/7f62b3de7cbe6b9374432283d96d435d1607971435432.xlsx

## Analysis: ##
After reformatting the population data file into CSV format (in a file named 'Population_francaise_par_annee.csv', copied here for convenience):
``R CMD BATCH R_commands_deces_par_annee_normalises_par_la_population``

## Output: ##
File 'Deces_normalises_par_la_population_annee_apres_annee.pdf' (copied here for convenience).
