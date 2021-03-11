HIV variant collection downloaded from https://www.hiv.lanl.gov/content/index (database accessed on April 26, 2020); SARS-CoV-2 variant collection downloded from https://platform.gisaid.org/epi3/frontend# (database accessed on April 22, 2020; then: selection of variants at least 26 kb long, with no more than 5% "N" ambiguities).
HIV variant file named 'hiv-db.fasta', selected SARS-CoV-2 variant file named 'Selected_Corrected_April22_gisaid_cov2020_sequences.fasta'.

``makeblastdb -dbtype nucl -in hiv-db.fasta;blastn -query Selected_Corrected_April22_gisaid_cov2020_sequences.fasta -db hiv-db.fasta -word_size 8 -evalue 100 -outfmt 6 > blast_output_SARS-CoV-2_on_HIV``
