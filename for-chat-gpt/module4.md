# Module 4: Few Shot Examples

- [Few-shot Examples](#few-shot-examples)
- [Few-shot Examples for Actions](#few-shot-examples-for-actions)
- [Few-shot Examples with Intermediate Steps](#few-shot-examples-with-intermediate-steps)
- [Writing Effective Few-Shot Examples](#writing-effective-few-shot-examples)
	- [ChatGPT on few-shot prompt considerations](#chatgpt-on-few-shot-prompt-considerations)
- [Chain of Thought Prompting](#chain-of-thought-prompting)
- [ReAct Prompting](#react-prompting)
	- [Learn more about ReAct](#learn-more-about-react)
- [Using Large Language Models to Grade Each Other](#using-large-language-models-to-grade-each-other)
- [Exercise](#exercise)
- [Answer: Yes](#answer-yes)



## Few-shot Examples

Give input and output that you'd expect we are teaching the LLM by example

```txt
input:
output:
```

LLMs learn patterns to predict what the next word will be.

## Few-shot Examples for Actions

Can ask it to generate more examples based on the pattern

Then can edit responses and feedback to the LLM or another LLM to train it.

## Few-shot Examples with Intermediate Steps


```txt
think/situation:
action:
think/siutation:
action:
```

Can give it a pattern with intermediate steps and then just give it a situation and it will come up with the intermediate steps using the LLM's computational abilities.


## Writing Effective Few-Shot Examples

Better to use descriptive prefixes than generic "input" and "output". Better named variables provide more information.

Quotation marks for values

Do examples give enough information to derive the expected value?
If you asked 100 humans would it be clear what they were asked to do without any ambiguity?

Is it more effective to provide a rule at the top of the prompt to give more context than giving more examples?

### ChatGPT on few-shot prompt considerations

> in a "few-shot" prompt, what are the most important things to keep in mind

When crafting a “few-shot” prompt, here are the key considerations to ensure effectiveness:

1. Clarity of Instructions

	•	Explicit Prompting: Clearly describe the task or behavior you expect from the model.
	•	Avoid Ambiguity: Use unambiguous language to reduce misinterpretation.

2. High-Quality Examples

	•	Representative Examples: Choose examples that align closely with the desired output.
	•	Diversity: Cover a range of variations within the task to improve generalization.
	•	Correctness: Ensure all examples are error-free and demonstrate the correct behavior.

3. Consistency in Formatting

	•	Standardized Structure: Maintain a consistent input-output format for all examples.
	•	Separator Usage: Use clear delimiters between examples to avoid confusion (e.g., --- or ###).

4. Relevance of Examples

	•	Domain Specificity: Include examples relevant to the specific domain or style you are working with.
	•	Context Appropriateness: Avoid irrelevant or overly complex examples that might distract the model.

5. Quantity of Examples

	•	Balance: Include enough examples to provide context but not so many that it exceeds the token limit or confuses the model.
	•	Optimal Range: Typically, 3-5 examples work well for most tasks.

6. Explicit Signal for New Task

	•	Clear Transition: Use a phrase like “Now you try” or “New example” to indicate where the few-shot examples end and the new task begins.

7. Adaptation to Model

	•	Model Size: Larger models might benefit from slightly more complex examples, while smaller models may need simpler ones.
	•	Token Limit Awareness: Stay within the token limit to ensure all examples and instructions are processed.



## Chain of Thought Prompting

"Showing our work"

Here's the example. Here's the reasoning. Here's the answer.

> summarize this paper
https://arxiv.org/pdf/2201.11903


> The paper "Chain-of-Thought Prompting Elicits Reasoning in Large Language Models" introduces a method called chain-of-thought prompting to enhance the reasoning capabilities of large language models. This technique involves providing models with exemplars that include intermediate reasoning steps, enabling them to decompose complex problems into manageable parts. The authors demonstrate that this approach significantly improves performance on tasks requiring arithmetic, commonsense, and symbolic reasoning. Notably, when applied to a 540-billion-parameter language model, chain-of-thought prompting achieved state-of-the-art accuracy on the GSM8K benchmark for math word problems, surpassing even fine-tuned models.

<details>
<summary>More detailed summary</summary>

```text
provide a more detailed summary
```

> The paper *"Chain-of-Thought Prompting Elicits Reasoning in Large Language Models"* explores an innovative approach to improve the reasoning capabilities of large language models (LLMs). The core idea is **chain-of-thought (CoT) prompting**, which incorporates explicit intermediate reasoning steps in the model's output during problem-solving. This technique is particularly effective for tasks requiring multi-step reasoning, such as arithmetic, symbolic reasoning, and commonsense understanding.

Key Contributions:
1. **Chain-of-Thought Prompting**:
   - CoT prompting involves constructing exemplars where reasoning steps are explicitly laid out, guiding the model to produce more interpretable and structured responses.
   - For example, instead of directly outputting an answer, the model is prompted to break down the problem into smaller steps.

2. **Evaluation**:
   - The authors evaluated CoT prompting on tasks including math word problems, commonsense reasoning, and symbolic reasoning.
   - On the GSM8K benchmark for math word problems, CoT prompting led to significant performance improvements, achieving **state-of-the-art results**.

3. **Model Scalability**:
   - The effectiveness of CoT prompting is strongly correlated with model size. While smaller models showed limited improvement, large-scale models (e.g., a 540-billion-parameter model) demonstrated exceptional gains in reasoning performance.

4. **Interpretability**:
   - By generating intermediate reasoning steps, CoT prompting enhances the interpretability of the model's output, making it easier to understand how the model arrived at its conclusions.

5. **Comparison with Other Methods**:
   - The study shows that CoT prompting can outperform traditional methods like fine-tuning on reasoning tasks, emphasizing its potential as a lightweight and generalizable solution.

Experimental Results:
- On the GSM8K dataset, the CoT-prompted model achieved an accuracy of **58%,** significantly surpassing the previous state-of-the-art of 55% achieved by fine-tuned models.
- Improvements were also observed across other benchmarks, such as the AQUA-RAT dataset for reasoning and OpenBookQA for commonsense reasoning.

Implications:
The findings highlight the potential of leveraging CoT prompting to unlock latent reasoning capabilities in LLMs, particularly for large-scale models. This method requires no additional training, making it a practical and efficient enhancement to existing models.

The paper provides insights into the scalability of reasoning abilities in LLMs and emphasizes the importance of intermediate reasoning for complex problem-solving tasks.

</details>

## ReAct Prompting

Teach LLM on steps to take some other tool to perform actions and provide results

```text
Task:
Think:
Action:
Result:
```

Tool "LangChain" uses ReAct under the hood.


### Learn more about ReAct

[ReAct: Synergizing Reasoning and Acting in Language Models](https://arxiv.org/abs/2210.03629)

<details>
<summary>Summarize paper</summary>


> The paper titled “ReAct: Synergizing Reasoning and Acting in Language Models” introduces a novel approach that enables large language models (LLMs) to interleave reasoning and action generation, enhancing their problem-solving capabilities. ￼

Key Contributions:

	1.	Interleaved Reasoning and Acting: The ReAct framework allows LLMs to produce reasoning traces alongside task-specific actions. This integration enables models to plan, monitor, and adjust actions effectively while managing exceptions during task execution.
	2.	Enhanced Interaction with External Sources: By generating actions, models can interface with external knowledge bases or environments, facilitating information gathering and decision-making beyond their internal knowledge.
	3.	Improved Performance on Diverse Tasks: ReAct has been applied to various language and decision-making tasks, demonstrating superior performance over state-of-the-art baselines. Notably, it addresses issues like hallucination and error propagation in chain-of-thought reasoning by interacting with external APIs, leading to more accurate and interpretable task-solving trajectories.
	4.	Human-Like Problem Solving: The approach generates reasoning and action sequences that resemble human problem-solving methods, enhancing the interpretability and trustworthiness of the model’s outputs.

Applications Demonstrated:

	•	Question Answering (HotpotQA): ReAct reduces hallucinations by consulting external sources, resulting in more accurate answers.
	•	Fact Verification (Fever): The framework effectively verifies facts by cross-referencing information, mitigating error propagation.
	•	Interactive Decision Making (ALFWorld and WebShop): ReAct outperforms imitation and reinforcement learning methods, achieving higher success rates with minimal in-context examples.

In summary, the ReAct framework enhances LLMs by combining reasoning and acting capabilities, leading to improved performance, interpretability, and adaptability across a range of complex tasks.

</details>

## Using Large Language Models to Grade Each Other

Use LLM to evaluate/grade itself or another LLM

Give a few examples with the expected output score

```text
input:
output:
explanation:
grade:
```


## Exercise

1. Write a prompt and test it with ChatGPT or another large language model that uses few-shot examples to teach the large language model to perform a complex task. Provide the prompt and sample output from using the prompt.

```text
For ballet positions in grande plie
do heels lift off the floor?

Position: First
Answer: Yes

Position: Second
Answer: No

Position: Fifth
Answer:
```

Position: Fifth
Answer: Yes
---

1. Question 2
Write a prompt and test it with ChatGPT or another large language model that uses few-shot examples to teach the large language model to perform a complex task that requires performing intermediate sub-steps. Provide the prompt and sample output from using the prompt.

```text
Driving example in a neighborhood with narrow streets.
Situation: driving from home and turning right at a stop sign.
Action: accelerate car to speed limit of 25 mph.
Thought: do not go over the speed limit
Action: before stop sign take foot off accelerator to slow car.
Thought: driving as smoothly as possible saves wear and tear on the brakes
 and provides a more comfortable experience.
Action: Finally apply brakes to not go over the line.
Thought: obey rules of the road for safety.

Situation: turn right from a stop sign.
Action: turn on blinker to signal a right turn.
Thought: cross traffic or any cars behind
know where you intend to go.
Action: Look left, then right and then left again.
Thought: make sure there are no pedestrians, animals,
 or automobiles coming that you might run into.
Action: gently accelerated while turning right.
Thought: driving slow at first is safer
because you could see things you missed.

Situation: car parked on left side of the Street
Action: slow down while passing the parked car
 on the other side of the road.
Thought: there may be people or animals that are blocked from view
 who may dart out into traffic.
Action: after passing car accelerate back to the speed limit.
Thought: after it's clear and there are no obstructions
then it is safe to resume normal speed.

Situation: car parked on right side of the street
 that necessitates passing by going into the opposite lane.
Action: slow down.
Thought: be prepared to stop if there is a car coming
 on the opposite side of the road.
Action:
```

<details>
<summary>Response</summary>

Action: Check for oncoming traffic and wait if necessary. If clear, gently steer into the opposite lane while maintaining a slow speed.
Thought: Crossing into the opposite lane requires extra caution to avoid potential collisions.

Action: Pass the parked car while staying alert for pedestrians or animals.
Thought: Always be aware of any sudden movements or hidden obstructions around the parked car.

Action: Return to your lane as soon as it is safe to do so.
Thought: Staying in the correct lane ensures you comply with traffic rules and minimize risks to oncoming vehicles.

Would you like to expand on this example or add more situations?

</details>

[previous](./module3.md) | [next](./module5.md) | [top](#module-4-few-shot-examples) | [course](./readme.md)
