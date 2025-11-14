# Thomas Carroll Toolkit Documentation - AI Agent Instructions

## Project Overview

This is a Mintlify-powered documentation site for internal business tools (Expenses, Risk Register, Meeting Notes, Refund Requests). Content is written in MDX with YAML frontmatter, using Mintlify components for rich formatting.

## File Structure & Organization

- **Content**: `/tools/` directory with subfolders per tool (e.g., `/tools/expenses/`, `/tools/risk-register/`)
- **Configuration**: `docs.json` controls navigation, theming, and site structure
- **Components**: Use Mintlify components (Steps, Cards, Notes, Warnings) extensively
- **Assets**: Images in `/images/`, logos in `/logo/`, reusable snippets in `/snippets/`

## Writing Standards (from mintify.prompt.md)

- **Language**: Second person ("you") for instructions, UK English spelling
- **Structure**: YAML frontmatter required (`title`, `description`), inverted pyramid content
- **Components**: Steps for procedures, Cards for navigation, Notes/Warnings for callouts
- **Code**: Complete runnable examples with realistic data, proper error handling

## Development Workflow

```bash
# Install CLI globally
npm i -g mint

# Start local development server
mint dev

# Preview at http://localhost:3000
```

## Content Patterns

- **Frontmatter**: Always include `title`, `description`, optional `icon`
- **Navigation**: Tools organized in `docs.json` navigation tabs with groups/pages
- **API Docs**: OpenAPI specs in `/api-reference/openapi.json` with MDX wrapper pages
- **Reusable Content**: Use snippets system in `/snippets/` to avoid duplication
- **Progressive Disclosure**: Accordions for optional details, expandable sections for nested data

## AI Tool Integration

- **Claude Code**: Use `CLAUDE.md` at project root for consistent documentation standards
- **Guidelines**: Push back on ideas with reasoning, ask for clarification, never guess
- **Content Strategy**: Document for user success, prioritize accuracy, avoid duplication

## Key Reference Files

- `mintify.prompt.md`: Complete writing guidelines and component reference
- `docs.json`: Navigation and site configuration
- `/tools/expenses/introduction.mdx`: Exemplar content structure and component usage

## Quality Checks

- Validate frontmatter on all new pages
- Test local preview with `mint dev` before committing
- Ensure consistent terminology across related pages
- Use realistic examples, never placeholder data
- Include verification steps for procedures</content>
  <parameter name="filePath">/Users/mike.rudge/sites/toolkit-docs/.github/copilot-instructions.md
