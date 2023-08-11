# Promptimizer
Using Meta's Llama 2 LLM, we fine tune the model to be optimized for turning "bad" prompts that yield an inefficient responses into "good" ones which are optimal prompts specifically for AI that generate fruitful responses.

## Authors and Credits
- Julian Sanchez
- Emily Zou
- Nathan Benitez
- Nati Seifu

Additional credits:
- Abraham Bautista (Mentor)
- [PromptEnginerring](https://youtu.be/LslC2nKEEGU)
- [1littlecoder](https://youtu.be/eeM6V5aPjhk)
## Vision for the Model
- 
## Dataset
- Dataset was constructed according to [OpenAI's Best Practices for Prompt Engineering](https://help.openai.com/en/articles/6654000-best-practices-for-prompt-engineering-with-openai-api)
## Packages and Libraries
### Hugging Face
We used a very strong package in, AutoTrain, to fine-tune the open-source Llama V2 assistant for our purpose.
 - The one-liner code included in the training section is achieved through this package.
 - Usually, a large-scale fine-tuning processes would require a strong GPU, but the small dataset we have allows the fine-tuning at a smaller scale.

#### AutoTrain Documentation -- from HuggingFace
🤗 AutoTrain is a no-code tool for training state-of-the-art models for Natural Language Processing (NLP) tasks, for Computer Vision (CV) tasks, and for Speech tasks and even for Tabular tasks. It is built on top of the awesome tools developed by the Hugging Face team, and it is designed to be easy to use.

Who should use AutoTrain?
AutoTrain is for anyone who wants to train a state-of-the-art model for a NLP, CV, Speech or Tabular task, but doesn’t want to spend time on the technical details of training a model. AutoTrain is also for anyone who wants to train a model for a custom dataset, but doesn’t want to spend time on the technical details of training a model. Our goal is to make it easy for anyone to train a state-of-the-art model for any task and our focus is not just data scientists or machine learning engineers, but also non-technical users.

How to use AutoTrain?
We offer several ways to use AutoTrain:

No code users with large number of data samples can use AutoTrain Advanced by creating a new space with AutoTrain Docker image: https://huggingface.co/new-space?template=autotrain-projects/autotrain-advanced. Please make sure you keep the space private.

No code users with small number of data samples can use AutoTrain using the UI located at: https://ui.autotrain.huggingface.co/projects. Please note that this UI won’t be updated with new tasks and features as frequently as AutoTrain Advanced.

Developers can access and build on top of AutoTrain using python api or run AutoTrain Advanced UI locally. The python api is available in the autotrain-advanced package. You can install it using pip:

Copied
pip install autotrain-advanced
What is AutoTrain Advanced?
AutoTrain Advanced processes your data either in a Hugging Face Space or locally (if installed locally using pip). This saves one time since the data processing is not done by the AutoTrain backend, resulting in your job not being queued. AutoTrain Advanced also allows you to use your own hardware (better CPU and RAM) to process the data, thus, making the data processing faster.

Using AutoTrain Advanced, advanced users can also control the hyperparameters used for training per job. This allows you to train multiple models with different hyperparameters and compare the results.

Everything else is the same as AutoTrain. You can use AutoTrain Advanced to train models for NLP, CV, Speech and Tabular tasks.

We recommend using AutoTrain Advanced since it is faster, more flexible and will have more supported tasks and features in the future.

## Possible Future Capabilities
<to be filled>

## Resources Used
