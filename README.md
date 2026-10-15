# LLM Prompting Lab

A practical prompt-engineering learning notebook that explores how different prompting strategies influence LLM responses.

The project was cleaned and structured as a portfolio-ready lab rather than a course/week-based notebook. It uses the OpenAI API and keeps credentials outside the repository.

## Techniques Covered

The notebook includes hands-on examples of:

- Zero-shot prompting
- One-shot prompting
- Few-shot prompting
- Role prompting
- Style prompting
- Emotion prompting
- Contextual prompting
- Rephrase-and-Respond (RaR)
- Re-Reading (RE2)
- System prompting
- Self-Ask
- Chain-of-Thought-style prompting
- Step-Back prompting
- Self-Consistency-style prompting
- Thread-of-Thought-style prompting
- Tree-of-Thought-style prompting
- ReAct-style planning

## What This Project Demonstrates

- Prompt design for different task types
- Controlling tone and audience
- Supplying examples and context
- Decomposing complex questions
- Comparing reasoning-oriented prompting patterns
- Calling an LLM through the OpenAI API
- Logging prompts and responses for experimentation
- Handling API credentials without hardcoding secrets

## Repository Structure

```text
llm-prompting-lab/
├── llm_prompting_techniques.ipynb
├── requirements.txt
├── .gitignore
└── README.md
```

## Run the Notebook

Install the dependency:

```bash
pip install -r requirements.txt
```

Then open:

```text
llm_prompting_techniques.ipynb
```

You can provide your API key through the environment:

```bash
OPENAI_API_KEY=your_api_key_here
```

If the environment variable is not set, the notebook prompts for the key securely at runtime.

## Notes on Scope

This project currently uses OpenAI for execution.

Some advanced techniques in the notebook are demonstrated as **prompt patterns**, not as full implementations:

- ReAct does not call a live search or external tool.
- Self-consistency is demonstrated at the prompt level rather than by aggregating many independent model runs.
- Tree-of-thought is demonstrated through structured prompting rather than a separate search algorithm.

The cleaned notebook has cleared outputs and was not freshly executed against the API during the portfolio cleanup.

## Possible Next Improvements

- Add automated prompt evaluation
- Compare multiple models on the same prompt set
- Add structured scoring for quality, relevance, and consistency
- Implement true multi-sample self-consistency
- Build a tool-enabled ReAct agent
- Add experiment summaries and comparison tables

## Author

**Eman Barakat**
