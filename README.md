# Bootstrapped Pre-training with Dynamic Identifier Prediction for Generative Retrieval (ACL 2024)

Generative retrieval uses differentiable search indexes to directly generate relevant document identifiers in response to a query. Recent studies have highlighted the potential of a strong generative retrieval model, trained with carefully crafted pre-training tasks, to enhance downstream retrieval tasks via fine-tuning. However, the full power of pre-training for generative retrieval remains underexploited due to its reliance on pre-defined static document identifiers, which may not align with evolving model parameters. In this work, we introduce BootRet, a bootstrapped pre-training method for generative retrieval that dynamically adjusts document identifiers during pre-training to accommodate the continuing  memorization of the corpus. BootRet involves three key training phases: (i) initial identifier generation, (ii) pre-training via corpus indexing and relevance prediction tasks, and (iii) bootstrapping for identifier updates. To facilitate the pre-training phase, we further introduce noisy documents and pseudo-queries, generated by large language models, to resemble semantic connections in both indexing and retrieval tasks. Experimental results demonstrate that BootRet significantly outperforms existing pre-training generative retrieval baselines and performs well even in zero-shot settings.

[PDF](paper/ACL24-Bootstrapped Pre-training with Dynamic Identifier Prediction for Generative  Retrieval.pdf)
[Poster](paper/ACL24-Bootstrapped Pre-training with Dynamic Identifier Prediction for Generative  Retrieval.pdf)
[Video](paper/ACL24-Bootstrapped Pre-training with Dynamic Identifier Prediction for Generative  Retrieval.pdf)




