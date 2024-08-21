# LoRA_tutorial

We create a simple tutorial to finetune pre-trained BLOOM (1b7) from hugging face, using LoRA, on the squad dataset.

The code has been adapted from https://www.youtube.com/watch?v=iYr1xZn26R8

Hugging Face implementations are constantly updated, this runs without bugs on 21/08/2024.

More specifically the notebook above
* loads pretrained BLOOM from hugging face
* loads squad_v2 dataset, which is a Q&A type dataset that BLOOM is not traditionally good at
* uses LoRA to finetune its query_key_value parameters
* pushes the LoRA weights on my hugging face account, stathismegas/squad-bloom-1b7
* loads this fine tuned model from hugging face
* tries on some real Q&A

