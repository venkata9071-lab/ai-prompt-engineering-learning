Module 1: Finding Information
The AI novice vs AI power user

## what i learned was

An AI novice usually asks short questions and expects the model to fill in the missing information like they expect the accurate information 

An AI power user gives useful background information, uploads relevant files then he  asks the model to analyse carefully think hard then answer it 

and also improves the answer through follow-up prompts.

like by doing iterations.

#### what i find was 

Give enough context for ai kije images,files etc then give the prompt

Instead of asking AI to write the final content immediately, I can use this process:

Notes  

Outline it

Review  

Improve  

Bullet points  

Final draft  


## Pretrained Knowledge

Pretrained knowledge is what AI learned from public text during training.
it has sometime which is trained till there if asks llm to answer the tend it will face difficult to answer accurately insted it will search it and answer it accurately.

Like It may work well for common and stable topics, but it may be weaker for:

- recent information,
- rare topics,
- private information,
- company-specific data.

## Web Search

Web search is useful for:

- current news,
- recent product information,
- finding prices, weather,schedules,
- About the niche topics.

my note :- I should request web search when the answer may have changed after the model's knowledge cutoff.

For the web search sources

Web search doesn't automatically mean the answer is correct.

like for example 

how safe are the minoxidil petides? if i as this LLm may search the social media, blogs and untrusted websites 

for the more trusted resocures to search 

giving prompt like How safe are the minoxidil peptides? only use the sources like offical trusted health orgnaztions like who,fba, nhs and look at the studies which is backed by rigorous science. 

As a result it will search like WHO, FDA, NHS and trusted resources.

So,the quality of the answer depends on the quality of the websites the AI uses.


 Deep Research
 What I Learned

Deep Research is much more advanced than a normal web search.

Instead of searching only a few pages, it will mainly do these

- creates a research plan
- searches multiple sources
- compares information
- performs additional searches if required
- analyses the findings
- generates a detailed report with citations

so, this process can take few minutes 

for Example i have tried this prompts in deep search in chtgpt deepsearch

- Compare Azure Synapse vs Microsoft Fabric.
- Research the safest hair-loss treatments using official medical sources in uk
- Compare universities for MSc Data Engineering in current new fees structure

These tasks normally require reading many webpages manually, but Deep Research can do most of the work.

 Module 2

Brainstorming with AI
 
 brainstroming with ai and adding more context it get more better answers or ideas.

so, AI is very good at generating multiple ideas and possible solutions.

Instead of asking for one answer, I should ask for several options and compare them.

For example, 

 if i ask about the name the 200 potential uses for a brick. The purpose isn't to use every idea but to explore many possibilities and choose the best one.

Brainstroming : The more ideas, the better answer

Instead of asking:

Build me a gym workout plan for lean bulk near gym group i have took the plan

I tried giving AI more information.

"
I am 26 years old.
I recently joined the gym.
I am a beginner.
I can train for 1 hour every day.
My goal is lean bulking.
I have a slight shoulder injury.
"

Suggest 3 workout plans.

The response became much more personalized because AI understood my situation.

This helped me understand that:

More context = Better output.


I learned the Brainstorming is Iterative

Another lesson I learned is that brainstorming also a iterative process.

Instead of expecting the perfect answer immediately, I should continue working with AI.

The workflow looks like this:

Give context
   
   then

Ask for multiple options

    then

Review the responses

    then

Give feedback

    then

Ask AI to improve the ideas

    then

Repeat these iteration process to get the best ption in it 


Tso, this produces much better ideas than stopping after the first response.

Understanding Context


context means every piece of information AI uses to generate its answer.

Context can include:

- My prompt
- Uploaded documents
- PDFs
- Images
etc

All of these together help AI produce a better response.

For  Example

If I ask:

Should I study Physics or Zoology?


AI gives a generic comparison because it doesn't know anything about me.

But if I also provide:

- My career interests
- School grades
- Subjects I enjoy
- Career goals

AI can give advice that is much more relevant to my situation.

 AI Desktop Apps



Unlike ChatGPT where I manually upload files, desktop AI apps can search my computer (with permission), find relevant files, read them, and use them as context.

Examples include:

- Claude Desktop
- chagpt app etc

I have tried the claude cowork installed in laptop then given permissions for accessing the files i tried to automate the job application process like i given prompt use my resume and cover letter and get the data engineer roles extract into sheet and using given context apply the jobs for last 24 hours.

I have given the all context about the my details etc

it applied few applications.

and also Instead of uploading every file manually, AI can search only the files it needs.

My learning was

- AI is much better when treated as a thinking partner.
- Good brainstorming requires multiple iterations.
- Context is one of the biggest factors affecting response quality.
- More relevant information leads to better personalized answers.
- Conversation history becomes part of AI's context.
- Start a new conversation when changing topics completely.
- AI desktop apps reduce manual work by automatically finding relevant files.
- Always review AI's plan before allowing it to modify files.

 Module 3 was Working with Multimedia and Code

What I Learned

This module helped me understand that AI  can work with images, audio, video, code, and data and analyze the picture and can describe as well.

so,my main learning is that multimodal AI can take different types of input and also create different types of output. For example, I can upload an image and ask the  AI to explain it and  edit it, or use it as i want new on elike take the inspiration from this.

Working with Multimedia

what i learned was this LLm like chatgpt can text , image, audio etc 


I got  that text is usually faster and cheaper to generate.

 Images take longer, and video usually takes the most time and cost.so, mage and video is costly and take time compare to text for any LLms


what I understand was  from an image, like llms can see the

objects
basic text
handwritten notes in it

receipts
diagrams etc

However, it may miss small details from it we can get the ouput by doing iteration of prompts with AI

For example,

i tried in gym today evening i have upload the  two gym machines may look similar, so AI has detected the one machine which is split machine but other one it told butt builder but it wrong it is tricep machine 
so, what i have noted was it  may give the wrong name if the image is unclear.



I learned that image prompts should clearly describe:

the main subject
the setting
important detail
mood
visual style etc


what i understand was Image generation is useful for brainstorming ideas, but it may still make mistakes with text, hands, or character consistency.


Building Apps with AI

what i learned was AI can also write code and create simple websites or games from a text prompt.

A useful app prompt should explain:

1. The goal of the app
2. What the user will input
3. What the app should output

For example:

 Build a bill-splitting calculator where users enter the total bill and number of people, and the app shows how much each person should pay.

I understood that simple and clearly defined apps are easier for AI to build than complex applications.

 Data Analysis

AI can analyse spreadsheets and other structured data by writing and running code.

For example, I can upload sales data and ask:

Which products had the biggest changes in sales? Create a graph and explain the main trends.

AI may inspect the data or calcutare the total or average in it and it will identify the patterns in it , generate charts, explain the useful findins in it.


Lab example

I have tried to create a spiderman game by doing brainstroming  then researching it, finally the build it

I have used this prompt :- “Build a Spider-Man game” is too broad and may produce a generic or unmanageable result. By adding context about the city, player movement, traffic, pedestrians, enemies, visual style and development stages, the AI can understand the game more clearly and produce a practical, structured development plan.

Context used : Help me design and build a simple third-person web-swinging superhero game. The game should take place in a colourful modern city with tall skyscrapers, apartment buildings, shops, construction sites, roads, traffic and pedestrians. Main goal: The player controls a web-slinging superhero who can move freely through the city, stop crimes and fight enemies. Player movement: - run and jump - climb walls - wall-run - swing between buildings using webs - release the web to gain momentum - dive while falling - perform simple air tricks - land on rooftops, walls and streets City: - buildings of different heights - wide and narrow streets - rooftops with water tanks, air conditioners and antennas - moving cars, taxis, buses and police vehicles - pedestrians walking on pavements - daytime and sunset lighting Traffic: - vehicles follow fixed road paths - vehicles stop at traffic lights - pedestrians react when combat begins - police vehicles appear during crimes Enemies: - basic street criminals - armed enemies - heavy enemies - rooftop snipers - flying drones Combat: - punches and kicks - dodge - web shot - web pull - attach enemies to walls - throw nearby objects - air attacks Missions: - stop a robbery - chase a stolen vehicle - rescue a civilian - defeat enemies on a rooftop - complete a web-swinging time trial Visual style: - colourful comic-inspired city - red and blue superhero suit - smooth movement animations - bright daytime colours - orange and purple sunset lighting Start by building a small playable prototype, not the full game. The first prototype should contain: 1. One small city block 2. Five buildings 3. Basic player movement 4. One working web-swing mechanic 5. A few moving cars 6. Three basic enemies 7. One simple mission 8. A restart button Before writing code, create a development plan. Divide the game into small stages and explain which feature should be built first.