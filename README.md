# Artificial Intelligence Notation (AIN)

The **AIN** file format is a lightweight, human-readable format designed for storing instructions, prompts, and pseudo-code that guide AI models in performing tasks. It is optimized for clarity, simplicity, and versatility, making it easy for both humans and machines to interpret and use.

## Key Features

- **Human-Readable**: The format uses simple and minimal syntax, making it easy for both humans and AI systems to write, read, and edit.
- **Versatile**: Suitable for a variety of AI tasks such as code generation, problem-solving, and data processing.
- **Multiple Format Support**: Can be saved as plain text (.txt), Markdown (.md), YAML (.yaml), or JSON (.json) for easy integration with different tools.

## Structure

Each **AIN** file consists of:
- **Instructions/Prompts**: Concise tasks or instructions for the AI, with examples when applicable.
- **Data**: Input-output pairs or sample data that help AI understand the tasks.
- **Context**: Information specific to the project or environment that provides context to AI instructions for more accurate results.

### Example AIN File:

```ain
# Manifest Instructions for AI Task

## Overview:
This repository contains TypeScript code that interacts with Azure Blob Storage and processes YAML data.

## Specific Instructions:
- Always use the `@azure/storage-blob` package for Blob Storage.
- Use `js-yaml` for parsing and writing YAML data.
- JavaScript code should follow the convention of double quotes for strings and tabs for indentation.

## Example Task:
1. Upload a file to Azure Blob Storage using the `uploadFile()` method.
2. Parse a YAML file to extract user data and process it.
```

## Supported Formats

The **AIN** file format can be written in different formats, including:
- **YAML**: For structured data with clear key-value pairs.
- **Markdown (MD)**: Ideal for documentation-style instructions and easy readability.
- **Text (TXT)**: Simple, unformatted instructions.
- **JSON**: Machine-readable format for AI to process directly.

### Example Formats

#### YAML Example:

```yaml
task: "Upload file to Azure Blob Storage"
container_name: "user-files"
file_path: "/path/to/file.txt"
```

#### Markdown Example:

```markdown
# Task Description

Upload a file to Azure Blob Storage using `@azure/storage-blob`.

## Requirements:
- **Container Name**: user-files
- **File Path**: /path/to/file.txt
```

#### JSON Example:

```json
{
  "task": "Upload file to Azure Blob Storage",
  "container_name": "user-files",
  "file_path": "/path/to/file.txt"
}
```

## How It Works

1. **Organize AI Tasks**: Use **AIN** files to define task-specific instructions for the AI.
2. **Hierarchical Organization**: Store **AIN** files in a structured folder system. Lower-level files can inherit or override instructions from higher-level files, providing flexibility for project-specific tasks.

### Example Folder Structure:

```
/.github
  └── /copilot-instructions.md   <- General instructions for Copilot
/root
  ├── /manifest.ain              <- General manifest for AI tasks
  └── /project-specific.ain      <- Custom instructions for project-specific tasks
/scripts
  └── /scripts.ain               <- Instructions for scripting tasks
/docs
  └── /docs.ain                  <- Documentation creation guidelines
/examples
  └── /examples.ain              <- Example generation guidelines
```

## Benefits of Using AIN Files

- **Improved AI Efficiency**: Clear, structured context allows AI to generate more accurate and relevant responses.
- **Easy Collaboration**: Provides clarity and consistency, making team collaboration more efficient.
- **Scalability**: The format adapts well to both small and large projects, offering flexibility in complexity and task detail.

## Best Practices

- **Keep instructions clear and concise**: Simplicity helps AI perform better.
- **Avoid conflicting instructions**: Ensure that **AIN** files do not contradict each other to prevent confusion.
- **Modular Structure**: Break down large tasks into smaller, manageable instructions for easier AI processing.

## Getting Started

1. Create a new **AIN** file in your repository (e.g., `manifest.ain`).
2. Define the tasks, instructions, or prompts you want to provide to the AI.
3. Choose your preferred format (YAML, Markdown, JSON, or TXT).
4. Integrate the **AIN** files with your AI-powered tools (e.g., GitHub Copilot, OpenAI).
5. Use **AIN** files to ensure consistent, context-aware responses from AI models.

## Conclusion

The **AIN** file format is a simple yet powerful way to structure instructions and data for AI-driven projects. It supports multiple formats (YAML, Markdown, JSON) and provides organized, scalable, and context-driven interactions that enhance AI workflows.

---
## Fun Fact

The **AIN** format is like COBOL for the age of AI—timeless, yet modern, and built to adapt to the needs of the future! It combines the simplicity and clarity of classic formats with the power and flexibility required for working with AI agents.

## Purpose

The ultimate goal of the **AIN** format is to create a framework for working with AI agents like **GitHub Copilot** to guide and enhance project development. This format enables seamless collaboration between humans and AI, improving workflows, productivity, and results.

## TODO

### Research
 
 - [Model-Driven Engineering + DSL for AI](https://arxiv.org/abs/2307.04599?utm_source=chatgpt.com)  
   Przegląd systematyczny użycia metajęzyków w inżynierii oprogramowania AI – głównie w fazach modelowania i treningu.
 
 - [RAFT: Retrieval-Augmented Fine Tuning](https://medium.com/%40zbabar/unlocking-domain-specific-expertise-in-large-language-models-with-raft-5a96bfdf21d6?utm_source=chatgpt.com)  
   Strategia łączenia podejścia RAG z dostosowaniem do domenowych danych dla LLM.
 
 - [GitHub Copilot Agent Mode](https://code.visualstudio.com/blogs/2025/02/24/introducing-copilot-agent-mode?utm_source=chatgpt.com)  
   Nowy tryb działania Copilota jako agenta wykonującego polecenia użytkownika w IDE.
 
 - [Claude 3.5 Sonnet Agents in IDE](https://codegpt.co/agents/claude-sonnet?utm_source=chatgpt.com)  
   Integracja agentów Claude Sonnet w IDE do wykonywania zadań projektowych z własną bazą kodu.
 
 - [LLM Multi-Agent Analysis of Requirements](https://arxiv.org/abs/2409.00038?utm_source=chatgpt.com)  
   Badania nad analizą wymagań projektowych przez zespoły agentów AI, np. GPT i Mixtral.
 
 - [Model Context Protocol (MCP)](https://en.wikipedia.org/wiki/Model_Context_Protocol?utm_source=chatgpt.com)  
   Otwarty standard do integracji LLM z zewnętrznymi narzędziami i danymi przez spójny interfejs.
 
 - [Data Format Description Language (DFDL)](https://en.wikipedia.org/wiki/Data_Format_Description_Language?utm_source=chatgpt.com)  
   ISO standard do definiowania struktury danych tekstowych/binarnych w sposób zrozumiały dla AI.
 
 - [AutomationML](https://en.wikipedia.org/wiki/AutomationML?utm_source=chatgpt.com)  
   Format wymiany danych inżynierii oparty na XML, do opisu geometrii, topologii, logiki i więcej.

