# [CA] Model pel processament del llenguatge natural en Català per a spaCy

Model per a [spaCy](https://spacy.io) de la llengua catalana generat a partir de:

- Vectors de paraules de [fastText](https://github.com/facebookresearch/fastText/blob/master/docs/crawl-vectors.md)
- Gramàtica, morfologia i sintaxi fent servir dades del corpus d'[AnCora](https://github.com/UniversalDependencies/UD_Catalan-AnCora)
- Annotacions per a l'extracció d'entitats derivades de la wikipedia ([Cross-lingual Name Tagging and Linking for 282 Languages](http://nlp.cs.rpi.edu/paper/282elisa2017.pdf))

Els models es poden descarregar a la secció Publicacions (Releases).

## Instal·lació i ús

Podeu escollir entre dos models. El model gran és més precís però com que spaCy carrega tot el model a memòria assegureu-vos de tenir-ne suficient.

| Dada | Mitjà | Gran |
|---|---|---|
| Nom | `ca_fasttext_wiki_md` | `ca_fasttext_wiki_lg` |
| Versió | `1.0.0` | `1.0.0` |
| spaCy | `>=2.3.2`,`<2.4.0`| `>=2.3.2`,`<2.4.0`|
| Mida | 62 MB| 1,16 GB |
| Pipeline | `tagger`, `parser`, `ner` | `tagger`, `parser`, `ner` |
| Vectors | 20.000 | 2.000.000 |
| Llicència | `AGPL-3.0` |`AGPL-3.0` |
| Autor | Ciaran O'Reilly |Ciaran O'Reilly |

Podeu instal·lar el model i fer-lo servir amb spaCy executant les següents ordres a l'interfície de línia d'ordres:

```sh
# Per instal·lar el model mitjà
> pip install https://github.com/ccoreilly/spacy-catala/releases/download/ca_fasttext_wiki_md-1.0.0/ca_fasttext_wiki_md-1.0.0-py3-none-any.whl
> python -m spacy link ca_fasttext_wiki_md ca

# Per instal·lar el model gran
> pip install https://github.com/ccoreilly/spacy-catala/releases/download/ca_fasttext_wiki_lg-1.0.0/ca_fasttext_wiki_lg-1.0.0-py3-none-any.whl
> python -m spacy link ca_fasttext_wiki_lg ca
```

# [EN] spaCy NLP Model for the Catalan language

spaCy NLP model for the Catalan language generated from:

- [fastText](https://github.com/facebookresearch/fastText/blob/master/docs/crawl-vectors.md) word vectors
- The [AnCora](https://github.com/UniversalDependencies/UD_Catalan-AnCora) corpus for parts of speech, morphological features, and syntactic dependencies.
- Wikipedia annotations for named entity extraction ([Cross-lingual Name Tagging and Linking for 282 Languages](http://nlp.cs.rpi.edu/paper/282elisa2017.pdf))

Models can be found in the releases section of the repository.
## Installing and using the model

You can choose between two models. The larger one is more accurate but make sure to have enough memory as spaCy will load the whole model into it.

| Dada | Medium | Large |
|---|---|---|
| Name | `ca_fasttext_wiki_md` | `ca_fasttext_wiki_lg` |
| Version | `1.0.0` | `1.0.0` |
| spaCy | `>=2.3.2`,`<2.4.0`| `>=2.3.2`,`<2.4.0`|
| Size | 62 MB| 1,16 GB |
| Pipeline | `tagger`, `parser`, `ner` | `tagger`, `parser`, `ner` |
| Vectors | 20.000 | 2.000.000 |
| License | `AGPL-3.0` |`AGPL-3.0` |
| Author | Ciaran O'Reilly |Ciaran O'Reilly |

```sh
# To install the medium sized model
> pip install https://github.com/ccoreilly/spacy-catala/releases/download/ca_fasttext_wiki_md-1.0.0/ca_fasttext_wiki_md-1.0.0-py3-none-any.whl
> python -m spacy link ca_fasttext_wiki_md ca

# To install the larger model
> pip install https://github.com/ccoreilly/spacy-catala/releases/download/ca_fasttext_wiki_lg-1.0.0/ca_fasttext_wiki_lg-1.0.0-py3-none-any.whl
> python -m spacy link ca_fasttext_wiki_lg ca
```