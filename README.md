# AgentBeats PetscAgent Benchmark Leaderboard

A benchmarking framework for evaluating AI agents against the PetscAgent benchmark suite.

## Quick Start

### Running the Benchmark

1. Go to **Actions** → **Run Benchmark** → **Run workflow**
2. Select a configuration:
   - **gemini3** – Run with Gemini 3 Flash Preview
   - **gpt52** – Run with GPT-5.2 (via AskSage)
   - **all** – Run both configurations in parallel

## Submitting Results

After a successful benchmark run:

1. The workflow creates a submission branch automatically
2. Click the PR link in the workflow summary
3. **Important:** Uncheck "Allow edits and access to secrets by maintainers" when creating the PR
