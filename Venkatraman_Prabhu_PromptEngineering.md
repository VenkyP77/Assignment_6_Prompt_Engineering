# Prompt Engineering Portfolio
Name: Venkatraman Prabhu
Date: 
LLM Used: Gemini Pro

## Part 1: Prompt Design & Iteration
### 1.1 Scenario A: Technical Explanation
| Version | Prompt | What Changed | Why This Improved the Output|
|:-------:|:-------|:-------------|:----------------------------|
| V1 | Explain a complex concept like "Neural Networks" in a simple manner, as you would to a 10-year old | N/A | N/A |
| V2 | You are an experienced teacher with a rich experience in communicating effectively with 10-year old students. Explain the concept of "Neural Networks" in a simple manner with real-world examples. | A role was assigned to the LLM. Explicitly instructed to provide real-world examples | The LLM was not making any assumptions as to its role in the conversation. Also, it was clearly instructed to provide real-world examples in a simple manner to augment its explanation |
| V3 | <ROLE> You are a senior science teacher with a rich experience in effectively communicating with 10-year old students </ROLE>
<CONTEXT> You are communicating with 10-year old STEM students who are curious and want to explore the world of Machine Learning and Data Science. As a teacher it is your job to spark a desire in them for learning more about this by making the explanation interesting, yet easy to understand
</CONTEXT>
<TASK> You need to explain effectively the concepts of Neural Networks with real-world analogies </TASK>
<CONSTRAINTS> (Mandatory)
The explanation must contain the following:
1. Real-world analogies (not more than 3)
2. Visual representations in the form of infographics or mind-maps
3. Examples (not more than 3) of Neural Networks in action, in the real-world
4. Minimal use of technical jargon. Wherever, it is important to use jargon, make sure that it is explained in a simple manner.
</CONSTRAINTS>
<OUTPUT>
Output your response as a professional-grade structured word document which contains the following:
1. Summary / Overview
2. Detailed explanation with visuals and examples
3. Real-world implementation use cases
4. A high-level structured learning path to learn more about this concept
5. Additional sources to refer for a further deep-dive into this concept
</OUTPUT> | Used an XML tag based structured prompt. Provide role, context, task, constraints and output requirements explicitly. | A structured XML tagged prompt ensured that nothing was left ambiguous and the LLM had precise instructions. Also providing a context allowed the LLM to choose the appropriate tone and level of content for the output. Constraints and output requirements kept is focused and allowed it to generate a very high-quality output that could be shared as a word / pdf document, as-is. |

### 1.1 Scenario B: Professional Email
| Version | Prompt | What Changed | Why This Improved the Output|
|:-------:|:-------|:-------------|:----------------------------|
| V1 | [Your initial prompt] | N/A	N/A |
| V2 | [Your refined prompt] | [Specific changes made] | [Explanation] |
| V3 | [Your final prompt] | [Specific changes made] | [Explanation] |

### 1.1 Scenario C: Creative Content
| Version | Prompt | What Changed | Why This Improved the Output|
|:-------:|:-------|:-------------|:----------------------------|
| V1 | [Your initial prompt] | N/A	N/A |
| V2 | [Your refined prompt] | [Specific changes made] | [Explanation] |
| V3 | [Your final prompt] | [Specific changes made] | [Explanation] |

### 1.2 Iteration Documentation
### 1.3 Role and Context Analysis

## Part 2: Temperature & Parameter Control
### 2.1 Temperature Experimentation
### 2.2 Analysis & Recommendations

## Part 3: Strategic Prompting Techniques
### 3.1 Chain-of-Thought Prompting
### 3.2 Few-Shot Prompting

## Part 4: Responsible AI & Limitations
### 4.1 Testing for Hallucinations
### 4.2 Testing for Bias
### 4.3 Limitations & Responsible Use