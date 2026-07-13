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