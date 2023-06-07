## Tree of Thoughts: Deliberate Problem Solving with Large Language Models

This repo provides a simple practical explanation of the paper [Tree of Thoughts: Deliberate Problem Solving with Large Language Models](https://arxiv.org/pdf/2305.10601.pdf). It explores different methods for problem-solving using large language models.

## Problem: Reach the Number 24

The problem is to reach the number 24 using four given digits (4, 9, 10, 13) and basic arithmetic operations (+, -, *, /) by using each number only once.

### Methods Used to Solve the Problem

we have provided an overview of four different methods used to solve the problem.

#### Method 1: Standard Prompt

In this method, a standard prompt is used to provide a few examples and hope that the language model (LLM) can figure out a solution. The prompt includes inputs and corresponding answers. The model is expected to generate a solution based on the given input. However, there is a possibility of incorrect answers due to the model's limitations.

#### Method 2: Few-Shot CoT (Combinations of Two)

This method involves providing intermediate steps to the LLM and asking it to generate accurate intermediate steps and reach the final solution. The prompt includes the initial numbers and a step-by-step process of combining two numbers at each step until reaching the final number.

#### Method 3: Self Consistency

In this method, multiple outputs are generated using the standard prompt, and a majority vote is used to determine the final answer. However, this method may have issues with incorrect intermediate steps due to the parallel generation of tokens by the LLM.

#### Method 4: Tree of Thoughts (ToTs)

This method involves solving the problem in a systematic way, similar to how humans solve problems using a conscious and deliberate thought process. The solution is built in a tree-like structure, starting from the initial numbers and branching out to explore different combinations. Two types of prompts are used: a propose prompt to generate the first depth of the tree and a value prompt to evaluate the remaining depths. By analyzing the generated solutions, the final answer can be determined by considering the most promising paths.

Each method has its own advantages and limitations, and the choice of method depends on the problem and desired outcome.


