## Below is a recommended order for creating these documents so each naturally builds upon the previous. This sequence ensures we first set the project context (overview, user flow, tech decisions), then define our rules (tech stack, UI, theme, code organization), and finally outline our phased approach and detailed workflows.

1. @project-overview.md
   - Establish overall project purpose, scope, and goals.

2. @user-flow.md
   - Clarify how users will interact with the application (registration, navigation, messaging flows).

3. @tech-stack.md
   - Describe the core technologies used (Node, Next.js, TypeScript, etc.) and their roles.

4. @ui-rules.md
   - Define visual and interaction guidelines for building components (including accessibility and design principles).

5. @theme-rules.md
   - Establish theming foundations (colors, typography, animations) to be incorporated into UI development.

6. @codebase-best-practices.md  
   - Outline folder structure, file naming conventions, and Next.js App Router practices.

7. ./checklists/
   - Outline the different phases of the project, and the different tasks and features we'll need to complete in order to complete our goal. Each feature (or group of features) should have its own phase document.


## Below are recommended steps/prompts for creating these files from scratch, with only the project overview to guide you.

1. 
```
Use @project-overview.md to create a document called `user-flow.md`, which should define the user journey through different segments of the application.

The user journey should take into account the different features the app has & how they are connected to one-another. This document will later serve as a guide for building out our project architecture and UI elements.

Ask clarifying questions if needed-- we don't want any embellishments or assumptions.
```


2. NOTE: if you have any stack preferences, mention them here.
```
Use @project-overview.md and @user-flow.md to make recommendations for our stack. I already know I want to use ___, ___, and ___ (e.g. TypeScript, React, Tailwind).

For each anticipated part of our stack, propose and describe an industry standard and a popular alternative. We will work through the list together to determine what we'll use for the project.
```


3. USER ACTION: Look through the proposed stack and think about what you want to pick. For ones you're unsure of, ask about pros/cons, see what's most compatible with the rest of the stack, etc. When you're done, output the results in a markdown file called `tech-stack.md`.


4. 
```
Update @tech-stack.md to cover all best-practices, limitations, and conventions for using the selected technologies. It should be thorough, and include important considerations and common pitfalls for each technology.
```


5. NOTE: If you don't know much about UI, UX, design, or theming, this is a great opportunity to learn.
```
I want to learn more about common design principles, and how they might be applied to our project.
Give me a list of 15 possible themes (e.g. "minimalist", "retro", "futuristic", "glassmorphic", etc), with a description of each one.
Observe @project-overview.md and @user-flow.md for context about the project to guide your recommendations.
```


6. NOTE: Edit the blank spaces in the prompt to suit your desires for the project.
```
I want my project to be ____ (mobile-first, responsive, animated, etc). We need to define the visual and interaction guidelines for building components (including accessibility and design principles), as well as any tie-ins with the tech stack (consider our backend, for example).

Also, I have decided I want my theme to be ____ (minimalist, retro, futuristic, glassmorphic, etc).

Use @user-flow.md and @tech-stack.md to put together two new files, called `ui-rules.md` and `theme-rules.md`.
```


7. 
```
We need to define our project's folder structure, file naming conventions, and any other rules we need to follow.

We are building an AI-first codebase, which means it needs to be modular, scalable, and easy to understand. The file structure should be highly navigable, and the code should be well-organized and easy to read.

All files should have an explanation of their contents at the top, and all functions should have proper commentation of their purpose and parameters (JSDoc, TSDoc, etc, whatever is appropriate).
To maintain readability by Cursor's AI tools, files should not exceed 250 lines.

Use @tech-stack.md, @ui-rules.md, and @theme-rules.md to put together a new file called `codebase-best-practices.md`. This document should also include a file tree demonstrating the proper separation of concerns given our project's expected structure.
```


8. 
```
We need to define the different tasks and features we'll need to complete in order to build our project.

Create a phased approach to building the application, and define the different tasks and features we'll need to complete in order to complete our goal.

Rules to follow:
- Each phase should have its own document
- Each phase should be specific to a feature, or a group of closely-related features
- Each feature should have a checklist of actionable steps, clearly specifying which steps are frontend and which are backend (frontend first, backend second)
- Some tasks will be more complex than others, and will require more steps to complete. Don't be afraid to break down a task into multiple steps-- the checklist can be as long as you want.
- Create as many phases as you deem appropriate, as long as they are specific.

Use @project-overview.md , @user-flow.md , @tech-stack.md , @ui-rules.md , @theme-rules.md , and @codebase-best-practices.md to put together each of these new files.
```


9. 
```
Please also create a `phase-0-setup.md` file, which will be a checklist of the initial setup of the project, including installing dependencies, setting up dev tools, and configuring the environment.
```


10. (OPTIONAL)
```
For each of the files attached, within each one, flatten its lists into a single list of actionable steps. Format each checklist item with "[ ]" to denote empty completions status. Also, follow the bracket with either "FRONTEND: " or "BACKEND: ", based on the nature of the task.
```


11. USER ACTION: Make a brief Agent Rules document, which will be a list of rules for the agent to follow. Recommended to use Cursor Rules, or Cursor Notepads.
```
This is an AI-first codebase. It needs to be modular, scalable, and easy to understand. The file structure should be highly navigable, and the code should be well-organized and easy to read.

All files should have an explanation of their contents at the top, and all functions should have proper commentation of their purpose and parameters (JSDoc, TSDoc, etc, whatever is appropriate).
To maintain readability by Cursor's AI tools, files should not exceed 250 lines.

# Rules for AI Agents

- ALWAYS validate any changes to the codebase against @codebase-best-practices.md
- ...
```

12. USER ACTION: Make sure all these docs are in the right place. You want them all under the `docs` folder-- if you want even more organization, create subfolders. I like to put all the docs from these steps in the docs/rules folder.

13. ATTACH: `Agent Rules`, `phase-0-setup.md` (current phase doc), `tech-stack.md`, and `codebase-best-practices.md` (just good to always have in context)
```
Let's get started on our project.
```
