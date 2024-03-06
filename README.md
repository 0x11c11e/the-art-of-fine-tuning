# The Art of Fine Tuning
Fine-tuning is a process where a pre-trained model is further trained on a new dataset to supplement its existing knowledge. This approach enables the model to become adept at performing specific tasks beyond its initial training, such as classification, summarization, or conversational interactions. Originally, large language models are typically designed as autoregressive models, primarily focusing on predicting the next token in a sequence based on the preceding context. This design inherently limits their direct applicability to specialized tasks without additional training.

To adapt these models for various downstream tasks, they are fine-tuned using datasets tailored to these specific applications. This process allows the models to apply their broad foundational knowledge effectively to the new tasks. It's important to note that during the initial training phase of a large language model, the parameters start from arbitrary values. Optimizing these parameters to a state where the model is both effective and efficient involves considerable computational resources and expense. Hence, the cost of training a large language model from scratch is significantly higher than fine-tuning an existing model. The latter leverages the extensive learning already encapsulated in the pre-trained model, reducing the need for extensive computational resources and thus lowering costs. This approach not only economizes on training expenses but also expedites the model's readiness for specific applications.

---
## Fine tune in Colab

| Fine-tune Llama 2 in Google Colab | [Link](https://colab.research.google.com/drive/1FSMdcdX7Lwr-yQRhosDPRAZ6Mm0wpSRu#scrollTo=VspxyjL54uPz) |

---

## Fine-tuning ChatGPT for automatic scoring

This study explores the enhancement of automatic scoring systems through the fine-tuning of ChatGPT (GPT-3.5), with a focus on student-written responses in the educational sector. By leveraging a dataset comprising middle-school and high-school student responses across various science assessments, we fine-tuned GPT-3.5 to improve its scoring accuracy significantly. The process involved domain-specific adjustments to the model, demonstrating the potential of large language models in educational applications. Our findings highlight GPT-3.5's superior performance in automatic scoring tasks compared to traditional models, marking a step forward in the integration of AI in educational assessment.

## Relevant Papers

| Topic                                       | Paper            |
|---------------------------------------------|------------------|
| Fine-tuning ChatGPT for automatic scoring   | [Link](https://www.sciencedirect.com/science/article/pii/S2666920X24000110) |

---

## Fine-Tuning Language Models with Just Forward Passes

The paper "Fine-Tuning Language Models with Just Forward Passes" introduces a memory-efficient zeroth-order optimizer (MeZO) designed to fine-tune large language models (LMs) with the same memory footprint as inference, circumventing the prohibitive memory requirements of backpropagation for large models. Through adapting the classical Zeroth-Order Stochastic Gradient Descent (ZO-SGD) method for in-place operation, MeZO enables training on models up to 30 billion parameters on a single A100 80GB GPU—a task only feasible for a 2.7B parameter model using traditional backpropagation. Comprehensive experiments demonstrate MeZO's efficacy across various model scales (up to 66B), types (masked and autoregressive LMs), and tasks (classification, multiple-choice, and generation), achieving comparable or superior performance to backpropagation and other parameter-efficient tuning techniques, with significantly reduced memory and computational resources. The paper also provides theoretical insights supporting MeZO's capability to fine-tune large models effectively, despite traditional analyses suggesting otherwise.

## Relevant Papers

| Topic                                                             | Code | Paper |
|-------------------------------------------------------------------|------|-------|
| Fine-Tuning Language Models with Just Forward Passes              | [Github](https://github.com/princeton-nlp/MeZO) | [Link](https://proceedings.neurips.cc/paper_files/paper/2023/file/a627810151be4d13f907ac898ff7e948-Paper-Conference.pdf) |

---
