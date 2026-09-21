# code_release_001

This repository contains all scripts and code used for the generation of Darwin Core Archives for the 2nd EMO BON sequencing batch.

For related repositories, please see:

[data_release_001](https://github.com/emo-bon/data_release_001): Occurrence and event data.

[analysis_release_001](https://github.com/emo-bon/analysis-results-cluster-01-crate): Bioinformatics pipeline outputs.


## Step 1:

Download the metaGOflow results and rename the files. 

## Step 2:

Open the files in R and create the basic files. 

The relevant script is EMOBON_metaGOflow.R

## Step 3: 

Rename the samples so that the will have the correct source_mat_ids.

The relevant script is EMOBON_substitute_ids.R

## Step 4:


Retrieve AphiaIDs for taxa

While we have tried different approaches to retrieve the AphiaIDs for the taxonomic occurrences, the most complete and accurate one is to download the genbank_links Parquet file from [EDITO](https://browser.moregeo.it/external/minio.dive.edito.eu/oidc-sfooks/worms_stac/marine_taxonomy/worms_taxonomy_traits/worms_taxonomy_traits.json?.asset=asset-genbank_links_parquet) and use it to retrieve the AphiaIDs based on their corresponding NCBI Taxonomy IDs. 

The relevant script is Retrieve_AphiaIDs_taxonRanks.R

## Step 5:



