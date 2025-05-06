# Self-discover-agent

Paper https://arxiv.org/pdf/2402.03620

The research paper discusses SELF-DISCOVER, a framework for Large Language Models (LLMs) to self-discover task-intrinsic reasoning structures. Here's a summary of the paper:

**Key Contributions:**

1. **Self-Discovery Process**: SELF-DISCOVER introduces a self-discovery process where LLMs select and compose atomic reasoning modules into a coherent reasoning structure intrinsic to the task.
2. **Improved Performance**: The framework substantially improves the performance of LLMs on challenging reasoning benchmarks, such as BigBench-Hard, grounded agent reasoning, and MATH.
3. **Efficient Computation**: SELF-DISCOVER requires 10-40x fewer inference compute compared to inference-heavy ensemble approaches.

**Key Findings:**

1. **Self-Discovered Reasoning Structures**: The self-discovered reasoning structures are universally applicable across model families and share commonalities with human reasoning patterns.
2. **Comparison to CoT**: SELF-DISCOVER outperforms Chain-of-Thought (CoT) on 21/25 tasks with performance gains up to 42%.
3. **Comparison to Inference-Heavy Methods**: SELF-DISCOVER achieves superior performance against inference-heavy methods while requiring fewer inference compute.

**Analysis:**

1. **Task-Specific Reasoning**: SELF-DISCOVER performs best on tasks requiring world knowledge and has a moderate performance boost on algorithmic tasks compared to CoT.
2. **Error Analysis**: 74.7% model failures on MATH tasks come from computation errors.
3. **Transferability Study**: The self-discovered reasoning structures are transferable across model families, including PaLM 2-L, GPT-4, and Llama-2-70B.

**Conclusion:**

SELF-DISCOVER is a promising framework for improving the performance of LLMs on challenging reasoning tasks. Its self-discovery process allows LLMs to learn task-specific reasoning structures, leading to improved performance and efficient computation.

---

SELF-DISCOVER guides LLMs to self-discover and compose atomic reasoning modules into a reasoning structure to solve challenging tasks.
![image](https://github.com/user-attachments/assets/7e241b0f-ec2b-4d41-aa26-f3b386bd9750)

Given a generative LM, task, and seed reasoning module descriptions, we guide LMs to generate a reasoning structure in key-value format to solve the task. Finally, models can follow the self-discovered structures to solve the every instance from the task by filling in the values in JSON step-by-step.
![image](https://github.com/user-attachments/assets/8e97b299-7a2a-443b-bbed-546baa7b7a29)

## Experimental setup
We use LMs to compose a coherent reasoning structure by selecting relevant modules, adapting to task-specific descriptions, and implement a reasoning structure in JSON.
![image](https://github.com/user-attachments/assets/53c3ff4c-63b8-4b45-b7d8-5e36b9fc1f7a)


