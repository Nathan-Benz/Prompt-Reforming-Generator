# Prompt-Reforming-Generator
Using Meta's Llama 2 LLM, we fine tune the model to be optimized for turning "bad" prompts that yield an inefficient response into "good" ones which are optimal prompts that generate fruitful responses.

# Packages

We used a very strong package in, AutoTrain, to fine-tune the open-source Llama V2 assistant for our purpose.
 - The one-liner code included in the training section is achieved through this package.
 - Usually, a large-scale fine-tuning processes would take a strong GPU, but the small dataset we have allows the fine-tuning at a smaller scale.
