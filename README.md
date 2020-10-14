# [CA] Model pel processament del llenguatge natural en Català per a spaCy

Model per a [spaCy](https://spacy.io) de la llengua catalana generat a partir de:

- Vectors de paraules de [fastText](https://github.com/facebookresearch/fastText/blob/master/docs/crawl-vectors.md)
- Gramàtica, morfologia i sintaxi fent servir dades del corpus d'[AnCora](https://github.com/UniversalDependencies/UD_Catalan-AnCora)
- Annotacions per a l'extracció d'entitats derivades de la wikipedia ([Cross-lingual Name Tagging and Linking for 282 Languages](http://nlp.cs.rpi.edu/paper/282elisa2017.pdf))

Degut a la mida final del model (2.5GB) i dels vectors de paraules (1.1GB) aquests no s'inclouen al repositori però podeu descarregar-vos el model final a la secció Publicacions (Releases).

## Instal·lació i ús

Podeu instal·lar el model i fer-lo servir amb spaCy executant les següents ordres a l'interfície de línia d'ordres:

```sh
> pip install https://github.com/ccoreilly/spacy-catala/releases/download/1.0.0/ca_fasttext_wiki_md-1.0.0-py3-none-any.whl
> python -m spacy link ca_fasttext_wiki_md ca
```

# [EN] spaCy NLP Model for the Catalan language

spaCy NLP model for the Catalan language generated from:

- [fastText](https://github.com/facebookresearch/fastText/blob/master/docs/crawl-vectors.md) word vectors
- The [AnCora](https://github.com/UniversalDependencies/UD_Catalan-AnCora) corpus for parts of speech, morphological features, and syntactic dependencies.
- Wikipedia annotations for named entity extraction ([Cross-lingual Name Tagging and Linking for 282 Languages](http://nlp.cs.rpi.edu/paper/282elisa2017.pdf))
-

The final model is around 2.5GB and the fastText vectors over 1GB which is why they are not included in this repository. You can download the model under the Releases tab.

## Installing and using the model

You can install and use the model in spaCy by executing the following commands:

```sh
> pip install https://github.com/ccoreilly/spacy-catala/releases/download/1.0.0/ca_fasttext_wiki_md-1.0.0-py3-none-any.whl
> python -m spacy link ca_fasttext_wiki_md ca
```
