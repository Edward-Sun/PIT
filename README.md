# Pre-instruction-tuning

This repository contains the reproduced data for the paper [Instruction-tuned Language Models are Better Knowledge Learners](https://arxiv.org/abs/2402.12847).

## Wiki2023 Dataset
The data included in this repository is *not* the original data used in the paper.
I regenerated the data following the recipe proposed by the paper using the ChatGPT model (`gpt-3.5-turbo-1106`).
It should lead to a similar performance.

```shell
|-- wiki2023_film_test  # the test split of the film domain
    |-- doc.jsonl
    |-- qa.jsonl
|-- wiki2023_film_train  # the training split of the film domain
    |-- doc.jsonl
    |-- qa.jsonl
|-- wiki2023_other_train  # the training split of other domains
    |-- doc.jsonl
    |-- qa.jsonl
```

Each line of document jsonl files includes the Wikipedia ID, the title, and the body text of an article.
Each line of QA jsonl files includes the Wikipedia ID and a generated question-answer pair.
