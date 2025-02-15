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
