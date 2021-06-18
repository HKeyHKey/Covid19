## Analysis (categorizing patients as "positive" or "negative" with the same criteria than Gautret et al., but including available confounding variables): ##

N.B.: the data presented in <a href=https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7102549/>Gautret et al. (2020)</a> are wrong, as demonstrated in <a href=https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7779264/>the correction issued in January 2021</a>. The authors have not released the corrected data table - hence we are left with the fake one (suppl. table S1 of Gautret et al., 2020), which I copied here for didactical reasons ('Gautret_et_al_2020_data.dat').

Honest analysis of the data requires considering every available explanatory variable (HCQ and AZI treatment, as well as patient age, sex, and initial clinical status - omitting "time before inclusion", which is expected to be strongly linked to the initial clinical status, while being less rigorously measured). In R syntax, this could be tested by a linear model of the positive/negative PCR response (variable "y") with these 5 potential explanatory variables:
``lm(y~log(t)+age+sex+status+hcq+azth)``
