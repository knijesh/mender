# mender
Mender is an autonomous software-engineering agent built on Gemma 4 31B (4-bit QAT) that runs fully offline. Given a GitHub issue and a repository, it explores the code, reproduces the bug, edits files, and submits a patch verified by tests.

The repo has three parts:

harness/: a local replica of the competition sandbox, plus the agent config (prompts, skills, budgets)
gym/: trajectory collection and LoRA post-training
eval/: test-based grading, failure analysis, and ablations that separate harness gains from model gains

Built for the [Kaggle Gemma 4 Developer Agent Competition](https://www.kaggle.com/competitions/gemma-4-developer-agent).

Model: [google/gemma-4-31B-it-qat-w4a16-ct](https://huggingface.co/google/gemma-4-31B-it-qat-w4a16-ct)