# LLM Workflow Engine (LWE) Shell plugin

Shell plugin for [LLM Workflow Engine](https://github.com/llm-workflow-engine/llm-workflow-engine)

Transform natural language into a shell command, and optionally execute it.

**WARNING: POTENTIALLY DANGEROUS -- YOU ARE RESPONSIBLE FOR VALIDATING THE COMMAND RETURNED BY THE LLM, AND THE OUTCOME OF ITS EXECUTION.**

## Installation

### From packages

Install the latest version of this software directly from github with pip:

```bash
pip install git+https://github.com/llm-workflow-engine/lwe-plugin-shell
```

### From source (recommended for development)

Install the latest version of this software directly from git:

```bash
git clone https://github.com/llm-workflow-engine/lwe-plugin-shell.git
```

Install the development package:

```bash
cd llm-workflow-engine
pip install -e .
```

## Configuration

Add the following to `config.yaml` in your profile:

```yaml
plugins:
  enabled:
    - shell
    # Any other plugins you want enabled...
  # These are the default values.
  shell:
    command:
      confirm: true
    shell:
      path: null
```

## Usage

From a running LWE shell:

```
/shell Print the current working directory
```
