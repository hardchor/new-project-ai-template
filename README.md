# New Project Setup Walkthrough

This repository provides a structured walkthrough for initializing new software projects from scratch. It contains a series of documents and prompts designed to help you define project context, establish user flows, make technology stack decisions, and set best practices before outlining a phased development plan.

---

## How It Works

The core of this repository is the `_docs/resources/new-project-setup.md` file. This document provides a detailed sequence of steps and prompts to guide you through the initial phases of project setup.

Following the steps in `new-project-setup.md` will help you:

1.  **Define Project Scope:** Start with a high-level project overview to establish goals and context.
2.  **Create Foundational Documents:** Systematically generate key documents for user flows, technology stack, UI/theme rules, and project conventions.
3.  **Establish Best Practices:** Implement standards for folder structure, coding style, and development workflows.
4.  **Plan Development Phases:** Outline a clear, iterative plan for building your application from a barebones setup to a polished product.

By following this guide, you can quickly bootstrap a well-organized and robust foundation for your project, ensuring a consistent and clear approach for all contributors.

---

## Quick Start with Task Master

This template includes Task Master for AI-driven task management. Here's how to get started:

1. **Initialize Task Master** (already done if you cloned this template):
   ```
   task-master init
   ```

2. **Discuss your idea with AI and ask for a PRD** using `example_prd.txt`, and save it to `scripts/PRD.txt`

3. **Ask GitHub Copilot** (or run CLI) to parse your PRD and generate initial tasks:
   - **MCP Tool:** `parse_prd` | **CLI:** `task-master parse-prd scripts/prd.txt`

4. **Ask GitHub Copilot to analyze the complexity** of the tasks in your PRD using research:
   - **MCP Tool:** `analyze_project_complexity` | **CLI:** `task-master analyze-complexity`

5. **Ask GitHub Copilot to expand all of your tasks** using the complexity analysis

6. **Ask GitHub Copilot to begin working on the next task**

7. **Add new tasks anytime** using the add-task command or MCP tool

8. **Ask GitHub Copilot to set the status** of one or many tasks/subtasks at a time. Use the task id from the task lists.

9. **Ask GitHub Copilot to update all tasks** from a specific task id based on new learnings or pivots in your project.

10. **Ship it!**

---

To get started, open and follow the instructions in `_docs/resources/new-project-setup.md`.

Happy building!
