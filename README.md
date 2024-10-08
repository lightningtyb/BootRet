# Bootstrapped Pre-training with Dynamic Identifier Prediction for Generative Retrieval (ACL 2024)

## Abstract
Generative retrieval uses differentiable search indexes to directly generate relevant document identifiers in response to a query. Recent studies have highlighted the potential of a strong generative retrieval model, trained with carefully crafted pre-training tasks, to enhance downstream retrieval tasks via fine-tuning. However, the full power of pre-training for generative retrieval remains underexploited due to its reliance on pre-defined static document identifiers, which may not align with evolving model parameters. In this work, we introduce BootRet, a bootstrapped pre-training method for generative retrieval that dynamically adjusts document identifiers during pre-training to accommodate the continuing  memorization of the corpus. BootRet involves three key training phases: (i) initial identifier generation, (ii) pre-training via corpus indexing and relevance prediction tasks, and (iii) bootstrapping for identifier updates. To facilitate the pre-training phase, we further introduce noisy documents and pseudo-queries, generated by large language models, to resemble semantic connections in both indexing and retrieval tasks. Experimental results demonstrate that BootRet significantly outperforms existing pre-training generative retrieval baselines and performs well even in zero-shot settings.

## Method overview

![The bootstrapped pre-training pipeline of BootRet. (1) The initial docids $𝐼_𝐷^0$ are obtained with the initial model parameters $𝜃^0$. (2) To perform the 𝑡-th iteration, we design the corpus indexing task and relevance prediction task for pre-training. We construct noisy documents and pseudo-queries with a LLM, and design contrastive losses (the yellow and the orange rectangles) and a semantic consistency loss (the green rectangle) to learn the corpus and relevance information discriminatively. After pre-training, the model updates from $𝜃^(𝑡−1)$  to $𝜃^𝑡$. (3) The bootstrapped $𝜃^𝑡$  is used to dynamically update the docids $𝐼_𝐷^(𝑡−1)$  to $𝐼_𝐷^𝑡$, i.e., bootstrapped docids, which are further used in the next iteration. (Figure should be viewed in color).](resources/overview.png)


## Resources

[Paper](resources/ACL24-Bootstrapped_Pre-training_with_Dynamic_Identifier_Prediction_for_Generative_Retrieval.pdf)

[Poster](resources/poster-BootRet-ACL_Findings_1874.pdf)

[Slides](resources/slides-BootRet-ACL_Findings_1874.pptx)

[Video](https://www.dropbox.com/scl/fi/fa69j96u98m6pdyg1lacb/video-BootRet-ACL-Findings-1874.mp4?rlkey=ao3fj7v01rn6mszr88q3gu0th&st=g3hzhsjb&dl=0)




