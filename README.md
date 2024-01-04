# Local mac llm

The goal here is to get Mixtral 8x7b mixture of experts model running locally on a mac laptop. We will follow the blog post [here](https://blog.llamaindex.ai/running-mixtral-8x7-locally-with-llamaindex-e6cebeabe0ab).

We will be using [ollama](https://github.com/jmorganca/ollama), which is a tool that greatly simplifies running LLMs locally.

- Step 1: Install Ollama [here](https://ollama.ai/).

Next we will download a model. The full library of available models can be found [here](https://ollama.ai/library).
- Step 2a: Run `ollama run llama2`
- Step 2b: Run `ollama run mixtral` (this requires 48GB of RAM to run smoothly!)
- Step 2c: Run `ollama run mistral`

- Step 3: Use LlamaIndex to build a retrieval-augmented generation (RAG) framework so that our LLM is able to leverage our custom dataset 