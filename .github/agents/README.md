# GitHub Copilot Custom Agents

## Overview

This directory contains configuration files for GitHub Copilot Custom Agents. Custom agents are specialized AI assistants that can be configured to help with specific tasks in your repository.

## What is `my-agent.agent.md`?

The `my-agent.agent.md` file is a **configuration template** for creating a GitHub Copilot Custom Agent. This file defines:

### Purpose
Custom agents extend GitHub Copilot's capabilities by creating specialized assistants tailored to your repository's specific needs. They can help with:
- Code reviews specific to your coding standards
- Domain-specific code generation
- Repository-specific documentation
- Custom workflows and automations

### File Structure

The file follows a specific format required by GitHub Copilot:

1. **YAML Front Matter** (Lines 1-9):
   ```yaml
   ---
   name:           # The name of your custom agent
   description:    # A brief description of what the agent does
   ---
   ```
   This section contains metadata about the agent that GitHub Copilot uses to identify and describe it.

2. **Agent Instructions** (Lines 11-14):
   ```markdown
   # My Agent
   
   Describe what your agent does here...
   ```
   This section contains the actual instructions that tell the agent how to behave and what tasks it should help with.

### Current Status

The file is currently a **template** with placeholder values:
- `name:` - Empty, needs to be filled with the agent's name
- `description:` - Empty, needs to be filled with a brief description
- Instructions section - Contains placeholder text that needs to be replaced with actual agent instructions

### How to Use

To create a functional custom agent:

1. **Fill in the metadata:**
   - Set a meaningful `name` for your agent (e.g., "code-reviewer", "doc-writer")
   - Add a clear `description` explaining the agent's purpose

2. **Write agent instructions:**
   - Replace the placeholder text with detailed instructions
   - Define the agent's expertise area
   - Specify what tasks it should help with
   - Include any repository-specific guidelines

3. **Test locally:**
   - Use the Copilot CLI for local testing: https://gh.io/customagents/cli
   
4. **Deploy:**
   - Merge the completed file into the default repository branch
   - The agent will become available to repository collaborators

### Example

Here's what a completed agent might look like:

```yaml
---
name: latex-helper
description: Assists with LaTeX document editing and compilation issues in Overleaf
---

# LaTeX Helper Agent

I am a specialized agent for helping with LaTeX-related tasks in the Overleaf codebase.

My expertise includes:
- LaTeX syntax and compilation errors
- Document structure and best practices
- Troubleshooting compilation issues
- Package recommendations and usage

When helping with LaTeX code, I will:
1. Identify common LaTeX errors and suggest fixes
2. Recommend appropriate packages for specific needs
3. Follow Overleaf's coding standards and conventions
4. Provide examples relevant to the Overleaf platform
```

## References

- Custom Agents Format Documentation: https://gh.io/customagents/config
- Copilot CLI for Testing: https://gh.io/customagents/cli

## Summary

**What is this file doing?**

The `my-agent.agent.md` file is a **configuration template for GitHub Copilot Custom Agents**. It serves as a starting point for creating specialized AI assistants that can help developers with repository-specific tasks. Currently, it's incomplete and requires configuration with:
- A unique name
- A descriptive description
- Detailed instructions for the agent's behavior

Once properly configured and merged into the default branch, it will create a custom Copilot agent that repository collaborators can use for specialized assistance.
