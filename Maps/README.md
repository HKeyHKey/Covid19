## Download of population data:

``wget https://www.insee.fr/fr/statistiques/fichier/4265429/ensemble.zip;unzip ensemble.zip ``


## Statistics on confirmed Covid19 cases in every French "région" (sometimes with statistics at the smaller administrative scale: "départements"):

Compiled from Regional Health agencies ("ARS") and from https://www.eficiens.com/nombre-de-cas-coronavirus-par-region. Compiled data file: 'Donnees_des_ARS.dat' (raw text, tab-separated).


## Download of geographic "région" and "département" contours:

From https://www.data.gouv.fr/fr/datasets/contours-des-departements-francais-issus-d-openstreetmap/ and https://www.data.gouv.fr/fr/datasets/contours-des-regions-francaises-sur-openstreetmap/
(using the 2014 simplified contours for "départements" and 2018 contours for "régions").

## Map drawing (one individual PDF file per frame):

``R CMD BATCH R_commands_carte``

## Conversion of PDF frames to PNG, and video assembly:

``for f in `ls Carte_*.pdf`;do pdftoppm $f `echo $f | sed 's|\.pdf$||'` -png -rx 300 -ry 300;mv `echo $f | sed 's|\.pdf$|-1.png|'` `echo $f | sed 's|\.pdf$|.png|'`;done;ffmpeg -r 5 -i Carte_nombre_%03d.png -vcodec libx264 -preset veryslow -s 1024x768 -crf 18 Nombre_de_cas.avi;ffmpeg -r 5 -i Carte_taux_%03d.png -vcodec libx264 -preset veryslow -s 1024x768 -crf 18 Taux_de_cas.avi``

Video 'Nombre_de_cas.avi' is published on Youtube at: https://youtu.be/XIJpLlKEF7E
and video 'Taux_de_cas.avi' is published on Youtube at: https://youtu.be/VlVxPjh-RVg.
