# Claude Code SaaS/Web App Template

## Project Overview
This is a comprehensive template for building SaaS applications and front-end websites using Claude Code best practices. The structure is designed to support AI-driven development workflows with automated design review, comprehensive testing, and intelligent code assistance.

## Quick Start Commands

### Development
```bash
npm install           # Install dependencies
npm run dev          # Start development server
npm run build        # Build for production
npm run preview      # Preview production build
npm run lint         # Run linting
npm run typecheck    # Run TypeScript checks
npm test             # Run tests
```

### Claude Code Workflows
```bash
# Analyze codebase structure
/analyze-codebase

# Update documentation
/update-claude-md

# Run design review
@agent-design-review

# Clear context for fresh start
/clear
```

## Code Style Guidelines

### TypeScript/JavaScript
- Use TypeScript for all new code
- Prefer functional components with hooks
- Use descriptive variable and function names
- Follow the existing naming conventions:
  - Components: PascalCase
  - Functions: camelCase
  - Constants: UPPER_SNAKE_CASE
  - Files: kebab-case

### React Patterns
- Custom hooks for reusable logic
- Context for global state management
- Component composition over inheritance
- Props destructuring in component signatures

### File Organization
- Group related files in feature folders
- Index files for clean imports
- Separate concerns (logic, UI, styles)
- Co-locate tests with source files

## Testing Strategy
- Unit tests for utility functions
- Component tests for UI behavior
- Integration tests for user flows
- E2E tests for critical paths

## Repository Etiquette

### Before Starting Work
1. Read relevant CLAUDE.md files in subdirectories
2. Check ARCHITECTURE.md for system design
3. Review CONTRIBUTING.md for guidelines
4. Update plan.md for large features

### Development Workflow
1. **Explore**: Use Claude to understand existing code
2. **Plan**: Create detailed implementation plan
3. **Code**: Implement following TDD when appropriate
4. **Review**: Use design review agent for UI changes
5. **Commit**: Write clear, descriptive commit messages

### Git Conventions
- Use conventional commits format
- Keep commits atomic and focused
- Reference issues in commit messages
- Use meaningful branch names

## Developer Environment Setup

### Prerequisites
- Node.js 18+ 
- npm/yarn/pnpm
- Git
- VS Code (recommended)

### Recommended Extensions
- TypeScript and JavaScript Language Features
- ESLint
- Prettier
- Auto Rename Tag
- GitLens

## Architecture Patterns

### Frontend Structure
- **src/components**: Reusable UI components
- **src/pages**: Application pages/routes
- **src/hooks**: Custom React hooks
- **src/utils**: Utility functions and helpers
- **src/services**: API clients and external services
- **src/types**: TypeScript type definitions
- **src/styles**: Global styles and theme configuration

### Design System Integration
- Consistent component library
- Design tokens for spacing, colors, typography
- Responsive breakpoints
- Accessibility compliance (WCAG 2.1 AA)

## Claude Code Best Practices

### For Claude Developers
1. **Be Specific**: Mention specific files and components
2. **Provide Context**: Use screenshots for visual work
3. **Follow TDD**: Write tests first when appropriate
4. **Iterate Early**: Course correct frequently
5. **Use Subfolders**: Check CLAUDE.md in each directory

### Visual Development Workflow
1. **Quick Visual Check** (after implementation):
   - Identify what changed
   - Navigate to affected pages  
   - Verify design compliance
   - Capture evidence (screenshot at 1440px)
   - Check for console errors

2. **Comprehensive Design Review** (before PR):
   - Invoke `@agent-design-review`
   - Test responsiveness across devices
   - Validate accessibility compliance
   - Check visual polish and consistency

### Multi-Agent Workflows
- Use multiple Claude instances for complex tasks
- Separate concerns: development, review, testing
- Leverage git worktrees for parallel development
- Use custom slash commands for repeated workflows

## Context Files Reference

### Design & Review
- `/context/design-principles.md` - Comprehensive design standards
- `/context/style-guide.md` - Brand and visual guidelines
- Check individual CLAUDE.md files in each subdirectory

### Documentation
- `ARCHITECTURE.md` - System design and technical decisions
- `CONTRIBUTING.md` - Development guidelines and processes
- `CHANGELOG.md` - Version history and updates
- `plan.md` - Large project planning and roadmap

## Common Tasks

### Adding New Features
1. Plan in plan.md if complex
2. Create/update relevant CLAUDE.md files
3. Follow TDD workflow
4. Update tests and documentation
5. Run design review for UI changes

### Bug Fixes
1. Write failing test to reproduce
2. Fix the issue
3. Verify test passes
4. Update documentation if needed

### Refactoring
1. Ensure test coverage
2. Make changes incrementally
3. Verify tests continue passing
4. Update affected documentation

## Deployment

### Production Checklist
- [ ] All tests passing
- [ ] Type checking clean
- [ ] Linting passes
- [ ] Design review approved
- [ ] Performance optimized
- [ ] Accessibility validated
- [ ] Documentation updated

Remember: This template is designed to work seamlessly with Claude Code's AI-driven development workflows. Always leverage the available documentation and context files for optimal results.