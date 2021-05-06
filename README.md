# pre-commit hooks

Some custom pre-commit hooks for [pre-commit](https://github.com/pre-commit/pre-commit).

### Using pre-commit-hooks with pre-commit

Add this to your `.pre-commit-config.yaml`

    -   repo: https://github.com/mbaechtold/pre-commit-hooks
        rev: v1.0.0  # Use the ref you want to point at
        hooks:
        -   id: js-debug-statements
        -   id: js-it-only

### Hooks

- `js-debug-statements` - Check Vue (`.vue`) and JavaScript files for debug statements, such as:
    - `console.log`
    - `debugger`
    
- `js-it-only` - Check Vue (`.vue`) files for "it.only" statements.
