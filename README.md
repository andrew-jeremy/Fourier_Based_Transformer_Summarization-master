
## Project Abstract

In this work, we employ the newly developed token mixing approach using Fourier Transforms (FNET) to replace computationally expensive self-attention mechanism in the transformer  model on a  summarization task for  long documents (i.e., documents with more than 512 tokens).  As a baseline, we also carry out long document summarization using established methods such as Longformer and Big Bird transformer models that are capable of processing over 8000 tokens and are currently the state of the art methods for these type of problems.  The original FNET paper implemented this in an encoder only architecture while abstractive summarization requires both an encoder and a decoder. Since such a pretrained transformer model does not currently exist in the public domain, we decided to implement a toy transformer based on this Fourier token mixing approach in an encoder/decoder architecture which we trained starting with Glove embeddings for the individual words in the corpus. We investigated a number of different extensions to the original FNET architecture and evaluated them on their Rouge F1-score performance on a summarization task. All attempted modifications showed better performance on the summarization task than when using the original FNET encoder in a transformer architecture. The baseline results using either reduction steps before using PEGASUS or the longformer model have higher scores since there are no pretrained weights for the new FNET transformer model we are proposing. We thus demonstrated the computational gain of the architecture using a toy model. The extractive reduction techniques used as a baseline showed promise by improving on Rouge f1 scores using a small number of examples for tuning. The prepossessing extractive summarization techniques implement different strategies of for retaining the salient information of the document which can be used to fine tune PEGASUS<sub>LARGE</sub>.

## Important Project Links
- [Project Proposal](Project_Proposal.pdf)
- [Project Milestone](Project_Milestone.pdf)
- [Project Final Paper](Project_Final.pdf)
- [Project Final Presentation](https://docs.google.com/presentation/d/1PzWlqzRHvfJVOe4TiAKUiigcVzSEmAgTMLIOYDUu7NM/edit?usp=sharing)

## Jupyter Notebook Links
- [PEGASUS Baseline](Long_Document_Summarization_with_PEGASUS.ipynb)
- [Longformer Baseline](Longformer_PubMed_Base_v2.ipynb)
- [FNET Approach Notebook](abstractive_transformer_summarizer_with_FNET_transformer_ver2.ipynb)
- [FNET Approach Python Script](abstractive_transformer_summarizer_with_fnet_transformer.py)

# Fourier_Based_Transformer_Summarization-master
