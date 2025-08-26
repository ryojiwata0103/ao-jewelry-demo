# GitHub Deployment Knowledge

## GitHub CLI Commands
- Repository creation with push: `gh repo create [name] --public --source=. --push`
- GitHub Pages enable: `gh api repos/[owner]/[repo]/pages -X POST --field source[branch]=main --field source[path]=/`

## GitHub Pages Configuration
- Default URL pattern: https://[username].github.io/[repository-name]/
- Activation time: 1-2 minutes after enabling
- Source options: branch (main/master) and path (/ or /docs)

## Learned Patterns
1. Use `--source=.` and `--push` together for streamlined deployment
2. GitHub Pages API requires nested field notation for source configuration
3. Always verify Pages status with `gh api repos/[owner]/[repo]/pages` after enabling