# Patterns

[A Prompt Pattern Catalog to Enhance Prompt Engineering with ChatGPT](https://arxiv.org/pdf/2302.11382.pdf)

- [Summary of the patterns created by Adam Garry, Dell Director of Global Education Strategy](#summary-of-the-patterns-created-by-adam-garry-dell-director-of-global-education-strategy)
- [Pattern Category Prompt Pattern](#pattern-category-prompt-pattern)
- [Input Semantics](#input-semantics)
  - [Meta Language Creation](#meta-language-creation)
- [Output Customization](#output-customization)
  - [Output Automater](#output-automater)

## Summary of the patterns created by Adam Garry, Dell Director of Global Education Strategy

[Prompt Techniques Table | Prompt Technique | Description](https://chatgpt.com/share/9a3f08ab-9b58-4378-84eb-299b51e70dab)

[Prompt Patterns: Overview](https://chatgpt.com/share/c6209ab2-d816-40fa-adf5-9dfe6c40efaf)


## Pattern Category Prompt Pattern


| Pattern Category | Prompt Pattern |
| :---------------- | :-------------- |
| Input Semantics | Meta Language Creation |
| Output Customization | Output Automater <br/> Persona <br/> Visualization Generator <br/> Recipe <br/> Template |
| Error Identification | Fact Check List <br/> Reflection |
Prompt Improvement | Question Refinement <br/> Alternative Approaches <br/> Cognitive Verifier <br/> Refusal Breaker |
| Interaction | Flipped Interaction <br/> Game Play <br/> Infinite Generation <br/>
| Context Control | Context Manager

## Input Semantics

### Meta Language Creation

| Contextual Statements |
| :-------------------- |
|When I say X, I mean Y (or would like you to do Y) |

```text
From now on, whenever I type two identifiers
separated by a “→”, I am describing a graph. For
example, “a → b” is describing a graph with nodes
“a” and “b” and an edge between them. If I separate
identifiers by “-[w:2, z:3]→”, I am adding properties
of the edge, such as a weight or label.
```

## Output Customization

### Output Automater

```text
From now on, whenever you generate code that
spans more than one file, generate a Python script
that can be run to automatically create the specified
files or make changes to existing files to insert the
generated code.
```


