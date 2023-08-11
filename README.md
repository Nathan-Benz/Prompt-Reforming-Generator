# Promptimizer
Promptimizer is a Large Language Model (LLM) designed for users who want to generate better prompts in order to use fewer prompt iterations when using other LLMs to get more efficient/accurate prompts.

Using Meta's Llama 2 LLM as the base model, we perform fine-tuning for its optimization in order to convert "bad" prompts that usually produce inefficient/inaccurate responses into "good" ones, which can be interpreted as optimal indications given the specifications of the Generative AI in question.

## Authors and Credits
(Team JENNA)
- Julian Sanchez
- Emily Zou
- Nathan Benitez
- Nati Seifu

Additional credits:
- Abraham Bautista (Mentor)
- [PromptEnginerring](https://youtu.be/LslC2nKEEGU)
- [1littlecoder](https://youtu.be/eeM6V5aPjhk)
## Vision for the Model
We decided to tackle the issue of prompt engineering, specifically in the public domain. We recognize that there are exisiting models that are primarily used for prompt engineering by companies, but we wanted to make this skill available as a resource for the ordinary individual. Using this model, users can improve their day-to-day prompts to yield better prompts -- getting better returns on their interaction with AI. Not only this, but users also have the opportunity to observe and improve their own prompt engineering skills by observing the outputs of our model.
## Dataset
- Dataset was constructed according to guidelines obtained from [OpenAI's Best Practices for Prompt Engineering](https://help.openai.com/en/articles/6654000-best-practices-for-prompt-engineering-with-openai-api).
- A few prompts were generated according to the guidlines manually by authors. Following this, ChatGPT was used to generate similar contrasting prompts in high amount and speed.
- Generated prompts were compiled into a single .csv file that served as the dataset pushed to HuggingFace to be used to train the model.
- Latest dataset can be found [here](https://huggingface.co/datasets/NateBenz/formatted_prompts) 
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

'pip install autotrain-advanced'

What is AutoTrain Advanced?
AutoTrain Advanced processes your data either in a Hugging Face Space or locally (if installed locally using pip). This saves one time since the data processing is not done by the AutoTrain backend, resulting in your job not being queued. AutoTrain Advanced also allows you to use your own hardware (better CPU and RAM) to process the data, thus, making the data processing faster.

Using AutoTrain Advanced, advanced users can also control the hyperparameters used for training per job. This allows you to train multiple models with different hyperparameters and compare the results.

Everything else is the same as AutoTrain. You can use AutoTrain Advanced to train models for NLP, CV, Speech and Tabular tasks.

We recommend using AutoTrain Advanced since it is faster, more flexible and will have more supported tasks and features in the future.

## Limitations and Possible Future Capabilities
### Limitations
- Currently the model was not trained with a large enough dataset to generate consistent, viable fine-tuned responses.
- 

### Future Capabilities
- Based on the limiations of the current version, an increased dataset to train the model would yield a better model.
- Making this model usable as a Google extension, so that users have easy access to it and have it as company.
- Using responses from the user to apply concepts of reinforcement learning to further better the model.



## Resources Used
- [PromptEngineering](https://youtu.be/LslC2nKEEGU)
- [1littlecoder](https://youtu.be/eeM6V5aPjhk)
- [Accelerate Documentation](https://huggingface.co/docs/accelerate/index)
