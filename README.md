# w266 NLP - Final Project

Project proposal: https://docs.google.com/document/d/1vxy1xuW_0xpjkGAO3S1E3Jl0cB2AYbAltI0a6nj8S9A/edit

Links to related papers, repos, and other resources we looked at:
* Drawing a DAG: http://fozziethebeat.github.io/blog/2012/08/12/building-a-phrase-graph/
* Data Source: https://github.com/fictivekin/openrecipes, https://s3.amazonaws.com/openrecipes/20170107-061401-recipeitems.json.gz
* Alternate Data Source (Epicurious): https://github.com/AlliedToasters/EpicuriousRecipes/blob/master/full_format_recipes.json
* Parsers: https://github.com/dpapathanasiou/recipebook, https://github.com/hhursev/recipe-scrapers
* Semantic Parsing: https://en.wikipedia.org/wiki/Semantic_parsing
* Papers: https://dspace.mit.edu/handle/1721.1/113147, https://bir.brandeis.edu/bitstream/handle/10192/34135/ChenThesis2017.pdf?sequence=3&isAllowed=y

### work in progress paper
* https://www.overleaf.com/17863614zxfgdwycnbkq

### data files
* layer1.json.[0-9].valid.gz - pickled and in json format 

### notebooks
* 'preprocessing_json.ipynb' - we used recipes collected by MIT's PicToRecipe project. We broke the 1 million recipes into 10 parts and pickled them so we can selectively load them into panda dataframes. 
* 'eda.ipynb' - we explored the recipes to get a sense what information they contained and in what format 
* 'spacy_parser.ipynb' - we explored building a parser tree using spacy and NER using existing trained model
* 'spacy_parser_alt1.ipynb' - evaluate syntatic parsing on 1st step of 10 rather simple recipes (<=5 instructional steps)

### additional scripts
* spacy_install.md - install spaCy with conda
* explacy.py - A small tool that EXPLains spACY parse results; https://github.com/tylerneylon/explacy
