# MozArt
MozArt: a multilingual dataset of parallel cloze examples with annotator demographics.



The data is provided in individual JSONL files per language {lang}_data_with_annotations.jsonl, where {lang} denotes the ISO 639-1 code of each language (en, es, de, fr). Each line of the JSONL corresponds to one sentence completed by one annotator with the following information:

<pre>
<b>s_id</b>: str,  
<b>text</b>: str,  
<b>true_mask</b>: str,  
<b>tag</b>: str,  
<b>mask</b>: str,  
<b>u_id</b>: str,  
<b>native</b>: int,   
<b>nonnative</b>: int,  
<b>male</b>: int,  
<b>female</b>: int,   
<b>age</b>: int,  
<b>country_of_birth</b>: str,  
<b>current_country_of_residence</b>: str,  
<b>first_language</b>: str,  
<b>fluent_languages</b>: List[str],  
<b>nationality</b>: str,  
<b>time_taken</b>: float  
</pre>

Note that the attributes that were not provided voluntarily are filled with 'null'.

This work is licensed under the Creative Commons Attribution 4.0 International License. To view a copy of this license, visit http://creativecommons.org/licenses/by/4.0/ 

If you use our dataset, please cite:
```
Are Pretrained Multilingual Models Equally Fair Across Languages? (to appear in COLING 2022)
Authors: Laura Cabello Piqueras, Anders Søgaard
```

Main resources: 

* Philipp Koehn, 2005. [Europarl: A parallel corpus for statistical machine translation](https://aclanthology.org/2005.mtsummit-papers.11/). In Proceedings of Machine Translation Summit X: Papers, pages 79–86, Phuket, Thailand.  
* Philipp Koehn and Christof Monz. 2006. [Manual and automatic evaluation of machine translation between European languages](https://aclanthology.org/W06-3114/). In Proceedings on the Workshop on Statistical Machine Translation, pages 102–121, New York City. Association for Computational Linguistics.
	* [Shared task](https://www.statmt.org/wmt06/shared-task/) of the NAACL 2006 Workshop on Statistical Machine Translation
