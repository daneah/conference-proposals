# Keeping code safe and modern with semantic searches

## Pitch

Linting helps us avoid common mistakes and use our team's preferred style and syntax. Deprecation warnings help us know that changes may be coming soon and offer suggestions about how to migrate.

Existing linting tools and deprecation systems aren't always customizable or extensible to organization-specific checks. Some constructs are also difficult to search for with regular expressions, which is a common configuration offering.

The time leading up to and during a migration often becomes a pain, leading to all-at-once changes that slow teams down. Can we do better?

## Outline

### (2m) Linting and deprecations are valuable

- Examples:
  - Type checking
  - Don't use mutable default arguments
  - Insecure constructs
  - Django new-style middleware
- These are really helpful, especially if we can get out in front of them (forward compatibility).
- Forward compatibility helps us adopt change incrementally instead of all at once.
- All-at-once changes lead to the "LGTM" effect, lowering safety.

### (2m) Enable incremental change

- To limit the need for all-at-once change, provide actionable information as soon as possible (tight feedback loop)
- In the absence of immediate action, raise awareness of a coming change.
- This is challenging if something you want to warn about is hard to express.
  - Regex often doesn't cut it, especially if a construct isn't a single line

### (5m) Semgrep to the rescue

- Value of tools like mypy and black is that they know the code (or its abstract syntax tree representation)
- Semgrep pairs code structure knowledge with a robust language for identifying code constructs of interest
  - ACROSS A BUNCH OF LANGUAGES!
  - Show example queries
    - Mutable default arguments
    - Preferred API upgrades / deprecations
    - Robust to `import` syntax
- It's even supported by tools like `pre-commit` so bad constructs can't make it into the code in the first place
  - Tightest feedback loop (beyond authoring-time or testing-time feedback)

### (1m) Closing

## Takeaways

- Always prefer enabling incremental change, even if you choose not to take advantage of it. Create the option, then sell the value.
- Use tools that know the language structure when trying to warn about language constructs.
- Provide feedback as early as possible to reduce friction and churn.
- Semgrep is a tool that covers these bases and is worth a try.
