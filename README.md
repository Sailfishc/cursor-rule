# Cursor Rule / Cursor 规则

(English) A project for managing and applying custom rules within the Cursor IDE and other AI-assisted development environments.
(中文) 一个用于在 Cursor IDE 和其他 AI 辅助开发环境中管理和应用自定义规则的项目。

## Overview / 概述

(English) This repository contains a collection of rule definitions designed to guide AI assistants. These rules help enforce project-specific conventions, streamline workflows, and ensure adherence to best practices, ultimately improving the quality and consistency of AI-generated code and responses.
(中文) 本代码库包含一系列规则定义，旨在指导 AI 助手。这些规则有助于强制执行项目特定的约定，简化工作流程，并确保遵守最佳实践，最终提高 AI 生成的代码和响应的质量与一致性。

## Structure / 结构

(English) The rules are organized into top-level folders, each representing a distinct category or operational domain. This structure allows for easy navigation and selection of relevant rule sets.
(中文) 规则按顶级文件夹进行组织，每个文件夹代表一个独特的类别或操作领域。这种结构便于导航和选择相关的规则集。

- `isolation_rules/` - Contains various rule categories: /包含各类规则：
  - `Core/` - Fundamental operational rules for the AI assistant. / AI 助手的基础操作规则。
  - `Level1-4/` - Task-specific workflows organized by complexity, from quick bug fixes (Level 1) to complex system design (Level 4). / 按复杂度组织的任务特定工作流程，从快速错误修复（1级）到复杂系统设计（4级）。
  - `Phases/` - Guidelines for different phases of a task, such as planning, creative design, and implementation. / 任务不同阶段的指南，例如规划、创意设计和实施。
  - `visual-maps/` - Visual process maps to illustrate workflows and decision-making processes. / 可视化流程图，用于说明工作流程和决策过程。
- `README.md` - This file, providing an overview of the project. / 本文件，提供项目概述。

## Design Philosophy / 设计思路

(English)
Inspired by concepts for guiding AI behavior (similar to those outlined in [Cursor's documentation on Rules](https://docs.cursor.com/context/rules)), this project aims to provide a clear, structured, and adaptable way to manage AI instructions. The rules are designed to be:

- **Modular & Organized by Folder:** Rules are grouped into thematic folders. This makes it easy to find, understand, and select specific sets of instructions relevant to a particular task or domain. You can pick and choose folders or individual rules as needed.
- **Portable:** The rules are intended to be easily copied and integrated into different projects.
- **Actionable:** Rules provide concrete guidance that AI assistants can use to improve their behavior, code generation, and analytical processes.
- **Evolvable:** The structure allows for new rules and categories to be added as best practices and project needs evolve.

(中文)
本项目的设计思路借鉴了指导 AI 行为的理念（类似于 [Cursor 规则文档](https://docs.cursor.com/context/rules) 中概述的原则），旨在提供一种清晰、结构化且适应性强的方式来管理 AI指令。这些规则的设计具有以下特点：

- **模块化与按文件夹组织：** 规则被归类到主题文件夹中。这使得查找、理解和选择与特定任务或领域相关的特定指令集变得容易。您可以根据需要挑选文件夹或单个规则。
- **便携性：** 规则旨在方便地复制并集成到不同的项目中。
- **可操作性：** 规则提供具体的指导，AI 助手可以用它来改进其行为、代码生成和分析过程。
- **可进化性：** 该结构允许随着最佳实践和项目需求的发展添加新的规则和类别。

## Usage / 使用方式

(English)

1.  **Browse & Select:** Navigate the `isolation_rules/` directory and its subfolders to find the rules relevant to your current needs.
2.  **Download/Clone:** Download or clone this repository to your local machine.
3.  **Integrate into Your Project:**
    *   **For Cursor IDE Users:** Cursor uses a `.cursor/rules/` directory at the root of your project for project-specific rules (refer to [Cursor Project Rules documentation](https://docs.cursor.com/context/rules#project-rules)). You can copy the desired rule files (e.g., `.md` or `.mdc` files if you adapt them) from this repository into your project's `.cursor/rules/` directory. You might need to adjust the file format or structure slightly to match Cursor's expected MDC (Markdown with Components) format for full functionality like auto-attachment based on globs or agent-requested loading.
    *   **For Other AI Environments:** Copy the relevant rule files or their content into the system or prompt configuration area of your specific AI tool or platform.
4.  **Reference & Apply:** Instruct your AI assistant to consider the rules you've integrated. For Cursor, rules in `.cursor/rules/` can be automatically applied or manually invoked depending on their configuration.

(中文)

1.  **浏览与选择：** 浏览 `isolation_rules/` 目录及其子文件夹，找到与您当前需求相关的规则。
2.  **下载/克隆：** 将此代码库下载或克隆到您的本地计算机。
3.  **集成到您的项目中：**
    *   **对于 Cursor IDE 用户：** Cursor 在项目根目录中使用 `.cursor/rules/` 目录来存放项目特定规则（请参阅 [Cursor 项目规则文档](https://docs.cursor.com/context/rules#project-rules)）。您可以将本代码库中所需的规则文件（例如 `.md` 文件，或者如果您对其进行调整以适应 `.mdc` 格式）复制到您项目的 `.cursor/rules/` 目录中。您可能需要稍微调整文件格式或结构，以匹配 Cursor 期望的 MDC (Markdown with Components) 格式，从而实现诸如基于 glob 模式自动附加或 AI 代理请求加载等全部功能。
    *   **对于其他 AI 环境：** 将相关的规则文件或其内容复制到您特定 AI 工具或平台的系统或提示配置区域。
4.  **参考与应用：** 指示您的 AI 助手遵循您已集成的规则。对于 Cursor，`.cursor/rules/` 中的规则可以根据其配置自动应用或手动调用。

## Getting Started / 开始使用

[Add installation and usage instructions here]

## Contributing / 贡献指南

[Add contribution guidelines here]

## License / 许可证

[Add license information here] 