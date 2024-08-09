# Irish-English Speech Translation Shared Task Data@IWSLT-2023 and 2024

# Introduction
Irish (also known as Gaeilge) has around 170,000 L1 speakers and “1.85 million (37%) people across the island (of Ireland) claim to be at least somewhat proficient with the language”. In the Republic of Ireland, it is the national and first official language. It is also one of the official languages of the European Union and a recognized minority language in Northern Ireland with the ISO ``ga`` code.

IWSLT participants may obtain the Irish-English speech translation data from [here](https://github.com/shashwatup9k/iwslt2023_ga-en). The audio data consists of the [common voice](https://commonvoice.mozilla.org/en) and [Idlak](https://github.com/Idlak/Living-Audio-Dataset). You can sign [this form](https://forms.gle/N6KvepNo6gs8BpF56) for further updates. This corpus consists of approximately 10 hours of audio speech data and translations into English text.

We point participants to additional Irish pre-trained models (the models are trained on a common voice dataset), parallel and monolingual corpora from here:

- [wav2vec 2.0/wav2vec 2.0 (XLSR) ](https://github.com/facebookresearch/fairseq/tree/main/examples/wav2vec#pre-trained-models)
- [Opus Irish-English parallel and monolingual dataset](https://opus.nlpl.eu/results/ga&en/corpus-result-table)
- [Irish-English and English-Irish parallel COVID dataset](https://github.com/loresmt/loresmt-2021)

**NB!** The training dataset has duplicate segments due to gender and age variety.  In addition, please note that the 2024 test dataset will be from the radio news domain. 

[April 2 Update:] THE TEST DATA FOR 2024 IS NOW AVAILABLE [HERE](https://github.com/shashwatup9k/iwslt2023_ga-eng/tree/main/test-2024)

## Structure of the ` Shared Task data`:
```
ga-eng-iwslt2023/
├─ data/
│  ├─ train/
│     └─ stamped.tsv
│     └─ txt/
│        └─ train.eng
│     └─ wav/
│  ├─ dev/
│     └─ stamped.tsv
│     └─ txt/
│        └─ dev.eng
│     └─ wav/
│  ├─ test-2023/
│     └─ stamped.tsv
│     └─ txt/
│        └─ test.eng
│     └─ wav
│  ├─ test-2024 (only audio files for the IWSLT 2024 evaluation campaign)/
│     └─ stamped.tsv
│     └─ wav/
├─ LICENSE.md
├─ README.md
   
```
The latest data statistics are presented below:
-----------------------------------------------------
```
│ Language	       |Total_audios | Total_translatedSentences │ 
│Irish↔English (train) │  7478       │  7478            		│
│Irish↔English (dev)   │  1120       │  1120           		│
│Irish↔English (test-2023)  │  347        │  347            		│
│Irish↔English (test-2024)  │  614        │  -            		│
```

# License
Please see the [LICENSE](https://github.com/shashwatup9k/iwslt2023_ga-en/blob/main/LICENSE) file.

# Acknowledgments
We would like to thank [Science Foundation Ireland (SFI)](https://www.sfi.ie/) [(grant number SFI/12/RC/2289_ P2 Insight _ 2)](https://www.insight-centre.org/) and [ADAPT Centre](https://www.adaptcentre.ie/). We would also like to thank RTÉ/TG4 for providing the Irish-English speech data. 
## Citation
## References
<pre>
   @inproceedings{ahmad-etal-2024-findings,
    title = "{FINDINGS} {OF} {THE} {IWSLT} 2024 {EVALUATION} {CAMPAIGN}",
    author = {Ahmad, Ibrahim Said  and
      Anastasopoulos, Antonios  and
      Bojar, Ond{\v{r}}ej  and
      Borg, Claudia  and
      Carpuat, Marine  and
      Cattoni, Roldano  and
      Cettolo, Mauro  and
      Chen, William  and
      Dong, Qianqian  and
      Federico, Marcello  and
      Haddow, Barry  and
      Javorsk{\'y}, D{\'a}vid  and
      Krubi{\'n}ski, Mateusz  and
      Kim Lam, Tsz  and
      Ma, Xutai  and
      Mathur, Prashant  and
      Matusov, Evgeny  and
      Maurya, Chandresh  and
      McCrae, John  and
      Murray, Kenton  and
      Nakamura, Satoshi  and
      Negri, Matteo  and
      Niehues, Jan  and
      Niu, Xing  and
      Ojha, Atul Kr.  and
      Ortega, John  and
      Papi, Sara  and
      Pol{\'a}k, Peter  and
      Posp{\'\i}{\v{s}}il, Adam  and
      Pecina, Pavel  and
      Salesky, Elizabeth  and
      Sethiya, Nivedita  and
      Sarkar, Balaram  and
      Shi, Jiatong  and
      Sikasote, Claytone  and
      Sperber, Matthias  and
      St{\"u}ker, Sebastian  and
      Sudoh, Katsuhito  and
      Thompson, Brian  and
      Waibel, Alex  and
      Watanabe, Shinji  and
      Wilken, Patrick  and
      Zem{\'a}nek, Petr  and
      Zevallos, Rodolfo},
    editor = "Salesky, Elizabeth  and
      Federico, Marcello  and
      Carpuat, Marine",
    booktitle = "Proceedings of the 21st International Conference on Spoken Language Translation (IWSLT 2024)",
    month = aug,
    year = "2024",
    address = "Bangkok, Thailand (in-person and online)",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2024.iwslt-1.1",
    pages = "1--11",
    abstract = "This paper reports on the shared tasks organized by the 21st IWSLT Conference. The shared tasks address 7 scientific challenges in spoken language translation: simultaneous and offline translation, automatic subtitling and dubbing, speech-to-speech translation, dialect and low-resource speech translation, and Indic languages. The shared tasks attracted 17 teams whose submissions are documented in 27 system papers. The growing interest towards spoken language translation is also witnessed by the constantly increasing number of shared task organizers and contributors to the overview paper, almost evenly distributed across industry and academia.",
}
</pre>
<pre>
@inproceedings{agrawal-etal-2023-findings,
    title = "{FINDINGS} {OF} {THE} {IWSLT} 2023 {EVALUATION} {CAMPAIGN}",
    author = {Agarwal, Milind  and
      Agrawal, Sweta  and
      Anastasopoulos, Antonios  and
      Bentivogli, Luisa  and
      Bojar, Ond{\v{r}}ej  and
      Borg, Claudia  and
      Carpuat, Marine  and
      Cattoni, Roldano  and
      Cettolo, Mauro  and
      Chen, Mingda  and
      Chen, William  and
      Choukri, Khalid  and
      Chronopoulou, Alexandra  and
      Currey, Anna  and
      Declerck, Thierry  and
      Dong, Qianqian  and
      Duh, Kevin  and
      Est{\`e}ve, Yannick  and
      Federico, Marcello  and
      Gahbiche, Souhir  and
      Haddow, Barry  and
      Hsu, Benjamin  and
      Mon Htut, Phu  and
      Inaguma, Hirofumi  and
      Javorsk{\'y}, D{\'a}vid  and
      Judge, John  and
      Kano, Yasumasa  and
      Ko, Tom  and
      Kumar, Rishu  and
      Li, Pengwei  and
      Ma, Xutai  and
      Mathur, Prashant  and
      Matusov, Evgeny  and
      McNamee, Paul  and
      P. McCrae, John  and
      Murray, Kenton  and
      Nadejde, Maria  and
      Nakamura, Satoshi  and
      Negri, Matteo  and
      Nguyen, Ha  and
      Niehues, Jan  and
      Niu, Xing  and
      Kr. Ojha, Atul  and
      E. Ortega, John  and
      Pal, Proyag  and
      Pino, Juan  and
      van der Plas, Lonneke  and
      Pol{\'a}k, Peter  and
      Rippeth, Elijah  and
      Salesky, Elizabeth  and
      Shi, Jiatong  and
      Sperber, Matthias  and
      St{\"u}ker, Sebastian  and
      Sudoh, Katsuhito  and
      Tang, Yun  and
      Thompson, Brian  and
      Tran, Kevin  and
      Turchi, Marco  and
      Waibel, Alex  and
      Wang, Mingxuan  and
      Watanabe, Shinji  and
      Zevallos, Rodolfo},
    editor = "Salesky, Elizabeth  and
      Federico, Marcello  and
      Carpuat, Marine",
    booktitle = "Proceedings of the 20th International Conference on Spoken Language Translation (IWSLT 2023)",
    month = jul,
    year = "2023",
    address = "Toronto, Canada (in-person and online)",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2023.iwslt-1.1",
    doi = "10.18653/v1/2023.iwslt-1.1",
    pages = "1--61",
    abstract = "This paper reports on the shared tasks organized by the 20th IWSLT Conference. The shared tasks address 9 scientific challenges in spoken language translation: simultaneous and offline translation, automatic subtitling and dubbing, speech-to-speech translation, multilingual, dialect and low-resource speech translation, and formality control. The shared tasks attracted a total of 38 submissions by 31 teams. The growing interest towards spoken language translation is also witnessed by the constantly increasing number of shared task organizers and contributors to the overview paper, almost evenly distributed across industry and academia.",
}
</pre>
<pre>
=== Machine-readable metadata (DO NOT REMOVE!) =====================================================
Data available since: Irish-English Speech Translation Shared Task@IWSLT-2023 and 2024
License: CC BY-NC-SA 4.0
=======
Includes text/audio: yes
Shared Task Organisers 2023: Ojha, Atul Kr.; Judge, John; McCrae, John P.
Shared Task Organisers 2024: Ojha, Atul Kr.; McCrae, John P.
Contact: atulkumar.ojha@insight-centre.org, shashwatup9k@gmail.com
Contributor/&copy;holder: Insight Centre for Data Analytics, Data Science Institute, University of Galway, Ireland and ADAPT Centre, Ireland
=======================================================================================================
</pre>
