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
