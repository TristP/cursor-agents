# cursor-agents

Repository for managing multiple AI agent projects in Cursor IDE

## Purpose

This repository is designed to work with Cursor's multi-agent feature, allowing you to have different AI agents work on separate projects within a single workspace.

## Structure

Each subdirectory represents a separate project that can be worked on by different AI agents:

```
cursor-agents/
├── agent-1/          # First project/agent workspace
├── agent-2/          # Second project/agent workspace
├── agent-3/          # Third project/agent workspace
└── shared/           # Shared resources across all projects
```

## How to Use with Cursor

1. **Open this repository in Cursor**:
   ```bash
   cursor "C:\Users\TristanPerot\VAT EPR EXPERT FRANCE\Companies - Tristan Perot - Documents\Code\cursor-agents"
   ```

2. **Create project folders** for each agent:
   - Create a new folder for each separate project/task
   - Each folder acts as an isolated workspace for an agent

3. **Configure Cursor Agents**:
   - Use Cursor's composer to work on specific folders
   - Each agent can focus on its own directory
   - Agents won't interfere with each other's work

## Example Projects

You can organize your projects like:
- `invoice-extraction/` - Invoice processing tools
- `payment-reconciliation/` - Payment matching systems
- `data-automation/` - Automation scripts
- `api-integration/` - API clients and integrations

## Benefits

- ✅ **Isolation**: Each project is separate and independent
- ✅ **Version Control**: All projects in one git repository
- ✅ **Easy Management**: Switch between projects easily
- ✅ **Collaboration**: Multiple agents can work simultaneously
- ✅ **Shared Resources**: Common utilities in the `/shared` folder

## Getting Started

To add a new project:

```bash
cd cursor-agents
mkdir new-project-name
cd new-project-name
# Start working on your project here
```

## Notes

- Each project can have its own `requirements.txt`, `package.json`, or dependency files
- Use the `.gitignore` to exclude virtual environments, node_modules, etc.
- Commit and push your changes regularly to keep everything synced

---

Created: November 25, 2025
