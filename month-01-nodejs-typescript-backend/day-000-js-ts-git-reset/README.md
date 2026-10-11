# Day 0 — JavaScript, TypeScript, Git/GitHub Reset

## Objective

Refresh coding fluency after a long break and establish a safe, repeatable Git/GitHub workflow before starting the 180-day roadmap.

## Deliverables

- JavaScript solutions with example inputs and outputs.
- TypeScript exercises with strict compiler settings.
- A disposable Git lab repository and notes describing command behavior.
- A GitHub branch and pull request containing Day 0 work.
- Updated root `PROGRESS.md`.

## JavaScript tasks

1. Predict outputs for `var`/`let`/`const`, hoisting, closures, and `this`.
2. Implement `once(fn)`, a closure-based counter, and `memoize(fn)`.
3. Group an array of objects by a key and calculate totals with `reduce`.
4. Write an immutable update for a nested object.
5. Predict output ordering involving synchronous code, promises, and timers.
6. Compare sequential requests with `Promise.all`.
7. Implement bounded retry with exponential backoff and a maximum attempt count.

Place solutions under `javascript/` and include brief explanations in each exercise README or source comments.

## TypeScript tasks

1. Define `ApiResponse<T>` with success and error cases.
2. Define `Result<T, E>` as a discriminated union.
3. Implement `getProperty<T, K extends keyof T>(obj: T, key: K): T[K]`.
4. Implement a generic in-memory `Repository<T>`.
5. Write an exhaustive `switch` using `never`.
6. Explain `any` vs `unknown`, type narrowing, and why API data still needs runtime validation.

Use strict TypeScript settings. Record compiler errors you encountered and how you resolved them.

## Git/GitHub lab

Practise in a disposable repository first.

1. Initialize a repository and inspect `git status`.
2. Add a file, inspect `git diff`, stage it, inspect `git diff --staged`, and commit.
3. Create a feature branch, make a separate commit, and merge it.
4. Create a `.gitignore`; test patterns with `git check-ignore -v`.
5. Practise `git restore --staged` and `git restore <file>` on disposable changes.
6. Compare `git reset --soft`, default `git reset` (mixed), and `git revert`.
7. Stash changes, include untracked files with `git stash -u`, and restore them.
8. Use `git reflog` to locate a previous committed state in the disposable repository.
9. Push a feature branch to GitHub, open a pull request, review the diff, and merge.

## Safety rules

- Never run destructive experiments against the only copy of important work.
- `git restore <file>` discards unstaged edits to that file.
- `git reset --hard` can destroy uncommitted changes.
- `git reset` rewrites local branch history; use it carefully and avoid rewriting shared history.
- `git revert <commit>` creates a new commit that reverses a previous commit.
- Stash untracked files with `git stash -u`.
- If a secret was committed, treat it as exposed and rotate it; deleting it later does not remove it from history.

## Day 0 completion gate

- [ ] Solve most JS exercises without following a tutorial.
- [ ] Implement and explain the TypeScript exercises.
- [ ] Explain working directory vs staging area vs local repository vs remote.
- [ ] Explain restore vs reset vs revert.
- [ ] Push a branch and complete a pull request.
- [ ] Update root `PROGRESS.md` with evidence and self-assessment.

Do not require perfection before moving on. If a skill is weak, record it as a revision item and revisit it during Month 1.
