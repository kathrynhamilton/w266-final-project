# w266 NLP - Final Project 
(please do not release our report publicly)

### paper
* https://www.overleaf.com/17863614zxfgdwycnbkq

### slides
* https://docs.google.com/presentation/d/1gzrug2b9f24UqS0a-X-I-n__R9nA4UIOofjTO9SSH0c/edit?usp=sharing

### data files
* layer1.json.[0-9].valid.gz - pickled and in json format 
* patterns.jsonl - initial seeding word lists are in the ner_playground notebook, this file stores boosted patterns post bootstrapping 

### notebooks
* please view the following notebooks with nbviewer by modifying the file path below:
http://nbviewer.jupyter.org/github/kathrynhamilton/w266-final-project/blob/master/<file.ipynb>
* 'preprocessing_json.ipynb' - we used recipes collected by MIT's [PicToRecipe](http://pic2recipe.csail.mit.edu/) project. We broke the 1 million recipes into 10 parts and pickled them so we can selectively load them into panda dataframes. 
* 'eda.ipynb' - we explored the recipes to get a sense what information they contained and in what format 
* 'spacy_parser.ipynb' - we explored building a parser tree using spacy and NER using existing trained model
* 'spacy_parser_alt1.ipynb' - evaluate syntatic parsing on 1st step of 10 rather simple recipes (<=5 instructional steps)
* 'ner_playground.ipynb' - let's us explore bootstrapping and named entity recognition task

### custom model
* ./NER_Model - directory of model artifacts; including splitted training and evaluation data
* 'ner_manual_train.jsonl' - fully annotated training dataset, annotations are facilitated using Prodigy web UI

### additional scripts
* 'spacy_install.md' - install spaCy with conda, remember to download english language models; spacy_lookup and prodigy are added as well
* 'explacy.py' - visualize spaCy's dependency parser results; https://github.com/tylerneylon/explacy

### milestone references

Project proposal: https://docs.google.com/document/d/1vxy1xuW_0xpjkGAO3S1E3Jl0cB2AYbAltI0a6nj8S9A/edit

Links to related papers, repos, and other resources we looked at:
* Drawing a DAG: http://fozziethebeat.github.io/blog/2012/08/12/building-a-phrase-graph/
* Data Source: https://github.com/fictivekin/openrecipes, https://s3.amazonaws.com/openrecipes/20170107-061401-recipeitems.json.gz
* Alternate Data Source (Epicurious): https://github.com/AlliedToasters/EpicuriousRecipes/blob/master/full_format_recipes.json
* Parsers: https://github.com/dpapathanasiou/recipebook, https://github.com/hhursev/recipe-scrapers
* Semantic Parsing: https://en.wikipedia.org/wiki/Semantic_parsing
* Papers: https://dspace.mit.edu/handle/1721.1/113147, https://bir.brandeis.edu/bitstream/handle/10192/34135/ChenThesis2017.pdf?sequence=3&isAllowed=y
