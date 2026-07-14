# Introduction

chatgpt prompt engineer

## what i learn was

1. There are 2 types of LLMs.
2. Base LLM predicts next word.
3. Instruction LLM follows instructions.
4. Clear prompts give better answers.

so, clear prompts = better output.


# Prompt Guidelines

## Principle 1: Write Clear and Specific Instructions

### Tactic 1: Use Delimiters

### What I learned

- Delimiters separate the instruction from the input.
- AI understands exactly which text to process.
- Different delimiters like ```, """, and XML tags all work.
- Delimiters also help reduce prompt injection by treating the input as text instead of a command.

### Hands-on

#### Prompt 1

Summarize the text inside triple backticks into one sentence.

#### Prompt 2

Summarize the text inside XML tags.

#### Prompt 3

Summarize the text inside triple quotes.

### Observation

All delimiters worked well. The AI  has clearly understood which text it needed to summarize.

### Key Takeaway

Clear separation = Better understanding.

---

## Tactic 2: Ask for a Structured Output

### What I learned

- AI can return responses in a fixed format like JSON or HTML.
- Structured output makes the response organized and easier to read.
- JSON is useful because applications can easily process the data.
- Giving the required keys helps the AI return consistent results.

### Hands-on

#### Prompt 1

Generate a list of five travel destinations in JSON format.

#### Observation

The AI returned all travel destinations with the required keys in proper JSON format.

---

#### Prompt 2

Generate a list of three students in JSON format.

#### Observation

The AI followed the requested structure and included all the specified keys.

### Key Takeaway

Structured output = Easy to read and use.

### Example

#### prompt
can you generate a list of five travel destinations and provide them in json format with these keys place_name, country, destination_id, avg_temperature 

#### output from LLM

[ { "destination_id": 1, "place_name": "Bali", "country": "Indonesia", "avg_temperature": "28°C" }, { "destination_id": 2, "place_name": "Santorini", "country": "Greece", "avg_temperature": "24°C" }, { "destination_id": 3, "place_name": "Kyoto", "country": "Japan", "avg_temperature": "16°C" }, { "destination_id": 4, "place_name": "Banff National Park", "country": "Canada", "avg_temperature": "4°C" }, { "destination_id": 5, "place_name": "Cape Town", "country": "South Africa", "avg_temperature": "18°C" } ]

# Tactic 3: Check Whether Conditions Are Satisfied

## What I learned

- Before doing the task, the AI first checks if the condition is satisfied.
- If the condition is true, it completes the task.
- If the condition is false, it returns the response what i have asked for
- This helps avoid  wrong or unnecessary answers.

## Hands-on

### Prompt 1

Checked if the text had instructions.

**Observation**

The text didn't have any instructions, so the AI returned **"No steps provided."**


### Prompt 2

Checked the tea-making paragraph.

**Observation**

The AI found the instructions and converted them into numbered steps.

### Key Takeaway

Check the condition before doing the task.


# Tactic 4: Few-shot Prompting

## What I learned

- Few-shot prompting means giving the AI one or more examples first.
- The examples help the AI understand the style and format I want.
- After seeing the examples, the AI continues in the same way.
- This gives more consistent answers.

## Hands-on

### Prompt 1

Child and grandparent conversation.

**Observation**

The AI continued the conversation in the same wise style as the example.


### Prompt 2

Teacher explaining Azure services.

**Observation**

The AI answered in the same simple teaching style as the first example.

### Key Takeaway

Give examples first, then ask the task.

## Principle 2 : Give the Model Time to Think while answering the complex problems

### Tactic 1

#### What I learned

- mainly Breaking a task into smaller steps which gives better results for the complex problems and also clear output format makes the response easier to understand.
- The AI follows instructions more accurately when each step is specified.

#### my learning was 

Breaking the complex tasks into simple steps what to do in step by step.


### Tactic 2

#### What I learned

- Ask the AI to solve the problem before checking the given answer.
- Then Comparing its own solution with the given answer i think it will improves accuracy.
- This reduces the chance of incorrect judgments and also giving the explaination by comparing the both solution which will give the best solution

#### my learning was

Solve first, then compare it and explain it.

# Model Limitation: Hallucinations

## What I learned

- Sometimes the AI may also gives answers that sound correct but are actually creating a answers without any evidance.
- This is called a hallucination.
- It usually happens when the AI doesn't have enough information.
- For important information, it's better to verify the answer using a reliable source.

## Hands-on

### Prompt 1

Asked about a fake toothbrush product.

#### Observation

But while checking it in chatgpt, it identifies it its a fake toothbrush


### Prompt 2

Asked the AI to say if it wasn't sure instead of making up information.


The response was more reliable because the AI acknowledged uncertainty.

## learning was

AI can sound sometimes it may confident even when it's wrong, so always verify it important information.
# Iterative Prompt Development

## What I understood

Initially, I thought prompt engineering was about writing one perfect prompt. After this lesson, I understood that's not how it works.

The first prompt doesn't have to be perfect. The important part is improving it step by step based on the output until it gives the result I want.

### My Prompt Development Loop

Write prompt

Run it

Check the result

Find the problem

Improve the prompt

Run it again


## Iteration 1

### Problem

The product description was too long.

### Improvement

Added:

- Use at most 50 words or use the sentence like specifying it 3 sentence etc 

### What I learned

If the output is longer than expected, I should give a clear limit instead of simply saying "make it shorter."

## Iteration 2

### Problem

The description focused on general product details instead of what furniture retailers need.

### Improvement

Specified the target audience and asked the model to focus on materials and technical details.

### What I learned

The model gives better results when I clearly mention who the audience is and what information is important.


## Iteration 3

### Problem

The response didn't include the product IDs.

### Improvement

Added an instruction to include every 7-character Product ID.

### What I learned

If something important is missing, I shouldn't expect the model to guess. I should explicitly ask for it.


## Iteration 4

### Problem

The dimensions were difficult to read.

### Improvement

Asked the model to extract the dimensions and present them in a table.

### What I learned

The model can not only generate text but also organize information into tables, making the output easier to understand.


## Iteration 5

### Problem

The content wasn't ready to use on a website.

### Improvement

Asked the model to format the output as HTML.

### What I learned

The model can generate website-ready content like HTML, which saves development time.


## my Thoughts was


Instead of trying to write the perfect prompt on the first attempt, I should:

- Start with a simple prompt.
- Check the output carefully.
- Identify what is missing or incorrect.
- Improve the prompt step by step.

Every iteration makes the prompt better and gets the output closer to what I actually need.

## Summarizing

### What i have learned

- LLms like chatgpt or claude can turn long text into short summaries.
- I can control the summary using a word or sentence limit.
- I can ask the model to focus on a specific topic.
- The same review can have different summaries for different departments.
- Summarising keeps the main meaning of the whole text.
- Extracting returns only the specific information requested.

#### For Example 

for this text I bought a wireless mouse for work. It connects quickly and feels comfortable, but the battery only lasted two weeks. Delivery was fast and the price was reasonable.

i have used the prompt like summarize this in 10 words or two sentence  and output was comfortable wireless mouse,quick connection,reasonable price,battery lasted fortnight 

- And also summarize the text mainly focus on the auidence or purpose like summarize the text based on shipping etc

extracting the text getting the information what we reuired it only pulls the information only the specific information i asked for 

- Like prompt: extract the battey life output as The battey only lasted two weeks.

### Key Takeaway

The summary should match the purpose and audience.
# Inferring

## What I understood

Inferring means analysing text and finding information such as sentiment, emotions, names, products and topics.

The model can do different text-analysis tasks just by changing the prompt.

## Sentiment

- Sentiment shows whether the overall feeling is positive, negative or neutral.
- Giving a one-word output makes it easier to use in code.

## Emotions

- Emotions are more specific than sentiment.
- The model can detect feelings such as happiness, anger or disappointment.

## Information Extraction

- The model can extract exact details like product name and brand.
- JSON makes the output easy for applications to process.
- If information is missing, I should ask it to return "unknown."

## Multiple Tasks

- One prompt can extract sentiment, anger, item and brand together.
- The expected fields and format should be clearly specified.

## Topic Inference

- The model can identify the main topics in an article.
- It can also check whether specific topics are present.

## Example 

I bought a wireless mouse for work. It connects quickly and feels comfortable, but the battery only lasted two weeks. Delivery was fast and the price was reasonable. what is the sentiment of the review so, return only : postive , negitive, neutral

- llm  has given output positive

I have asked now idnetify the five emotions in it and return in lowercase by commas

- it given the satisfaction, disappointment, comfort, appreciation, frustration

extract the following information like product battery , shipping feedback and price feedback then also return mainly in json format 

- output from llm: {
  "product": "Wireless mouse",
  "battery": {
    "feedback": "The battery only lasted two weeks."
  },
  "shipping": {
    "feedback": "Delivery was fast."
  },
  "price": {
    "feedback": "The price was reasonable."
  }
}

- Customer review analysis
- Urgent complaint detection
- News alerts
- Automatic content tagging

## key point was

I think Analyse text and then  extract useful meaning.
# Transforming

## I learned was

Transforming means changing text or data from one form into another while keeping the main meaning.
like translating the given text into french or telugu

## Translation

- The model can detect the languages and translate the  text.
- It can also  translate into multiple languages and formal and informal too

## Tone like casual or professional etc

- The same message can be rewritten in a casual, professional or formal tone.

## Format Conversion

- The model can convert data between formats such as JSON, HTML and Markdown.
 what i learned was i should given in prompt about he input and output as well

## spell checking or grammer checking

- The model can correct spelling, grammar and punctuation.
using like proofread and correct this sentence 

## Multiple changes we can do in single prompt

- One prompt can correct grammar, change tone and convert format at the same time as well.
# The Chat bot

## What I understood was

The chat format stores every message as a role and content.so,The main roles are system, user and assistant.

This system message controls the chatbot's behaviour.

 user message :- contains what the person says.

 assistant message :-  stores the chatbot's previous reply.

## one thing note was Conversation Memory

The chatbot only remembers earlier information when the full conversation history is sent again.


## OrderBot

The OrderBot uses a system message to define:

- the menu,
- prices,
- questions to ask,
- pickup or delivery,
- the conversation style.

i have tried this example for chatbot 


context = [
    {
        "role": "system",
        "content": """
You are Data Engineering HelpBot.

Your job is to help beginners understand data engineering topics.

You should:
- greet the user,
- ask what topic they want help with,
- explain using simple language,
- give one practical example,
- ask one short follow-up question,
- keep responses concise and friendly.

Topics include:
- Azure Data Factory
- Azure Synapse Analytics
- data lakes
- ETL and ELT
- SQL
- Git
- data pipelines

If the user asks something outside these topics,
politely say you are focused on data engineering.
"""
    }
]
