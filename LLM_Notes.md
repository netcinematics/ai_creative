# intro large language models
- subset of deep learning
- LLM pre-trained and fined tuned for apps
- dog: sit, come, stay, down
- special: police, guide, hunting
- general purpose training, 
- classify, q n a, summary, text generation
- retail, finance, entertainment.
## Features
### large 
= petabyte and parameter count, 
- hyper paramters in ml
- define skill
### general purpose
- commonality of language
- resource restriction
### pre trained and fine tuned
- general purpose, then smaller db
## general use
- few-shot: train model with miminum data
- zero-shot: not specifically trained
### PaLM
- april 2022, 540 billion
- dense decoder only, new pathway system
- multipl tpu v4 pods
- many tasks at once, quickly
- distributed computation for accellerators.
- encoder and decoder of representations
###
foundation language models from prompt
### comparison
llm no need to be expert or train,
just think prompt design
clear concise informative,
### traditional: training, compute time, hardware
## EXAMPLE text genration QA
- domain knowledge, not necessary
### Prompt Design / Engineering
- design tailors to specific task
- design instructions, context, input for output
- PE: develop and optimize prompts for apps.
- PE: performance, domain, example
- PE: more specialized, for accuracy/performance
## 3 types of LLMs
1. Generic / Raw LLM
 - predict what comes next (token)
- dialog by predicting next response.
- token: atomic unit for LLM.
- vector representation of input and next output
2. Instruction Tuned lLM
- response given an input, conversational
3. Dialog Tuned (framed as questions)
- special case of instruction tuned.
- natural question like phrases
### Chain of Thought Reasoning
- Models better, if first output reasoning.
- Task Specific tuning make models more reliable
### Tuning
- customize, based on examples,
- adapting model to new domain, per new data
- legal or medical
- fine tuning, byodataset, hosting model.
### Fine tuning
- expensive not realistic
- PETM Parameter Efficient (no duplication)
- on Custom data, add on layers, at inference time.
### GenAI
- explore, custom, fine tune on google cloud.
### GenAI app builder.
Palm API experiment with LM, MakerSuite GUI
- model train, deploy, monitor.
