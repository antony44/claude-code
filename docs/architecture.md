
# Repository Architecture Guide

This document explains the structure and philosophy of the Claude Code Excellence repository.

## Top-Level Directories

- **apps/**: Contains standalone applications or example projects. Each subfolder is its own project (e.g., `web-basic`, `web-next`, `saas-starter`). Applications should import primitives from `skills/` rather than copying code.
- **skills/**: Reusable modules grouped by domain. These are the building blocks of your applications. Each module is a primitive with clean interfaces. Avoid duplicates and ensure functions are configurable.
- **templates/**: Starting points for new projects. Copy a template to `apps/` when starting a new project. Templates should not be used directly in production.
- **docs/**: Documentation and design discussions. Update this section when the architecture evolves.
- **CLAUDE.md**: Rules for using this repo with Claude Code. Follow these guidelines to maintain a healthy codebase.

## Skills Organization

- **web/**: Front-end primitives for SEO, UI components, analytics hooks, and CMS integration.
- **video/**: Tools for video creation and editing. Includes Remotion presets, animations, formats, subtitles, and FFmpeg helpers.
- **infra/**: Infrastructure scripts and configurations (Supabase integration, SQL migrations, deployment scripts).
- **shared/**: Common types and utilities shared across domains.

## Best Practices

- Design primitives that solve general problems and are highly configurable.
- Keep applications thin by delegating logic to `skills/`.
- Review and refactor regularly to avoid accumulating redundant code.
- Document new modules and changes thoroughly to help future developers and AI assistants.

This architecture is designed to scale with your needs while keeping complexity manageable.
