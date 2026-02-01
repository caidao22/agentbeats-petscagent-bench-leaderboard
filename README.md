# AgentBeats PetscAgent Benchmark Leaderboard

A benchmarking framework for evaluating AI agents against the PetscAgent benchmark suite.

## Quick Start

### Running the Benchmark

1. Go to **Actions** → **Run Benchmark** → **Run workflow**
2. Select a configuration:
   - **gemini3** – Run with Gemini 3 Flash Preview
   - **gpt52** – Run with GPT-5.2 (via AskSage)
   - **all** – Run both configurations in parallel

> **⚠️ Warning:** Each benchmark run consumes a significant amount of LLM tokens. Monitor your API usage and costs accordingly.

### Reproducibility

Individual runs exhibit noticeable run-to-run variation. Extensive experiments indicate that this variability arises from inherent limitations of current LLMs.
Even with the temperature set to 0, the same model still generates different code for identical prompts. In addition, some models, such as Gemini, suffer from stability issues and are frequently overloaded, further impacting reproducibility.

### Required Docker Images

The benchmark uses the following Docker images from GitHub Container Registry:

- ghcr.io/caidao22/petscagent-bench-green-agent:latest
- ghcr.io/caidao22/petscagent-bench-purple-agent:latest
- ghcr.io/caidao22/petscagent-bench-petsc-mcp-servers:latest
- ghcr.io/caidao22/petscagent-bench-client-cli:latest

## Submitting Results

After a successful benchmark run:

1. The workflow creates a submission branch automatically
2. Click the PR link in the workflow summary
3. **Important:** Uncheck "Allow edits and access to secrets by maintainers" when creating the PR
