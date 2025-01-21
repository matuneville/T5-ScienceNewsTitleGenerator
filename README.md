# T5 Title Generator for Science Articles

This repository contains a fine-tuned T5 model designed to generate concise and relevant titles for scientific articles.

---

## Model Description

The model is built on **Google's T5 (Text-to-Text Transfer Transformer)** architecture. T5 is a powerful sequence-to-sequence model capable of performing various NLP tasks, including summarization, translation, and text classification.

### Objective
This fine-tuned model focuses on generating accurate and concise titles for scientific articles based on their abstracts or main content. By leveraging the T5 architecture, the model transforms longer scientific content into short, descriptive titles.

- **Fine-tuned on a scientific dataset**: Optimized specifically for the task of title generation.
- **Evaluation against base T5**: Results were compared with the standard T5 summarization capability, showcasing the improvements achieved through fine-tuning.

### Status

The model has been fine-tuned for **500 steps**. While the current checkpoint demonstrates significant improvements in title generation, further training may enhance the performance. This checkpoint serves as an intermediate result showcasing the potential of fine-tuning the T5 architecture for this task.

### Evaluation Metrics

- **ROUGE** scores were used to evaluate the model's performance on the validation dataset, which indicate if the model generates titles with higher or lower relevance and linguistic quality.

---

#### Example:
```plaintext

Article:

    Researchers from the University of Toronto and LG AI Research have developed an "explainable" artificial
    intelligence (XAI) algorithm that can help identify and eliminate defects in display screens. The new algorithm,
    which outperformed comparable approaches on industry benchmarks, was developed through an ongoing AI research
    collaboration between LG and U of T that was expanded in 2019 with a focus on AI applications for businesses .
    Researchers say the XAI algorithm could potentially be applied in other fields that require a window into how
    machine learning makes its decisions, including the interpretation of data from medical scans. "Explainability and
    interpretability are about meeting the quality standards we set for ourselves as engineers and are demanded by the
    end user," says Kostas Plataniotis , a professor in the Edward S. Rogers Sr. department of electrical and computer
    engineering in the Faculty of Applied Science & Engineering. "With XAI, there's no 'one size fits all.' You have to
    ask whom you're developing it for. Is it for another machine learning developer? Or is it for a doctor or lawyer?"
    ...

Original Title:

    Researchers Develop 'Explainable' Algorithm

Title by My Finetuned Model:

    Researchers Develop "Explainable" Artificial Intelligence (XAI) Algorithm

Title by Pretrained Model:

    researchers from the university of Toronto and LG AI Research have developed an "explainable" artificial
    intelligence algorithm.

```

---

## Usage

### Installation
1. Install the Hugging Face Transformers library:
   ```bash
   pip install transformers
   ```

### Loading the Model

TODO: upload model to hugging face


