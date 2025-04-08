OBS: Vi kan bruge hvad vi synes er godt og paste det ind i [part 1 markdown filen](./part1.md)

# Part 1.1
## Traits

Traits are the desired characteristics of the AI or its response. For instance you could want the AI to act as a profressional developer when the response must be professional and up to standard. Alternatively you could tell it to be formal or casual.
Furthermore you could define the structure of it's response and tell it to respond in bulletin-format or code-only - or perhaps in a paragraph of text.

## Tasks

The task is the instructions you give to the AI directly, like telling it.
``` 
Convert this text into professional format
```
``` 
Generate 5 riddles
```

## Tone
Setting the tone for the AI response can greatly affect the output it generates. Say for instance you wanted some notes written as a casual letter for a friend, or if in another instance you wanted stray thoughts and letters to be turned into a formal letter to a boss, the tone can have an impact on how the output comes across.

Aside from general wording and defining how comfortable the AI can be in its speech, the tone can also be used to specify how objective or neutral the AI is in its response. Some people may prefer a more friendly and humorous AI, but others may want a cold and concise coding machine.

## Targets

The target is also known as the intended audience; who you want to recieve the output-content. You may need an output to be written for a class of 1 semester students starting their Bachelor AI-course, or you may want the output written at the quality-level of a profressional programmer.

Often times the AI will infer what the purpose of its output is for, like when you ask it to patch code or when you ask it to formalise text; but its often a good idea to specify this to get the best results out of a prompt.

# Part 1.2

Each component in prompt engineering plays a crucial role in shaping the desired behavior and thought process to achieve a specific purpose. The structure of a prompt can vary significantly depending on the needs of the user, ensuring it aligns with their goals and expectations.

* Traits can help set the context of a problem and define what kind of 'specialist' is needed:
**"You are a programming god"**

* Tasks tells the AI what needs to be done. This is by far the most important of the 4 T's as this is the raw instructions.

* Tone helps adjust the structure of the output allowing it to be kind, mean, formal or informal; the possibilities are endless and they help shape the response to what the user needs
* Targets can be used to have the AI understand who the intended audience is as there may be a big difference between explaining code to a professional Python programmer and a complete beginner.

# Part 1.3

### Poorly Written Prompt: 
```
Tell me about apples.
```


Revised Prompt (using the 4 T's):

* Traits: Provide a concise summary (around 100 words) in bullet points.
* Tasks: Explain the nutritional benefits of eating apples.
* Tone: Use an informative and encouraging tone.
* Targets: Aim this explanation at someone interested in healthy eating habits.

The revised prompt could look something like this:
```
Tell me the key nutritional benefits of eating apples in a concise bullet-point list of around 100 words, using an informative and encouraging tone, for someone interested in healthy eating habits.
```

There are many things the AI could say about apples; hereof their history, the tastes across different continents or the compositional-structure. 

By defining a more specific prompt using the 4 T's, we have aimed its focus at explaining the neutritional benefits and directing that at someone interested in healthy eating. This could for example be substituted for writing the response for a potential customer or written to convince someone to eat more apples. It can be specified to the user's specific desire.


# Part 1.4 

An alternative to the 4 T's could be the ICIO-structure as nicely explained in the following [Article by Medium](https://medium.com/@edu360harvey/navigating-the-complexities-of-prompt-engineering-in-ai-advanced-frameworks-and-practical-358a6bd8aa01)

The model is structured as follows:

* Instruction: This is similar to the second T in the 4 T's (Tasks) and defines what the AI should do; the instructions if you will.

* Context: This provides the AI with the background information needed to understand context or why it is doing its instructions. 

* Input data: This is where the user can provide information or data in alignment with the **Context** to further specify what needs to be done. This could for example be a list of JSON-objects, written knowledge, incomplete notes or other forms of supplementary data.

* Output indicator: This is similar to the  4 T's last 2 points, **Tone** and **Targets**. This part specifies the format and nature of the output. Similar to the 4 T's you can either explicitly tell it the format:
```
Output in a short paragraph
```
```
Output with no explainations and only bullet-points
```
Alternatively it can also be implied in the nature of the output, for example
```
Make this text longer and emphasize how good ICIO can be
```
Where this prompt in itself implies that the AI needs to ouput text and that it must be similar to the inputted text.

## Could ICIO have an advantage over TTTT?

One potential advantage of the ICIO framework is its ability to handle tasks like SQL code refactoring more effectively. For example, we often use AI when working with SQL, where we provide the instruction "Give this query X functionality," the **Context** can be supplied through DDL or table structures, enabling the AI to understand the properties of each entity (relation) and know what they are called. In this scenario the ICIO shines and is preferred over the 4 T's as there no necessity over defining a target, tone or even traits, as the format is inferred through the input SQL.