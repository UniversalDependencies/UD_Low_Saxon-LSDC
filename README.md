# Summary

The UD Low Saxon LSDC dataset consists of sentences in 8 major Low Saxon dialect groups from both Germany and the Netherlands. These sentences are (or are to become) part of the LSDC dataset and represent the language from mostly the 19th and early 20th century in genres such as short stories, novels, speeches, letters and fairytales. 


# Introduction

The first version of the UD Low Saxon LSDC dataset contained 18 Low Saxon (sub-)dialects from both Germany and the Netherlands represented by 2 sentences each and belonging to the domains of short stories, novels, speeches, letters and fairytales. Each sentence was chosen from a different text to present some of the variation within the different dialect groups. In the second version, 40 sentences from four Westphalian dialects, two from Germany and two from the Netherlands, were added. The coverage of other dialect groups will be improved in future releases. For the third version, we have raised the number of sentences to 190 and made slight modifications to the subgrouping of the dialects. The **current fourth version** of the dataset contains 1,000 sentences, of which 500 are placed in the train and 500 in the test set. The dialect distribution between the train and the test set is not balanced yet and we plan to improve this in future releases.

The major dialect group is shown as the third segment of the sentence ID. The following dialects are included:
* BRA = Brandenburgish
* DNS = German North Saxon
* DWF = German Westphalian
* MVP = Mecklenburgish – West Pomeranian
* NNS = Dutch North Saxon
* NPR = Low Prussian
* NWF = Dutch Westphalian
* OFL = Eastphalian

Since there is no official interregional spelling, the interregional spelling suggestion used by e.g. the Dutch Low Saxon Wikipedia (_Nysassiske Skryvwyse_, described in more detail here: https://skryvwyse.eu/ (only in Low Saxon)) is used as a compromise for normalisation, but the original spelling of the source is included in the line "text_orig =" and a Middle Low Saxon lemma is added in the tenth column ("lemma_gml=xxx") in order to make the Modern Low Saxon data more easily comparable with the Middle Low Saxon data in the reference corpus "Referenzkorpus Mittelniederdeutsch/Niederrheinisch". For this reason, the Middle Low Saxon lemma forms largely follow the "Mittelniederdeutsches Handwörterbuch" by Agathe Lasch et al. like in the reference corpus. Middle Low Saxon lemmata are only added in the cases where there is an attestation in Middle Low Saxon, i.e. the word is either listed in the Handwörterbuch or is found in the reference corpus. Middle Low Saxon lemmata are still included if the word's meaning has changed, an in addition, we have done our best to create new complex word lemmata from known simplex words and reconstruct potential Middle Low Saxon forms for words which have not yet been attested at that stage of the language. The last few hundred sentences in the train set either do not contain Middle Low Saxon lemmata yet or they have been done automatically. 

The first version of the dataset contained only sentences from copyright-free material from the 19th and early 20th century. Part of the sentences are already included in the first release of the LSDC dataset found here: https://github.com/Helsinki-NLP/LSDC/ See there for further information on the origin of the data. The other sentences originate mostly from Joh. A. Leopold's work 'Van de Schelde tot te Weichsel', a digitised version of which is accessible here: https://www.dbnl.org/titels/titel.php?id=leop008sche00 An exception constitutes the text 'Krisjaon Klaover' to be found in the Twentse Taalbank: http://www.twentsetaalbank.nl/docs/TWA.1894-Heinink-Krisjaon_Klaover-150.pdf These other sentences will be added to the next release of the LSDC dataset. Starting from the third version, the dataset also contains a few sentences from works by modern authors from which we have received permission to include small parts of their work in annotated corpora.


# Acknowledgments

The following people were involved in the creation of this dataset:

* Janine Siewert (data collection, selection and annotation)
* Jack Michael Rueter (annotation-related advice) 

## References

If you use this treebank, please cite this paper:

```
@inproceedings{siewert-rueter-2024,
  author    = {Siewert, Janine and Rueter, Jack},
  title     = {{The Low Saxon LSDC Dataset at Universal Dependencies}},
  booktitle = {Proceedings of the 2024 Joint International Conference on Computational
               Linguistics, Language Resources and Evaluation},
  series    = {LREC-COLING 2024},
  year      = {2024},
  month     = {05},
  address   = {Torino, Italia},
  organization = {ELRA Language Resources Association (ELRA) and the
                  International Committee on Computational Linguistics
                  (ICCL)},
  pubstate  = {forthcoming},
  note      = {accepted}
}
```
### References used for the creation of this dataset: 

* Lasch, Agathe et al. 1928 ff. *Mittelniederdeutsches Handwörterbuch.* Neumünster: Wachholtz.
* ReN-Team. 2019. *Referenzkorpus Mittelniederdeutsch/Niederrheinisch (1200-1650).* Archived in Hamburger Zentrum für Sprachkorpora. Version 1.0. Publication date 2019-08-14. http://hdl.handle.net/11022/0000-0007-D829-8.


# Changelog

* 2021-05-15 v2.8
  * Initial release in Universal Dependencies.


<pre>
=== Machine-readable metadata (DO NOT REMOVE!) ================================
Data available since: UD v2.8
License: CC BY-SA 4.0
Includes text: yes
Genre: fiction nonfiction
Lemmas: manual native
UPOS: manual native
XPOS: manual native
Features: manual native
Relations: manual native
Contributors: Siewert, Janine
Contributing: elsewhere
Contact: janine.siewert@helsinki.fi
===============================================================================
</pre>
