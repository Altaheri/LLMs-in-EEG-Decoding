# Review on Large Language Models in EEG Signal Decoding

Recommended review papers cover key components of modern artificial intelligence:

- Self-supervised learning (SSL)  
[A Cookbook of Self-Supervised Learning](https://ai.meta.com/blog/self-supervised-learning-practical-guide/)

- Multimodal learning  
[Self-Supervised Multimodal Learning: A Survey](https://ieeexplore.ieee.org/abstract/document/10630605/?casa_token=6SoLtSVwWVQAAAAA:0fVfKHrEFcpn9e8v5QxZbgmnfciBtZGwYo7HrByIvR0_1wZVWe32xL2Cor_w69N-X3qyX_Pn8w)

- Foundation models  
[On the Opportunities and Risks of Foundation Models](https://arxiv.org/abs/2108.07258)
[Foundation Models Defining a New Era in Vision: A Survey and Outlook](https://ieeexplore.ieee.org/abstract/document/10834497/?casa_token=UsePsFo52zcAAAAA:Zyequ-7KhPJ656tORInzu5uIjxsofM3nmKL2PdWzMaQupzGbJstaQlWXPQXbk2WpgLFDLWhmFQ)  
[A Survey of Large Language Models](https://paper-notes.zhjwpku.com/assets/pdfs/llm_survey_2303.18223.pdf)  

- Learning from models  
[Learning from models beyond fine-tuning](https://www.nature.com/articles/s42256-024-00961-0)

---

This table briefly overviews research papers, highlighting the title, year, publication venue, performance, and code availability.

| Paper Title | Year | Publication Venue | Foundation Model | Performance | Code Availability |
|-------------|------|-------------------|------------------|-------------|--------------------|
| [BELT: Bootstrapped EEG-to-Language Training by Natural Language Supervision](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10649644) | 2023 | *IEEE TRANSACTIONS ON NEURAL SYSTEMS AND REHABILITATION ENGINEERING* | BERT, GPT-3 | Achieved 42.31% BLEU-1 score and 67.32% precision in sentiment classification | Not available |
| [Neuro-GPT: Towards A Foundation Model for EEG](https://ieeexplore.ieee.org/document/10635453) | 2023 | *IEEE International Symposium on Biomedical Imaging (ISBI)* | GPT | Significantly improved classification performance compared to models trained from scratch | [Available](https://github.com/wenhui0206/NeuroGPT) |
| [Open Vocabulary Electroencephalography-to-Text Decoding and Zero-Shot Sentiment Classification](https://ojs.aaai.org/index.php/AAAI/article/view/20472)             | 2022 | *AAAI Conference on Artificial Intelligence (AAAI-22)*      | GPT-3.5          | BLEU ~22.0, Accuracy ~85%, F1 ~0.84                                                 | [Available](https://github.com/MikeWangWZHL/EEG-To-Text)     |
| [Large Brain Model for Learning Generic Representations with Tremendous EEG Data in BCI](https://openreview.net/pdf?id=QzTpTRVtrP) | 2024 | *ICLR 2024* | Unified Foundation Model | Outperformed state-of-the-art methods in respective fields | [Available](https://github.com/935963004/LaBraM) |
| [EEG-GPT: Exploring Capabilities of Large Language Models for EEG Classification and Interpretation](https://arxiv.org/abs/2401.18006) | 2023 | *arXiv Preprint* | GPT-3 | Achieved excellent performance in classifying normal vs. abnormal EEG | Not available |
| [Are EEG-to-Text Models Working?](https://arxiv.org/pdf/2405.06459)                                                 | 2024 | *IJCAI 2024*         | N/A                                   | Details not provided                                                        | [Available](https://github.com/NeuSpeech/EEG-To-Text)|
|  |  |  |  |  |  |
| [BENDR: Using Transformers and a Contrastive Self-Supervised Learning Task to Learn from Massive Amounts of EEG Data](https://www.frontiersin.org/journals/human-neuroscience/articles/10.3389/fnhum.2021.653659/full) | 2021 | Frontiers in Human Neuroscience         | BENDR (Transformer-based)             | State-of-the-art results on multiple EEG classification tasks               | [Available](https://github.com/SPOClab-ca/BENDR) |
| [Decoding EEG Brain Activity for Multi-Modal Natural Language Processing](https://www.frontiersin.org/articles/10.3389/fnhum.2021.659410/full) | 2021 | *Frontiers in Human Neuroscience* | N/A | Improved accuracy over baselines; specific metrics not provided | Not available |
| [Thought2Text: Text Generation from EEG Signal using Large Language Models (LLMs)](https://arxiv.org/abs/2410.07507) | 2024 | *arXiv Preprint* | LLaMa, Mistral | Demonstrated efficacy in generating coherent text from EEG signals | [Available](https://github.com/abhijitmishra/Thought2Text) |
| [BrainECHO: Semantic Brain Signal Decoding through Vector-Quantized Spectrogram Reconstruction](https://arxiv.org/abs/2410.14971) | 2024 | *arXiv Preprint* | Whisper | Outperformed state-of-the-art methods on EEG and MEG datasets | Not available |
| [Enhancing EEG-to-Text Decoding through Transferable Representations from Pre-trained Contrastive EEG-Text Masked Autoencoder](https://arxiv.org/abs/2402.17433) | 2024 | *arXiv Preprint* | BART | Outperformed baseline framework by 8.34% in ROUGE-1 F1 and 32.21% in BLEU-4 | Not available |
| [Deep Representation Learning for Open Vocabulary Electroencephalography-to-Text Decoding](https://arxiv.org/abs/2312.09430) | 2023 | *arXiv Preprint* | BART | Achieved 42.75% BLEU-1, 33.28% ROUGE-1-F, and 53.86% BERTScore-F | Not available |
| [Sleep CLIP: A Multimodal Sleep Staging Model Based on Sleep Signals and Sleep Staging Labels](https://www.mdpi.com/1424-8220/23/17/7341)                  | 2023 | MDPI Sensors   | CLIP-based Architecture               | Reported state-of-the-art performance in sleep staging                      | Not available                                       |


---


This table summarizes more information including the contributions, datasets, applications, performance, publication venues, and code availability.

| Paper Title | Year | Main Contribution | Dataset | Task/Application | Metrics Used | Performance | GPU Used | Journal/Publication Venue | Code Availability |
|-------------|------|--------------------|---------|------------------|--------------|-------------|----------|---------------------------|--------------------|
| [BELT: Bootstrapped EEG-to-Language Training by Natural Language Supervision](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10649644) | 2023 | Introduced BELT, a model that bootstraps EEG representation learning using large LMs, improving brain-to-language translation and zero-shot sentiment classification. | EEG datasets with natural reading tasks | Brain-to-language translation, sentiment classification | BLEU-1, precision | Achieved 42.31% BLEU-1 score and 67.32% precision in sentiment classification | Not specified | *arXiv Preprint* | Not available |
| [Neuro-GPT: Towards A Foundation Model for EEG](https://arxiv.org/abs/2311.03764) | 2023 | Introduced Neuro-GPT, a foundation model consisting of an EEG encoder and a GPT model, pre-trained on large-scale data to improve performance in low-data regimes for EEG tasks. | Large-scale EEG dataset | Motor imagery classification | Classification accuracy | Significantly improved classification performance compared to models trained from scratch | Not specified | *arXiv Preprint* | [Available](https://github.com/wenhui0206/NeuroGPT) |
| [Open Vocabulary Electroencephalography-to-Text Decoding and Zero-Shot Sentiment Classification](https://arxiv.org/abs/2112.02690) | 2021 | Proposes an open-vocabulary EEG-to-text decoding pipeline that also performs zero-shot sentiment classification via an integrated LLM. | Private EEG corpus + sentiment labels         | EEG-to-text generation, zero-shot sentiment classification | BLEU, Accuracy, F1             | BLEU ~22.0, Accuracy ~85%, F1 ~0.84                                                         | Not specified | *arXiv Preprint*                   | Not available    |
| [Large Brain Model for Learning Generic Representations with Tremendous EEG Data in BCI](https://arxiv.org/abs/2405.18765) | 2024 | Proposed LaBraM, a unified foundation model for EEG that enables cross-dataset learning through unsupervised pre-training, improving performance across multiple EEG tasks. | Approximately 2,500 hours of various EEG signals from around 20 datasets | Abnormal detection, event type classification, emotion recognition, gait prediction | Various task-specific metrics | Outperformed state-of-the-art methods in respective fields | Not specified | *arXiv Preprint* | [Available](https://github.com/935963004/LaBraM) |
| [EEG-GPT: Exploring Capabilities of Large Language Models for EEG Classification and Interpretation](https://arxiv.org/abs/2401.18006) | 2024 | Proposed EEG-GPT, leveraging LLMs for EEG classification, achieving performance comparable to state-of-the-art methods with enhanced interpretability. | EEG datasets with normal and abnormal recordings | EEG classification | Accuracy | Achieved excellent performance in classifying normal vs. abnormal EEG with limited training data | Not specified | *arXiv Preprint* | Not available |
| [Are EEG-to-Text Models Working?](https://arxiv.org/pdf/2405.06459)                                                                                   | 2023 | Systematically evaluated existing EEG-to-text decoding approaches, highlighting performance gaps and challenges for robust generalization.                                                                          | Various EEG datasets (comparative analysis)                                    | EEG-to-text decoding                                  | BLEU, WER, etc. (varies)        | Demonstrated limitations and raised questions on current EEG-to-text performance benchmarks             | Not specified | *arXiv Preprint*                       | [Available](https://github.com/NeuSpeech/EEG-To-Text)          |
| [BENDR: Using Transformers and a Contrastive Self-Supervised Learning Task to Learn from Massive Amounts of EEG Data](https://www.frontiersin.org/journals/human-neuroscience/articles/10.3389/fnhum.2021.653659/full) | 2021 | Proposed a self-supervised Transformer-based approach (BENDR) for EEG representation learning using contrastive objectives, achieving robust performance on multiple EEG classification tasks.                         | TUH EEG and other large EEG corpora                                            | EEG classification                                    | Accuracy, F1                   | Achieved near state-of-the-art results on several EEG classification benchmarks                          | Not specified | *arXiv Preprint*                       | [Available](https://github.com/SPOClab-ca/BENDR)      |
| [Decoding EEG Brain Activity for Multi-Modal Natural Language Processing](https://www.frontiersin.org/articles/10.3389/fnhum.2021.659410/full) | 2021 | Investigated the integration of EEG signals with textual data to enhance NLP tasks, demonstrating that EEG features can improve sentiment classification. | Custom dataset with EEG recordings during reading tasks | Sentiment classification | Accuracy | Improved accuracy over baselines; specific metrics not provided | Not specified | *Frontiers in Human Neuroscience* | Not available |
| [Thought2Text: Text Generation from EEG Signal using Large Language Models (LLMs)](https://arxiv.org/abs/2410.07507) | 2024 | Proposed a three-stage approach to generate text from EEG signals by fine-tuning LLMs with EEG data, enabling direct text generation from brain activity. | Public EEG dataset with image stimuli | Text generation | BLEU, ROUGE, human evaluation | Demonstrated efficacy in generating coherent text from EEG signals | Not specified | *arXiv Preprint* | [Available](https://github.com/abhijitmishra/Thought2Text) |
| [BrainECHO: Semantic Brain Signal Decoding through Vector-Quantized Spectrogram Reconstruction](https://arxiv.org/abs/2410.14971) | 2024 | Introduced a multi-stage strategy for semantic brain signal decoding via vector-quantized spectrogram reconstruction, enhancing text generation from EEG. | EEG dataset (Brennan) and MEG dataset (GWilliams) | Semantic decoding, text generation | Accuracy, BLEU, ROUGE | Outperformed state-of-the-art methods on both EEG and MEG datasets | Not specified | *arXiv Preprint* | Not available |
| [Enhancing EEG-to-Text Decoding through Transferable Representations from Pre-trained Contrastive EEG-Text Masked Autoencoder](https://arxiv.org/abs/2402.17433) | 2024 | Developed a Contrastive EEG-Text Masked Autoencoder (CET-MAE) to enhance EEG-to-text decoding by leveraging pre-trained LLMs for improved language reconstruction. | ZuCo dataset with text-evoked EEG recordings | EEG-to-text decoding | ROUGE-1 F1, BLEU-4 | Outperformed baseline framework by 8.34% in ROUGE-1 F1 and 32.21% in BLEU-4 | Not specified | *arXiv Preprint* | Not available |
| [Deep Representation Learning for Open Vocabulary Electroencephalography-to-Text Decoding](https://arxiv.org/abs/2312.09430) | 2023 | Presented an end-to-end deep learning framework for open vocabulary EEG-to-text decoding, incorporating subject-dependent representation learning and a BART language model. | ZuCo v1.0 and v2.0 datasets with EEG recordings during natural reading tasks | EEG-to-text decoding | BLEU-1, ROUGE-1-F, BERTScore-F | Achieved 42.75% BLEU-1, 33.28% ROUGE-1-F, and 53.86% BERTScore-F, outperforming previous state-of-the-art methods | Not specified | *arXiv Preprint* | Not available |
| [Sleep CLIP: A Multimodal Sleep Staging Model Based on Sleep Signals and Sleep Staging Labels](https://www.mdpi.com/1424-8220/23/17/7341)                                                          | 2023 | Proposed a multimodal sleep staging approach leveraging a CLIP-based architecture, integrating EEG and textual labels for improved staging performance.                                                               | Not specified                                                                | Sleep staging                                        | Accuracy, F1, Cohen’s Kappa     | Reported state-of-the-art performance in sleep staging                                                | Not specified | MDPI Sensors                 | Not available                                             |


## Notes:
- The GPU models used for training are not specified in most papers.
- For more details, visit the provided links to the respective papers and repositories.
