# GermanicPOS
### Structure
Models:
  - Contains Basic formations of the model. These jupyter notebooks can be dowloaded alongside the corresponding datasets and run as is to reproduce the results of the study.
    - The OHG dialect examination can be replicated by replacing the file name in the data loading at the beginning of the notebook, to call the desired dialectal subset ("OHG_sents_notker.npy", "OHG_sents_notker2.npy", "OHG_sents_heterogenous.npy") and ("OHG_tags_minimal_notker.npy", "OHG_tags_minimal_notker2.npy", "OHG_tags_minimal_heterogenous.npy")
  - Ablation
    - Contains scheduler to subsample and train for the ablation study
    - Each ablation file contains the essential contents of the corresponding language models, placed in a loop such that it trains the model 100 times per language per desired dataset size
    - 
Datasets:
  - Contains extracted aligned sentence-tag arrays for all languages, including the OHG dialect subsamples, parsed from the datasets cited below
  - Tagset Descriptions (Appendix A) is a reproduction of the appendix from the associated study. This provides a complete list of subsititutions and conversions that were made to produce the X_tags_minimal.npy files available here
  
Results & Visualizations:
  - The files here are the complete results set from the original study for any examination
  - Contains The output accuracies of all of the models grouped by language (all sample sizes)
  - Contains code to generate the plots used in the paper

### Dataset Citation Info
De Herdt, T. (1997). Project Wulfila : an electronic edition of the Gothic Bible. Universitaire Faculteiten Sint-Ignatius Antwerpen.

Taylor, A., A. Warner, S. Pintzuk, and F. Beths. (2003). The York-Toronto-Helsinki Parsed Corpus of Old English Prose. Oxford Text Archive.

Walkden, G. (2016). The HeliPaD: a parsed corpus of Old Saxon. International journal of corpus linguistics, 21(4), (pp. 559-571).

Wallenberg, J. C., Ingason A. K., Sigurðsson, E. F., and Rögnvaldsson E. (2011). Icelandic Parsed Historical Corpus (IcePaHC). Version 0.9. http://www.linguist.is/icelandic_treebank

Zeige, L. E. , Schnelle, G., Klotz, M., Donhauser, K., Gippert, J., Lühr, R. (2024). Deutsch Diachron Digital - Referenzkorpus Altdeutsch. Version 1.2. Humboldt-Universität zu Berlin.
