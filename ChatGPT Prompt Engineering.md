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

---

### Prompt 2

Checked the tea-making paragraph.

**Observation**

The AI found the instructions and converted them into numbered steps.

### Key Takeaway

Check the condition before doing the task.

---

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

---

### Prompt 2

Teacher explaining Azure services.

**Observation**

The AI answered in the same simple teaching style as the first example.

### Key Takeaway

Give examples first, then ask the task.