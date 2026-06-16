# A Guide to Large Language Model Systems

*Inference, hardware, retrieval, agents, and safety.*
By Aditya Kamat

This is a guide to how large language model systems actually work, from a single forward pass up to a full production system with retrieval, agents, and the safety problems that come with them.

It started as my own notes. I spent about a year learning this, and the explanations I needed were scattered across papers, talks, and docs. I put the whole picture in one place, in order, so you don't have to assemble it yourself the way I did.

**[Read A Guide to Large Language Model Systems](./A%20Guide%20to%20Large%20Language%20Model%20Systems%20-%20Inference%2C%20hardware%2C%20retrieval%2C%20agents%2C%20and%20safety%20-%20Aditya%20Kamat.pdf)** (PDF)

## How it's built

It follows one ordinary chat request all the way down the stack. Each part wraps another layer around that request: the model, the work that makes it fast, the hardware, serving at scale, retrieval, agents, and finally safety. Every topic opens with the problem it solves, gives a rough mental model before the precise one, and keeps real numbers next to the context they came from. Anything deeper than a first read needs is marked, so you can skip it and come back later.

## Who it's for

You can write code and you understand the basics like memory and latency. You do not need a machine learning background. Where one helps, the chapter builds it before it relies on it.

## What's inside

- Part I. The model: what a forward pass computes, and what it costs
- Part II. Inference: making one model fast, with the KV cache, batching, quantisation, and speculative decoding
- Part III. The hardware: the GPU and the memory limits underneath everything
- Part IV. Serving: many requests sharing the hardware at a latency target
- Part V. Knowledge: retrieval, embeddings, and search
- Part VI. Agency: tools, the agent loop, and the action boundary
- Part VII. The system: design, optimisation, profiling, and operations
- Part VIII. Safety and alignment: how models go wrong, and how to oversee them

Appendices: beyond text, a glossary, and further reading.

## How to read it

Read it in order the first time. The layers build on each other, so a later chapter assumes the mental model an earlier one gave you. Once you have the whole picture, the chapters stand on their own as a reference.

## Feedback

If something is wrong or unclear, please open an issue. Corrections are welcome.

## License

The text is released under CC BY 4.0, so you are free to share and adapt it with attribution.
