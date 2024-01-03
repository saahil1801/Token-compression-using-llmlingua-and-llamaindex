# Token-compression-using-llmlingua-and-llamaindex

LLMLingua utilizes a compact, well-trained language model (e.g., GPT2-small, LLaMA-7B) to identify and remove non-essential tokens in prompts. This approach enables efficient inference with large language models (LLMs), achieving up to 20x compression with minimal performance loss.LongLLMLingua mitigates the 'lost in the middle' issue in LLMs, enhancing long-context information processing. It reduces costs and boosts efficiency with prompt compression, improving RAG performance by up to 21.4% using only 1/4 of the tokens.

💰 Cost Savings: Reduces both prompt and generation lengths.

📝 Extended Context Support: Enhances support for longer contexts, mitigates the "lost in the middle" issue, and boosts overall performance.

⚖️ Robustness: No additional training needed for LLMs.

🕵️ Knowledge Retention: Maintains original prompt information like ICL and reasoning.

📜 KV-Cache Compression: Accelerates inference process.

🪃 Comprehensive Recovery: GPT-4 can recover all key information from compressed prompts.


LlamaIndex is a widely used RAG framework. LLMLingua and LongLLMLingua have also been incorporated into the LlamaIndex pipeline, which allows for more convenient use of LLMLingua-related technologies in RAG scenarios.More specifically, LongLLMLinguaPostprocessor can be used as a Postprocessor in LlamaIndex by invoking it, with arguments consistent with those in the PromptCompressor of LLMLingua. You can call the corresponding compression algorithms in LLMLingua and the question-aware prompt compression method in LongLLMLingua.
