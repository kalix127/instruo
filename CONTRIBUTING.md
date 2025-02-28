# Contributing Guidelines for Instruo

Thank you for your interest in contributing to the **Instruo** project! Your contributions help make this project better for everyone. Please take a moment to read through these guidelines to ensure a smooth collaboration.

## Table of Contents

1. [Getting Started](#getting-started)
2. [Code of Conduct](#code-of-conduct)
3. [How to Contribute](#how-to-contribute)
   - [Reporting Bugs](#reporting-bugs)
   - [Suggesting Enhancements](#suggesting-enhancements)
   - [Adding New Tools](#adding-new-tools)
4. [Project Structure](#project-structure)
5. [Style Guidelines](#style-guidelines)
   - [Coding Standards](#coding-standards)
   - [Tool Documentation Format](#tool-documentation-format)
   - [Commit Messages](#commit-messages)
6. [Documentation Guidelines](#documentation-guidelines)
7. [Testing](#testing)
8. [License](#license)

---

## Getting Started

- **Fork the Repository**: Create a personal fork of the project on GitHub.
- **Clone Your Fork**: Clone your forked repository to your local machine.
- **Create a Branch**: Create a new branch for your contribution (`git checkout -b feature/YourFeatureName`).
- **Install Dependencies**: Run `pnpm install` to install all necessary dependencies.

## Code of Conduct

By participating in this project, you agree to abide by the [Code of Conduct](./CODE_OF_CONDUCT.md), which aims to foster an open and welcoming environment.

## How to Contribute

### Reporting Bugs

If you find a bug, please open an [issue](https://github.com/rahulv-official/instruo/issues) and include:

- A clear and descriptive title.
- Steps to reproduce the issue.
- Expected and actual results.
- Screenshots or code snippets, if applicable.

### Suggesting Enhancements

We welcome suggestions for new features or improvements. Please open an [issue](https://github.com/rahulv-official/instruo/issues) and include:

- A clear and descriptive title.
- A detailed description of the enhancement.
- Any relevant examples or mockups.

### Adding New Tools

We appreciate contributions that add new tools to the platform. Please ensure that:

- The tool is generally useful and aligns with the project's goals.
- You follow the coding and documentation guidelines outlined below.
- You include tests for your tool.

## Project Structure

Understanding the project structure is crucial for effective contribution:

- **Tools Content & Documentation Directory**:
  - Markdown content for tools is stored in `content/tools/<tool-category>/<tool-name>.md`.
- **Components Directory**:
  - Reusable Vue components for tools are stored in `components/content/tools/<tool-category>/<tool-name>/`.
- **Utilities**:
  - Utility scripts and helper functions are stored in the `utils/` directory.

## Style Guidelines

### Coding Standards

- **Language**: Use TypeScript for all code where applicable.
- **Styling**: Use **Tailwind CSS** for consistent styling.
- **Naming Conventions**: Use `PascalCase` for component names and filenames.

### Tool Documentation Format

For Markdown files documenting tools, follow this structure:

1. **Front Matter**

   Include YAML front matter with the title and description of the tool:

   ```yaml
   ---
   title: Tool Title
   description: A brief description of the tool.
   ---
   ```

2. **Tool Implementation**

   Use the tool component to render the tool interface, for example:

   ```markdown
   ::ToolComponentName
   ::
   ```

3. **What is the Tool?**

   Describe what the tool does and its purpose.

4. **Features**

   List the key features of the tool.

   ```markdown
   ## Features

   - **Feature 1**: Description of the feature.
   - **Feature 2**: Description of the feature.
   ```

5. **Use Cases**

   Explain the various scenarios where the tool can be useful.

   ```markdown
   ## Use Cases

   - **Developers**: Encode sensitive data.
   - **General Users**: Decode Base64 strings received online.
   ```

6. **How to Use**

   Provide a step-by-step guide on how to use the tool.

   ```markdown
   ## How to Use

   1. Step 1: Description of the step.
   2. Step 2: Description of the step.
   ```

7. **Example Usage**

   Provide input-output examples for the tool.

   ```markdown
   ## Example Usage

   **Input**: Plain text: `Hello, World!`  
   **Output**: Base64: `SGVsbG8sIFdvcmxkIQ==`
   ```

8. **Error Handling**

   Document error scenarios and how the tool handles them.

   ```markdown
   ## Error Handling

   - **Invalid Input**: Returns a helpful error message.
   ```

9. **Why Use This Tool?**

   Explain why this tool is helpful.

### Commit Messages

- Use the [Conventional Commits](https://www.conventionalcommits.org/) format.
- Begin with a type (`feat`, `fix`, `docs`, etc.) followed by a short description.
- Example: `feat: add Base64 encoding tool`

## Documentation Guidelines

Proper documentation is crucial for users to understand and effectively use the tools and components.

- Use the **Tool Documentation Format** described above for writing documentation in `content/tools/`.

## Testing

- **Unit Tests**: Write unit tests for tools or components if applicable.
- **Cross-Browser Testing**: Ensure compatibility with major browsers.
- **Visual Testing**: Verify the visual appearance of tools and components.

## License

By contributing, you agree that your contributions will be licensed under the [MIT License](https://github.com/rahulv-official/instruo/blob/main/LICENSE).
