## Standards You Must Follow When Working on This Repository

### All Code/Projects

### Testing
Add test coverage for all functions/code. Ideally in a Test Driven Development manner - i.e., defining tests based on the specification for the feature you're about to implement, then implement the feature and make sure the test passes. Please ensure we have 90% test coverage of all code.

### A quick gut-check: **“Will I care if this fails?”**


### Python Code
- Follow Python best practices
- Utilize Python 3.12
- Follow PEP 8 

### PHP Code
- Follow PHP best practices
- Follow PSR-12

### Bash Scripts

### Documentation
- The docs folder contains important documentation. 
- Please keep documentation written for users and human developers in docs/humans/
- Please keep documentation written for LLMs in docs/ai/

### Progress Files
- Create individual progress files in the docs/progress/ directory after completing work, following the below format. Use today's actual UTC date and time in the filename.
- Use individual progress files to record changes, which are then compiled into progress.md. This system prevents merge conflicts and maintains a clear development history.

#### When to Create a Progress File
- Read the current progress.md before starting work to avoid duplicate efforts
- After completing a task, bug fix, or feature, create a new progress file
- Use today's UTC date and current time in the filename

File Naming Convention

Format: YYYY-MM-DD-HH-MM-SS-brief-description.md
Example: 2025-06-29-14-30-00-fix-node-exporter-error.md

File Content Format

### YYYY-MM-DD - Short description of the change
- **Issue**: Brief description of the problem (if applicable)
- **Root cause**: Why the issue occurred (if applicable)
- **Fix**: What was done to resolve it
- **Files changed**: List of modified files
- **Result**: The outcome of the change
Example Progress File

File: progress/2025-07-01-10-15-00-add-progress-system.md

### 2025-07-01 - Implemented individual progress file system
- **Issue**: Frequent merge conflicts in progress.md when multiple PRs modify it
- **Root cause**: All contributors editing the same file simultaneously
- **Fix**: Created individual progress files that compile into progress.md
- **Files changed**: 
  - `progress/` directory structure
  - `docs/progress-guide.md`
  - `scripts/compile_progress.py`
  - `AGENTS.md`
- **Result**: Contributors can record progress without merge conflicts

#### Progress File Best Practices
- One progress file per logical change or PR
- Keep descriptions concise but informative
- Include issue numbers when applicable (e.g., "Fixes #123")

## Key Technologies

{{CLAUDE_PROMPT}}
List the main technologies, frameworks, and languages used in this project as a bulleted list.
Include version numbers if found in package files (package.json, requirements.txt, etc.).
Group by category (Frontend, Backend, Testing, DevOps, etc.) if applicable.
{{/CLAUDE_PROMPT}}

## Workflows

Any questions or confirmations you would usually ask me, ask Gemini first. Use your Gemini CLI tool for questions and to discuss each step. 

Make sure to use your sequential thinking tool as well. 

Present your plans and your finished tasks to Gemini for review to ensure you didn't introduce new errors or edge cases and that you are building a strong solution. 

Please use sub-agents as much as possible to keep your work focused and progressing quickly. Sub-agents should run in parallel where possible. 

