## This folder contains protein interaction datasets

# Folders:

InActRelease_2017Nov13 - IntAct database release (txt.gz) and viral taxonomy from last uniprot release. Output of interactions_and_sequences.Rmd script.

DownloadDate_20181122 - data from VirHostNet database downloaded on 22/11/2018 and and viral taxonomy from last uniprot release. Output of interactions_and_sequences.Rmd script.

# Files:

human_viral.tsv.zip - human (9606)-viral (10239) network. Compressed to avoid GitHub file size restriction. Output of interactions_and_sequences.Rmd script.

viral_viral.tsv - protein interactions between viral proteins of human-interacting viral taxons. Output of interactions_and_sequences.Rmd script.

viral_viral.tsv - all interactions between human proteins. Output of interactions_and_sequences.Rmd script.

VirHostNet_human_viral.tsv - interactions between human and viral proteins that are uniquely present in VirHostNet database (not in IntAct)

# Description of columns in these files

pair_id - unique identifier of the undirected interaction: ordered alphabetically and concatenated interacting molecule IDs

IDs_interactor_A, IDs_interactor_B - interacting molecule ID

interactor_IDs_databases_A, interactor_IDs_databases_B - database that provides interacting molecule ID such as UniProt, ChEMBL or IntAct (IntAct: when the molecule cannot be mapped to ID in any other resource)

Taxid_interactor_A, Taxid_interactor_B - taxonomic species that interacting molecule belongs to

Publication_Identifiers - pubmed ID of the papers that has reported the interaction

Confidence_values - MIscore. Details: https://psicquic.github.io/MITAB25Format.html, http://www.ebi.ac.uk/intact/pages/faq/faq.xhtml, https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4316181/

Host_organisms - taxid of organism in which the interaction detections experiment was performed

bait_prey_status_A, bait_prey_status_B - specifies the experimental role of a protein: a bait, a prey, a neutral component or else (http://www.ebi.ac.uk/ols/ontologies/MI/terms?obo_id=MI:0495)

Interaction_detection_methods - Method to determine the interaction. http://www.ebi.ac.uk/ols/ontologies/MI/terms?obo_id=MI:0001

Interaction_types - http://www.ebi.ac.uk/ols/ontologies/MI/terms?obo_id=MI:0190

Interaction_identifiers - Interaction identifier given by database (e.g. intact:EBI-1547321|imex:IM-11865-3)

Expansion_methods - The method by which complex n-ary data is expanded into binary data. http://www.ebi.ac.uk/ols/ontologies/MI/terms?obo_id=MI:1059

Features_interactor_A, Features_interactor_B - Property of a subsequence that may interfere with the binding of a molecule. http://www.ebi.ac.uk/ols/ontologies/MI/terms?obo_id=MI:0116

Identification_method_participant_A, Identification_method_participant_B - Method to determine the molecules involved in the interaction. http://www.ebi.ac.uk/ols/ontologies/MI/terms?obo_id=MI:0002

binding_region_A_start, binding_region_A_end, binding_region_B_start, binding_region_B_end - start and end position of binding-associated features

binding_region_A_type, binding_region_B_type - Type of the binding region. Details: http://www.ebi.ac.uk/ols/ontologies/MI/terms?obo_id=MI:0117, https://psicquic.github.io/MITAB27Format.html