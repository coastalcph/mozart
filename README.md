# MozArt
MozArt: a multilingual dataset of parallel cloze examples with annotator demographics.


The data is provided in individual JSONL files per language {lang}_data_with_annotations.jsonl, where {lang} denotes the ISO 639-1 code of each language (en, es, de, fr). Each line of the JSONL corresponds to one sentence completed by one annotator with the following information:

<pre>
<b>s_id</b>: str,  				sentence indentifier
<b>text</b>: str,  				sentence text
<b>true_mask</b>: str,  			word masked in the sentence
<b>tag</b>: str,  				part-of-speech of the word masked
<b>mask</b>: str,  				word given by the annotator to fill in the gap
<b>u_id</b>: str,  				annotator identifier 
<b>native</b>: int,   				binary variable; 1: the annotator is a native speaker of the target language, 0: otherwise
<b>nonnative</b>: int,  			binary variable; 1: the annotator isn't a native speaker of the target language, 0: otherwise
<b>male</b>: int,  				binary variable; 1: the annotator is a male (self-reported), 0: otherwise
<b>female</b>: int,   				binary variable; 1: the annotator is a female (self-reported), 0: otherwise
<b>age</b>: int,  				annotator's age at the time of completion
<b>country_of_birth</b>: str,  		annotator's country of birth
<b>current_country_of_residence</b>: str,	annotator's current country of residence at the time of completion
<b>first_language</b>: str,  			annotator's first language
<b>fluent_languages</b>: List[str],  		list of languages that the annotator has reported to be fluent in
<b>nationality</b>: str,  			annotator's nationality
<b>time_taken</b>: float  			time taken to complete the task (ms)
</pre>

Note that the attributes that were not provided voluntarily are filled with 'null'.

This work is licensed under the Creative Commons Attribution 4.0 International License. To view a copy of this license, visit http://creativecommons.org/licenses/by/4.0/ 

If you use our dataset, please cite:
```
@inproceedings{cabello2022pretrained,
  title={Are Pretrained Multilingual Models Equally Fair Across Languages?},
  author={Cabello Piqueras, Laura and S{\o}gaard, Anders},
  booktitle={COLING 2022},
  year={2022}
}
```

Main resources: 

* Philipp Koehn, 2005. [Europarl: A parallel corpus for statistical machine translation](https://aclanthology.org/2005.mtsummit-papers.11/). In Proceedings of Machine Translation Summit X: Papers, pages 79–86, Phuket, Thailand.  
* Philipp Koehn and Christof Monz. 2006. [Manual and automatic evaluation of machine translation between European languages](https://aclanthology.org/W06-3114/). In Proceedings on the Workshop on Statistical Machine Translation, pages 102–121, New York City. Association for Computational Linguistics.
	* [Shared task](https://www.statmt.org/wmt06/shared-task/) of the NAACL 2006 Workshop on Statistical Machine Translation
