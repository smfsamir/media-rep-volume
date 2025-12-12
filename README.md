# media-rep-volume

These are the artifacts for the project **Quantifying Media Representation Dynamics Across 25 Years of
News Reporting on Policing-related Deaths**

# Closed-source LLM prompts
Prompts for a closed-source LLM (we applied GPT-4o) are in the `llm_prompts` directory. We used two conversational turns to complete the parse. The first turn is in `task_1_prompt.txt`, the second in `task_2_prompt.txt`. 

# Training dataset
The training data annotations (described in Section 4.1) are available in `data/training_data.json`. The corresponding articles are in `data/articles`. 

# Analysis dataset and predictions
The articles for the analysis in Section 5 as well as the predictions from the PerspectiveGap for these articles are in `unsupervised_inference_predictions.tsv`. 

# Model
The PerspectiveGap model (based on Flan-T5) will be released upon publication. The training and evaluation recipe are available in `main_distillation.py`. In order to apply it, the coreference resolution model must be applied (`main_coref.py`). 
