# Agent Guide for lab-dict-sets-tuple-en

## Purpose
This repo is a Python lab focused on dicts, sets, and tuples.
Primary deliverable is a Jupyter notebook with student responses.

## Repo Layout
- `README.md` lab instructions and references
- `your-code/challenges.ipynb` student solutions

## Commands
No project-specific build, lint, or test commands were found.
There is no `pyproject.toml`, `setup.cfg`, `requirements.txt`, or `package.json`.
No CI config or Makefile is present.

If you need to run the notebook locally:
- Launch Jupyter from the repo root:
  - `jupyter notebook`
  - Open `your-code/challenges.ipynb`

If you add a test framework later, document it here.
Until then, avoid inventing commands that are not configured.

### Single-test guidance
There is no configured test runner in this repository.
If a test runner is introduced later, include a single-test command here.
For example, if `pytest` is added, single-test patterns typically look like:
- `pytest path/to/test_file.py::test_name`
Only include real commands that exist in the repo.

## Cursor/Copilot Rules
- No `.cursor/rules/` directory found.
- No `.cursorrules` file found.
- No `.github/copilot-instructions.md` file found.
If any of these appear later, update this guide accordingly.

## Code Style
This repo is Python-first and notebook-based.
Follow PEP 8 conventions unless the lab specifies otherwise.
Keep changes small and aligned with the educational context.

### Imports
- Prefer standard library imports first, then third-party, then local.
- Use one import per line for clarity.
- Avoid unused imports; keep notebooks clean.
- Use `import module` over `from module import *`.

### Formatting
- Use 4 spaces for indentation.
- Keep line length reasonable (around 88-100 chars).
- Use blank lines to separate logical blocks.
- Avoid trailing whitespace in notebook cells.

### Naming
- Variables and functions: `snake_case`.
- Constants: `UPPER_SNAKE_CASE`.
- Avoid single-letter names except for short loops.
- Match the lab prompt variable names when required.

### Types
- Type hints are optional in this repo.
- If adding helper functions, annotate public functions when it improves clarity.
- Avoid adding complex typing that distracts from learning objectives.

### Control Flow
- Prefer clear, explicit loops over clever one-liners.
- Use list/set/dict comprehensions when they remain readable.
- Keep conditionals simple; avoid nested complexity in lab answers.

### Error Handling
- Prefer explicit checks over broad `try/except`.
- Catch specific exceptions only when necessary.
- Avoid swallowing errors that help learners understand failures.

### Data Structures
- Favor immutability when it makes sense (tuples for fixed sequences).
- Use sets for membership checks and deduplication.
- Use dictionaries for key-value mappings and frequency counts.

### Notebook Practices
- Preserve the existing prompt text and markdown instructions.
- Place answers directly under the relevant prompt.
- Avoid deleting or renaming cells unless required.
- Keep outputs small; avoid printing huge data unless requested.
- Re-run only the cells you modify when possible.

### Comments
- Add comments only when the code is not self-explanatory.
- Avoid narrating obvious Python syntax.
- Keep comments short and instructional.

### Functions
- The lab generally uses inline solutions, not reusable utilities.
- If you add functions, keep them small and local to the exercise.

## Editing Guidance for Agents
- Do not introduce new dependencies without a clear prompt.
- Do not restructure the notebook; align with the lab flow.
- Avoid altering student outputs unless correcting a mistake.
- Keep solutions aligned with the lesson scope.

## Verification
There are no automated checks.
If you changed the notebook, open it in Jupyter and run the edited cells.
If you cannot run Jupyter, note that verification was not performed.

## When Unsure
- Check `README.md` for lab requirements.
- Avoid inventing commands or styles that are not in the repo.
- Keep the solution minimal, correct, and easy to follow.
