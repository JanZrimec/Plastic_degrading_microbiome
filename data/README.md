## Supplementary datasets

### Dataset S1: Dataset_queries.csv
A compiled dataset of 95 sequenced plastic enzymes spanning 17 plastic types with experimentally observed evidence of plastic modifying or degrading activity from published studies and databases (see publication).
The dataframe contains the following columns: plastic, id, organism, reference, doi, pmid, proteins names and aa_seq, where 'plastic' denotes the plastic name and 'id' is a unique id used to identify the enzymes derived from the uniprot id.

### Dataset S2: Dataset_hits.csv
A dataset of plastic-degrading enyzme hits across the global microbiome identified using hidden Markov models (HMMs) constructed from the above query dataset (see publicaton). The HMM queries across metagenomes identified altogether 30,025 homologous plastic-degrading enzyme hits non-redundant at the amino acid level, comprising 11,906 hits in the ocean and 18,119 in the soil dataset. 
The dataframe contains the following columns: target_name, hmm_model, plastic, dataset, e_value, score, seqid, auc, latitude, longitude, country, ocean and environment, where 'target_name' denotes the unique id of the target metagenome assembly, 'hmm_model' the unique id of the query hmm model (plastic id, seq. id. cutoff, model consecutive number), 'score' the bitscore, 'seqid' the blast seq. id. cutoff used to construct the hmm model, 'auc' the area under the precision-recall curve after filtering using gut microbiome data, and 'latitude, longitude, country, ocean and environment' columns denote the sample-specific parameters (see publication).

### Hidden Markov models: Dataset_HMMs.tar.gz
An tar.gz archive containing the .hmm file with the Hidden Markov models (HMMs) constructed from the above query enyzme data as described in the publication. This is an ASCII file containing descriptive records followed by large numerical matrices that hold the probabilistic models of the enzymes.
