# Patterns

[A Prompt Pattern Catalog to Enhance Prompt Engineering with ChatGPT](https://arxiv.org/pdf/2302.11382.pdf)

- [Summary of the patterns created by Adam Garry, Dell Director of Global Education Strategy](#summary-of-the-patterns-created-by-adam-garry-dell-director-of-global-education-strategy)
- [Pattern Category Prompt Pattern](#pattern-category-prompt-pattern)
- [Input Semantics](#input-semantics)
  - [Meta Language Creation](#meta-language-creation)
- [Output Customization](#output-customization)
  - [Output Automater](#output-automater)
- [Generated Table of Contents](#generated-table-of-contents)
  - [I. Introduction](#i-introduction)
  - [II. Comparing Software Patterns with Prompt Patterns](#ii-comparing-software-patterns-with-prompt-patterns)
  - [III. A Catalog of Prompt Patterns for Conversational LLMs](#iii-a-catalog-of-prompt-patterns-for-conversational-llms)
  - [Specific Prompt Patterns](#specific-prompt-patterns)
    - [1. Meta Language Creation Pattern](#1-meta-language-creation-pattern)
    - [2. Output Automater Pattern](#2-output-automater-pattern)
    - [3. Flipped Interaction Pattern](#3-flipped-interaction-pattern)
    - [4. Persona Pattern](#4-persona-pattern)
    - [5. Question Refinement Pattern](#5-question-refinement-pattern)
    - [6. Alternative Approaches Pattern](#6-alternative-approaches-pattern)
    - [7. Cognitive Verifier Pattern](#7-cognitive-verifier-pattern)
    - [8. Fact Check List Pattern](#8-fact-check-list-pattern)
    - [9. Template Pattern](#9-template-pattern)
    - [10. Infinite Generation Pattern](#10-infinite-generation-pattern)
    - [11. Visualization Generator Pattern](#11-visualization-generator-pattern)
    - [12. Game Play Pattern](#12-game-play-pattern)
    - [13. Refusal Breaker Pattern](#13-refusal-breaker-pattern)
    - [14. Context Control Pattern](#14-context-control-pattern)
  - [IV. Example Implementations](#iv-example-implementations)
  - [V. Concluding Remarks](#v-concluding-remarks)

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


the generated avatar videos explaining the prompt techniques:

Prompt Techniques Part 1
Prompt Techniques Part 2
Prompt Techniques Part 3
Prompt Techniques Part 4
Prompt Techniques Part 5
Prompt Techniques Part 6
Prompt Techniques Part 7

## Generated Table of Contents

Based on the document content, here's a table of contents for the paper on prompt patterns for large language models:

### I. Introduction
- Overview of prompt engineering techniques
- Importance of prompts in LLM interactions

### II. Comparing Software Patterns with Prompt Patterns
- Relationship between prompt quality and LLM output
- Overview of software patterns
- Adaptation of software patterns to prompt patterns

### III. A Catalog of Prompt Patterns for Conversational LLMs
- Overview of prompt pattern categories

### Specific Prompt Patterns
#### 1. Meta Language Creation Pattern
#### 2. Output Automater Pattern
#### 3. Flipped Interaction Pattern
#### 4. Persona Pattern


- Act as an X
- Provide outputs that persona X would create

You can have a panel of experts, like a CEO. Act as a CFO. Act as a CTO, Act as a Chief Marketing Officer. Act as a Cybersecurity expert to examine vulnerabilities in my code.

#### 5. Question Refinement Pattern
#### 6. Alternative Approaches Pattern
#### 7. Cognitive Verifier Pattern
#### 8. Fact Check List Pattern
#### 9. Template Pattern
#### 10. Infinite Generation Pattern
#### 11. Visualization Generator Pattern
#### 12. Game Play Pattern
#### 13. Refusal Breaker Pattern
#### 14. Context Control Pattern

### IV. Example Implementations
- Cloud application deployment example

### V. Concluding Remarks

[next](./module2.md) | [top](#patterns) | [course](./readme.md)
