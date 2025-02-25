# Introduction to Prompt Patterns

## Question Refinement Pattern


```text
When I ask a question, suggest a better version
 of the question to use instead.
Prompt me if I would like to use the better version instead
 and if I confirm, answer the question.
If I say no or NA or N/A,
 suggest a different version of the question
 and continue with the same interaction.
```

## Cognitive Verifier Pattern

```text
When you are asked a question, follow these rules

Generate a number of additional questions
that would help more accurately answer the question.

Combine the answers to the individual questions
to produce the final answer to the overall question.
```

## Audience Persona Pattern

```text
For each question I ask
provide outputs that persona X would understand.
```

## Flipped Interaction Pattern


```text
I would like you to ask me questions to achieve X
Ask me questions one at a time
until you have enough information to answer the question
or to achive this goal.
```

```text
When you are asked a question, follow these rules

Generate a number of additional questions
 that would help more accurately answer the question
 or meet the goal.
Ask these questions one at a time.
If I answer NA or N/A
 proceed to the next question.

Combine the answers to the individual questions
 to produce the final answer
 to the overall question or to meet the goal.
```


## Quiz

1. Write a prompt and test it with ChatGPT or another large language model that uses the Question Refinement Pattern. Provide the prompt and sample output from using the prompt to refine several different questions.

2. Write a prompt and test it with ChatGPT or another large language model that uses the Cognitive Verifier Pattern. Provide the prompt and sample output from using the prompt to better answer several complex questions or improve the performance on a complex task.

[previous](./module2.md) | [next](./module4.md) | [top](#introduction-to-prompt-patterns) | [course](./readme.md)
