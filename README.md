# chatgpt-prompt-engineering
Jupyter code notebooks of "ChatGPT Prompt Engineering for Developers" by DeepLearning.AI and OpenAI.


## After many days I am again doing my hands dirty with AI/ML and from past 4 months I have been working closely on OpenAi's GPT model.

This course is presented by one of my favourite professor Andrew Ng.

Here, in this short course taught by Isa Fulford (OpenAI) and Andrew Ng (DeepLearning.AI) they will describe how LLMs work, provide best practices for prompt engineering, and show how LLM APIs can be used in applications for a variety of tasks, including:

1. Summarizing (e.g., summarizing user reviews for brevity)
2. Inferring (e.g., sentiment classification, topic extraction)
3. Transforming text (e.g., translation, spelling & grammar correction)
4. Expanding (e.g., automatically writing emails)


### Guidelines

There are two principles for prompting -

**1. Write clear and specific instructions.** (clear dosen't means short, often times longer prompts are better for the task which we wanted from the model to execute clearly which means longer prompts actually provide more clarity and context for the model, which can actually lead to more  detailed and relevant outputs)

**Tactic 1** -  Use Delimiters (Triple Quotes{"""}, Triple backticks{``` ```}, Triple Dashes{---}, Angle Brackets{<>}, XML Tags {<tag> </tag>}

**Tactic 2** -  Ask for a Structured output.(JSON, HTML)

**Tactic 3** - Ask the model to check whether conditions are satisfied.(if the task makes assumptions that aren't necessarily satisfied, then we can tell the model to check these assumptions first and then if they're not satisfied, indicate this and kind of stop short of a full task completion attempt. You might also consider potential edge cases and how the model should handle them to avoid unexpected errors or result.)

** Tactic 4** - "Few-shot" prompting.(just providing examples of successful executions of the task you want performed before asking the model to do the actual task you want it to do.)

2. Give the model time to "think"

**Tactic 1**- Specify the steps required to complete a task (If a model is making reasoning errors by rushing to an incorrect conclusion, you should try reframing the query to request a chain or series of relevant reasoning before the model provides its final answer. Another way to think about this is that if you give a model a task that's too complex for it to do in a short amount of time or in a small number of words, it may make up a guess which is likely to be incorrect.)

**Tactic 2**- Instruct the model to work out its own solution before rushing to a conclusion

