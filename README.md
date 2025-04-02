# Instruction datasets

Collection of synthetic instruction datasets used during the instruction pretraining of Model-small-instr-1, Model-small-instr-2 and Model-small-instr-3.

## Dataset creation

Datasets were created using two different techniques:

- Adapting already existing datasets or corpora by modifying their format to make them suitable for the instruction pretraining. 
- Creating the dataset from scratch by using a LLM ([Salamandra-7B](https://huggingface.co/BSC-LT/salamandra-7b-instruct)) to generate diverse instructions based on existing data.

## Dataset information

The following table presents the basic information of each dataset.

| Language | Dataset Name                                | Type                              | Entries  | Creation Method     | File Size (MB) | License                |
|----------|--------------------------------------------|-----------------------------------|----------|--------------------|---------------|------------------------|
| GL       | EGU (Enciclopedia Galega Universal)       | Encyclopedic Knowledge           | 47,396   | Manually Adapted   | 33.00         | CC BY-SA 4.0          |
| GL       | MT (GL - ES)                              | Translations                     | 275,292  | Manually Adapted   | 101.00        | CC BY-SA 4.0          |
| GL       | MT (GL - EN)                              | Translations                     | 421,974  | Manually Adapted   | 101.00        | CC BY-SA 4.0          |
| GL       | SLI NER                                   | Named Entity Recognition         | 8,138    | Manually Adapted   | 2.40          | CC BY 4.0             |
| GL       | GalCoLA                                   | Orthographic Correction          | 8,160    | Manually Adapted   | 1.90          | CC BY-SA 4.0          |
| GL       | SLI PoS TAGGING                           | Morphological Analysis           | 46,864   | Manually Adapted   | 45.15         | CC BY 4.0             |
| GL       | Wikipedia Multiple-Choice QA             | QA Multiple-choice               | 1,486    | LLM-Generated      | 1.60          | CC BY-SA 4.0          |
| GL       | CódigoCero Summarization                 | Summarization                    | 342      | LLM-Generated      | 1.60          | CC BY-SA 4.0          |
| PT       | Wikipedia Multiple-Choice QA             | QA Multiple-choice               | 547      | LLM-Generated      | 0.59          | CC BY-SA 4.0          |
| PT       | Extraglue-Instruct (Boolean Questions)   | QA Simple                        | 28,281   | Manually Adapted      | 25.00         | MIT License           |
| PT       | Extraglue-Instruct (CB)                  | Concept Bottleneck               | 1,500    | Manually Adapted       | 1.20          | MIT License           |
| PT       | Extraglue-Instruct (MultiRC)             | Reading Comprehension            | 108,972  | Manually Adapted       | 221.00        | MIT License           |
| PT       | Extraglue-Instruct (STSB)                | Text Similarity                  | 22,996   | Manually Adapted      | 18.00         | MIT License           |
| PT       | Extraglue-Instruct (WNLI)                | NLI (Inference)                  | 3,810    | Manually Adapted       | 2.40          | MIT License           |
| PT       | Aya (Train)                               | QA Simple                        | 8,997    | Manually Adapted     | 3.00          | Apache License 2.0    |
| PT       | OpenAssistant                            | Chat / Assistant                 | 287      | Manually Adapted   | 1.90          | Apache License 2.0    |
| EN       | Natural Instructions - NER               | Named Entity Recognition         | 1,574    | Manually Adapted   | 1.20          | Apache License 2.0    |
| EN       | QASC                                     | QA Multiple-choice               | 9,980    | Manually Adapted   | 8.90          | CC BY 4.0             |
| EN       | OpenAssistant                            | Chat / Assistant                 | 154      | Manually Adapted   | 1.20          | Apache License 2.0    |
| ES       | ALEXSIS                                  | Linguistic Simplification        | 3,918    | Manually Adapted   | 2.20          | CC BY-NC-SA 4.0       |
| ES       | COAH                                     | Sentiment Analysis               | 1,816    | Manually Adapted   | 1.60          | CC BY-NC-SA 4.0       |
| ES       | COAR                                     | Sentiment Analysis               | 2,202    | Manually Adapted   | 1.30          | CC BY-NC-SA 4.0       |



## Disclaimer and limitations

Some datasets were not included due to license restrictions, meaning they cannot be publicly shared or redistributed. The datasets included in this repository follow various licenses, such as CC BY-SA 4.0, CC BY 4.0, CC-BY-NC-ND 4.0, Apache License 2.0, and MIT License.

Users should ensure they comply with the respective licenses when using these datasets. If a dataset requires attribution, non-commercial use, or has other restrictions, those conditions must be respected. For more details on specific license terms, please refer to the official documentation or the original data sources.

## Acknowledgements

These datasets were developed and compiled within the Nós Project, funded by the Ministerio para la Transformación Digital y de la Función Pública - Funded by EU – NextGenerationEU within the framework of the [project ILENIA] (https://proyectoilenia.es/) with reference 2022/TL22/00215336. 

## Citations

```bibtex
@incollection{Molina-Gonzalez2014,
  author    = {M. D. Molina-González and E. Martínez-Cámara and M. T. Martín-Valdivia and L. A. Ureña-López},
  title     = {Cross-domain sentiment analysis using Spanish opinionated words},
  booktitle = {Natural Language Processing and Information Systems},
  volume    = {8455},
  pages     = {214--219},
  publisher = {Springer International Publishing},
  year      = {2014},
  doi       = {10.1007/978-3-319-07983-7_28},
}

@inproceedings{naturalinstructions,
  title={Cross-task generalization via natural language crowdsourcing instructions},
  author={Mishra, Swaroop and Khashabi, Daniel and Baral, Chitta and Hajishirzi, Hannaneh},
  booktitle={ACL},
  year={2022}
}

```bibtex
@inproceedings{supernaturalinstructions,
  title={Super-NaturalInstructions:Generalization via Declarative Instructions on 1600+ Tasks},
  author={Wang, Yizhong and Mishra, Swaroop and Alipoormolabashi, Pegah and Kordi, Yeganeh and Mirzaei, Amirreza and Arunkumar, Anjana and Ashok, Arjun and Dhanasekaran, Arut Selvan and Naik, Atharva and Stap, David and others},
  booktitle={EMNLP},
  year={2022}
}

@article{allenai:qasc,
      author    = {Tushar Khot and Peter Clark and Michal Guerquin and Peter Jansen and Ashish Sabharwal},
      title     = {QASC: A Dataset for Question Answering via Sentence Composition},
      journal   = {arXiv:1910.11473v2},
      year      = {2020},
}

@misc{köpf2023openassistantconversationsdemocratizing,
      title={OpenAssistant Conversations -- Democratizing Large Language Model Alignment}, 
      author={Andreas Köpf and Yannic Kilcher and Dimitri von Rütte and Sotiris Anagnostidis and Zhi-Rui Tam and Keith Stevens and Abdullah Barhoum and Nguyen Minh Duc and Oliver Stanley and Richárd Nagyfi and Shahul ES and Sameer Suri and David Glushkov and Arnav Dantuluri and Andrew Maguire and Christoph Schuhmann and Huu Nguyen and Alexander Mattick},
      year={2023},
      eprint={2304.07327},
      archivePrefix={arXiv},
      primaryClass={cs.CL},
      url={https://arxiv.org/abs/2304.07327}, 
}

@inproceedings{agerri-etal-2018-developing,
    title = "Developing New Linguistic Resources and Tools for the {G}alician Language",
    author = "Agerri, Rodrigo  and
      G{\'o}mez Guinovart, Xavier  and
      Rigau, German  and
      Solla Portela, Miguel Anxo",
    editor = "Calzolari, Nicoletta  and
      Choukri, Khalid  and
      Cieri, Christopher  and
      Declerck, Thierry  and
      Goggi, Sara  and
      Hasida, Koiti  and
      Isahara, Hitoshi  and
      Maegaard, Bente  and
      Mariani, Joseph  and
      Mazo, H{\'e}l{\`e}ne  and
      Moreno, Asuncion  and
      Odijk, Jan  and
      Piperidis, Stelios  and
      Tokunaga, Takenobu",
    booktitle = "Proceedings of the Eleventh International Conference on Language Resources and Evaluation ({LREC} 2018)",
    month = may,
    year = "2018",
    address = "Miyazaki, Japan",
    publisher = "European Language Resources Association (ELRA)",
    url = "https://aclanthology.org/L18-1367/"
}

@inproceedings{ferres-saggion@LREC2022,
    title = "ALEXSIS: A Dataset for Lexical Simplification in Spanish.",
    author = "Ferrés, Daniel  and Saggion, Horacio",
    booktitle      = {Proceedings of the Language Resources and Evaluation Conference},
    month          = {June},
    year           = {2022},
    address        = {Marseille, France},
    publisher      = {European Language Resources Association},
    pages     = {3582--3594},
    url       = {https://aclanthology.org/2022.lrec-1.383}
}

@misc{gervasio,
      title={Advancing Generative AI for Portuguese with
             Open Decoder Gervásio PT-*}, 
      author={Rodrigo Santos, João Silva, Luís Gomes,
              João Rodrigues, António Branco},
      year={2024},
      eprint={2402.18766},
      archivePrefix={arXiv},
      primaryClass={cs.CL}
}

@misc{singh2024aya,
      title={Aya Dataset: An Open-Access Collection for Multilingual Instruction Tuning}, 
      author={Shivalika Singh and Freddie Vargus and Daniel Dsouza and Börje F. Karlsson and Abinaya Mahendiran and Wei-Yin Ko and Herumb Shandilya and Jay Patel and Deividas Mataciunas and Laura OMahony and Mike Zhang and Ramith Hettiarachchi and Joseph Wilson and Marina Machado and Luisa Souza Moura and Dominik Krzemiński and Hakimeh Fadaei and Irem Ergün and Ifeoma Okoh and Aisha Alaagib and Oshan Mudannayake and Zaid Alyafeai and Vu Minh Chien and Sebastian Ruder and Surya Guthikonda and Emad A. Alghamdi and Sebastian Gehrmann and Niklas Muennighoff and Max Bartolo and Julia Kreutzer and Ahmet Üstün and Marzieh Fadaee and Sara Hooker},
      year={2024},
      eprint={2402.06619},
      archivePrefix={arXiv},
      primaryClass={cs.CL}
}

@dataset{gamallo_pablo_2023_7671278,
  author       = {Gamallo  Pablo and
                  Garcia Marcos and
                  de-Dios-Flores Iria and
                  Ramom Pichel Campos  José and
                  Sandra Rodríguez Rey and
                  Bardanca Daniel},
  title        = {Nos\_ES-GL\_aut},
  month        = mar,
  year         = 2023,
  publisher    = {Zenodo},
  version      = {1.0.0},
  doi          = {10.5281/zenodo.7671278},
  url          = {https://doi.org/10.5281/zenodo.7671278},
}
