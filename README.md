UCCA English Web Treebank Corpus
================================
Version 0.1 (August 13, 2018)
-----------------------------

This bundle contains 163 passages from the reviews section of the English Web Treebank (LDC2012T13),
annotated according to the foundational layer of UCCA, v2.0. 
The passages are given as xmls in the [UCCA format](https://github.com/UniversalConceptualCognitiveAnnotation/docs/blob/master/FORMAT.md).
This corpus contains 11103 tokens over 804 sentences, as tokenized and split according
to the [Universal Dependencies English Web Treebank](http://github.com/UniversalDependencies/UD_English-EWT) dataset.
Of the UCCA-annotated sentences, 622 belong to the UD training set, 192 to the development set and
153 to the test set.


Files included
--------------
1. The passages files in XML format. file names are of the form `XXX.xml` where XXX 
   is the passage ID. Please see [the UCCA resource webpage](http://www.cs.huji.ac.il/~oabend/ucca.html)
   for a software package for reading and using these files.
2. [`streusle2ucca.txt`](streusle2ucca.txt): mapping from document IDs used in the STREUSLE project
   (which are the same as the UD document IDs) to UCCA passage IDs.
3. [`scripts/get_ud.sh`](scripts/get_ud.sh): script to download all UD-annotated sentences corresponding
   to the UCCA passages in this corpus, rename them according to the UCCA IDs, and split the UCCA
   passages according to the UD sentences. The renamed UD files are saved in `ud`, and the split UCCA
   files in `sentences_by_ud`.