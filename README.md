# Common Voice Utils 

This repository collects together linguistic processing data for using dataset
dumps from the Common Voice project. It aims to provide a one-stop-shop for 
utilities and data useful in training ASR and TTS systems.

## Tools

* Phonemiser: A rudimentary grapheme to phoneme system based on a deterministic longest-match left-to-right replacements of orthographic units
* Validator: A validation script that can be used with `import_cv2.py` from [coqui-ai/STT](https://github.com/coqui-ai/STT/)
* Alphabet: The relevant alphabet of the language, appropriate for use in training ASR
* Segmenter: A deterministic sentence segmentation algorithm tuned for segmenting paragraphs from Wikipedia

## Language support 

| Language | Autonym   | Code | Code (CV) | Phonemiser | Validator | Alphabet | Segmenter |
|--------------------- |---------- |----- |------- |----------- |----------|---------- |------------|
| Abaza                | Абаза     |`abq` | `ab`   | ✔          | ✔         | ✔        |           |
| Arabic               |      |`ara` | `ar`   |            |           |          |            |
| Assamese             |      |`asm` | `as`   |            |           |          |            |
| Breton               | Brezhoneg |`bre` | `br`   | ✔          | ✔         | ✔        |      ✔     |
| Catalan              |      |`cat` | `ca`   |            |           |          |            |
| Czech                |      |`ces` | `cs`   |            |           |          |            |
| Hakha Chin           |      |`cnh` | `cnh`   |            |           |          |            |
| Chuvash              | Чӑвашла |`chv` | `cv`   | ✔          | ✔         | ✔        |      ✔     |
| Welsh                | Cymraeg     |`cym` | `cy`   |            |           |          |            |
| Dhivehi              | ދިވެހި |`div` | `dv`   | ✔          |        |      |         |
| Greek                | Ελληνικά |`ell` | `el`   | ✔          |        |      |         |
| German               | Deutsch     |`deu` | `de`   |            |           |          |            |
| English              | English     |`eng` | `en`   |            |           |          |            |
| Esperanto            | Esperanto     |`epo` | `eo`   |            |           |          |            |
| Spanish              | Español   |`spa` | `es`   |            |           |          |            |
| Estonian             | Eesti     |``    | `et`   |            |           |   ✔       |            |
| Basque               | Euskara   |`eus` | `eu`   |            |           |    ✔      |            |
| Persian              |           |`pes` | `fa`   |            |           |          |            |
| Finnish              | Suomi     |`fin` | `fi`   | ✔           |           |   ✔       |            |
| French               |      |`fra` | `fr`   |            |           |          |            |
| Frisian              |      |`` | `fy-NL`   |            |           |          |            |
| Irish                |      |`gle` | `ga-IE`   |            |           |    ✔      |            |
| Hindi                |      |`hin` | `hi`   |            |           |          |            |
| Upper Sorbian        |      |`` | `hsb`   |            |           |       ✔   |            |
| Hungarian            |      |`hun` | `hu`   |            |           |     ✔     |            |
| Interlingua          |      |`` | `ia`   |            |           |          |            |
| Indonesian           |      |`ind` | `id`   |            |           |     ✔     |            |
| Italian              |      |`ita` | `it`   |            |           |          |            |
| Japanese             |      |`jpn` | `ja`   |            |           |          |            |
| Georgian             |  ქართული ენა    |`kat` | `ka`   |    ✔          |           | ✔         |            |
| Kabyle               |      |`` | `kab`   |            |           |          |            |
| Kazakh               | Қазақша     |`kaz` | `kk`   |   ✔          |           |          |            |
| Kyrgyz               | Кыргызча     |`kir` | `ky`   |    ✔         |           |  ✔        |            |
| Luganda              |      |`` | `lg`   |            |           |          |            |
| Lithuanian           |      |`` | `lt`   |            |           |          |            |
| Latvian              |      |`` | `lv`   |            |           |          |            |
| Mongolian            | Монгол хэл |`khk` | `mn`   | ✔          |        |      |         |
| Maltese              |      |`mlt` | `mt`   |            |           |          |            |
| Dutch                |      |`nld` | `nl`   |            |           |          |            |
| Oriya                |      |`` | `or`   |            |           |          |            |
| Punjabi              |      |`pan` | `pa-IN`   |            |           |          |            |
| Polish               |      |`pol` | `pl`   |            |           |     ✔     |            |
| Portuguese           |      |`por` | `pt`   |            |           |     ✔     |            |
| Romansch (Sursilvan) |      |`` | `rm-sursilv`   |            |           |  ✔        |            |
| Romansch (Vallader)  |      |`` | `rm-vallader`   |            |           |   ✔       |            |
| Romanian             |      |`ron` | `ro`   |            |           |          |  ✔          |
| Russian              | Русский     |`rus` | `ru`   |            |           |     ✔     |            |
| Kinyarwanda          |      |`` | `rw`   |            |           |          |            |
| Sakha                | Саха тыла  |`sah` | `sah`   | ✔          |        |      |         |
| Slovenian            |      |`slv` | `sl`   |            |           |    ✔      |            |
| Swedish              | Svenska      |`swe` | `sv-SE`   |            |           |     ✔     |            |
| Tamil                | தமிழ்    |`tam` | `ta`   |            |           |          |            |
| Thai                 | ภาษาไทย     |`tha` | `th`   |    ✔        |           |     ✔     |            |
| Turkish              | Türkçe |`tur` | `tr`   |   ✔         |           |          |            |
| Tatar                | Татар теле |`tat` | `tt`   | ✔          |        |  ✔     |         |
| Ukrainian            |  Українська мова    |`ukr` | `uk`   |   ✔         |           |          |            |
| Vietnamese           |      |`vie` | `vi`   |            |           |          |            |
| Votic                |      |`vot` | `vot`   |            |           |          |            |
| Chinese (China)      |      |`cmn` | `zh-CN`   |            |           |          |            |
| Chinese (Hong Kong)  |      |`cmn` | `zh-HK`   |            |           |          |            |
| Chinese (Taiwan)     |      |`cmn` | `zh-TW`   |            |           |          |            |

## How to use it

### Grapheme to phoneme

```python
>>> from cvutils import Phonemiser
>>> p = Phonemiser('ab')
>>> p.phonemise('гӏапынхъамыз')
'ʕapənqaməz'

>>> p = Phonemiser('br')
>>> p.phonemise("implijout")
'impliʒut'
```

### Validator

```python
>>> from cvuilts import Validator
>>> v = Validator('ab')
>>> v.validate('Аллаҳ хаҵеи-ԥҳәыси иеилыхны, аҭыԥҳацәа роума иалихыз?')
'аллаҳ хаҵеи-ԥҳәыси иеилыхны аҭыԥҳацәа роума иалихыз'

>>> v = Validator('br')
>>> v.validate('Ha cʼhoant hocʼh eus da gendercʼhel da implijout ar servijer-mañ ?')
"ha c'hoant hoc'h eus da genderc'hel da implijout ar servijer-mañ"
```

### Sentence segmentation

```python
>>> from cvutils import Segmenter 
>>> s = Segmenter('br')
>>> para = "Peurliesañ avat e kemm ar vogalennoù e c'hengerioù evit dont da vezañ heñvel ouzh ar vogalennoù en nominativ (d.l.e. ar stumm-meneg), da skouer e hungareg: Aour, tungsten, zink, uraniom, h.a., a vez kavet e kondon Bouryatia. A-bouez-bras evit armerzh ar vro eo al labour-douar ivez pa vez gounezet gwinizh ha legumaj dreist-holl. A-hend-all e vez gounezet arc'hant dre chaseal ha pesketa."
>>> for sent in s.segment(para):
...     print(sent)
... 
Peurliesañ avat e kemm ar vogalennoù e c'hengerioù evit dont da vezañ heñvel ouzh ar vogalennoù en nominativ (d.l.e. ar stumm-meneg), da skouer e hungareg: Aour, tungsten, zink, uraniom, h.a., a vez kavet e kondon Bouryatia.
A-bouez-bras evit armerzh ar vro eo al labour-douar ivez pa vez gounezet gwinizh ha legumaj dreist-holl.
A-hend-all e vez gounezet arc'hant dre chaseal ha pesketa.
```

