# Finance-Domain-Specific-Fine-Tuning-Of-VQA-Models-for-Document-Visual-Question-Answering
Document Visual Question Answering (DocVQA) is a multimodal task that requires reasoning from both textual content and spatial layout to infer semantic  relationships between them.
Document Visual Question Answering (DocVQA) is a multimodal task that requires reasoning from both textual content and spatial layout to infer semantic relationships between them. Recent Vision Language Models(VLMs), such as Donut, LayoutLMv3 and BLIP-2 multimodels have shown strong performance on image understanding tasks. However, these state-of-the-art models underperformed when applied to domain specific documents such as educational reports, healthcare forms, editorial articles, legal contracts due to variation in vocabulary usage, visual patterns and layout structure.
This project proposes a domain specific fine tuning architecture for vision language models excelled to document visual question answering. The main goal is to enhance accuracy, reasoning capability and robustness by reconciling pre-trained VLMs to tailored domain specific documents using open source datasets and targeted training strategies. The projects will explore all different kinds of fine-tuning methods including parameter-efficient-fine-tuning (adapters, QLoRA, LoRA), and instruction based fine tuning. The experiment and evaluation will be conducted across different domains (computer vision, NLP) to evaluate the performance metrics.


This repo contains Files for fine tuning qwen model with QLoRa and its performance evaluation.
The model has been fine tuned with 6000 QnA images pairs.
We saw significant performance improvement by just training on 6000 dataset , due to hardware constraint , which means if fine tuned on large dataset , performance can improve significantly.

We used kaggle to train and evaluate the performance of model.
Hyperparmeter settings can be found in expermients_config.yaml file.
Performance evaluation has been done on base model and fine tuned model with highest dataset and epochs(6000,7).