# Sarcasm-Aware Depression Detection from Reddit using NLP

This project explores automated depression detection from Reddit posts using NLP, with a focus on improving reliability by accounting for sarcastic language.

## Motivation
Transformer-based models achieve high accuracy in depression detection but often fail on sarcastic or ironic text. This project introduces a sarcasm-aware pipeline to flag potentially unreliable predictions.

## Approach
- Fine-tuned **DistilBERT** for depression detection
- Fine-tuned **DistilBERT** for sarcasm detection
- Error analysis to identify sarcasm-related failures
- Interpretation layer combining both model outputs
- Interactive **Gradio demo**

## Models
| Task | Model | Macro F1 |
|----|----|----|
| Depression Detection | DistilBERT | ~0.98 |
| Sarcasm Detection | DistilBERT | ~0.78 |

## Demo
An interactive Gradio-based demo allows users to input Reddit-style text and receive:
- Depression prediction + confidence
- Sarcasm prediction + confidence
- Combined interpretation

## Datasets
Due to size constraints, datasets are not hosted in this repository.

- Reddit Depression Dataset  
- Reddit Sarcasm Dataset  

## Disclaimer
This project is for research and educational purposes only and is **not a clinical diagnostic tool**.

## Author
Anuj Prakash  
Indiana University Bloomington
