
# Rules for Claude Code

These guidelines help Claude Code work effectively with this repository:

1. **Respect the structure**: Do not modify files in `skills/` unless you are refactoring with explicit permission. These modules are primitives meant to be reused.
2. **Use primitives**: When implementing new features in apps or templates, prefer composing existing modules from `skills/` over writing bespoke code.
3. **Separation of concerns**: Keep application-specific code in `apps/`, reusable libraries in `skills/`, and scaffolds in `templates/`.
4. **Documentation**: Update `README.md` files in each folder when adding new functionality or altering structure. Document new primitives clearly.
5. **Review before removal**: If you think a module is unused or redundant, propose a refactor rather than deleting directly. State the reason and your intended replacement.
6. **Minimal duplication**: Avoid copying code between apps; extract shared logic into `skills/` and import it instead.
7. **Ask clarifications**: If instructions are ambiguous or conflict with these rules, ask for clarification before proceeding.

By following these rules, Claude Code will maintain consistency and integrity across the repository.
