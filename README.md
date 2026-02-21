![GitHub stars](https://img.shields.io/github/stars/hgosansn/AgentPrompts?style=for-the-badge)
![GitHub issues](https://img.shields.io/github/issues/hgosansn/AgentPrompts?style=for-the-badge)
![Last commit](https://img.shields.io/github/last-commit/hgosansn/AgentPrompts?style=for-the-badge)
![Top language](https://img.shields.io/github/languages/top/hgosansn/AgentPrompts?style=for-the-badge)
![License](https://img.shields.io/github/license/hgosansn/AgentPrompts?style=for-the-badge)

Agent Prompts
=============

- [grunt-developer-agent.md](grunt-developer-agent.md)
  - Public gist: https://gist.github.com/hgosansn/be19039b46a6a247bd1e7cab0c6037bc


Updating an existing prompt
-----------------------


To update an existing gist with changes from a prompt file:

```bash
gh gist edit <gist-id> grunt-developer-agent.md
```

Replace `<gist-id>` with the actual ID of the gist you want to update. This command uploads the latest version of the file to the gist.



Adding a new prompt
-------------------

1. Create a new Markdown file under `AgentPrompts`, e.g. `new-agent-prompt.md`.
2. Add the prompt contents and save.
3. Publish as a gist:

```bash
gh gist create new-agent-prompt.md --public --desc "Short description"
```

Notes
-----

- The README lists prompt files relative to this repository root. Add any new prompt files to the `AgentPrompts` folder so they appear here.
- If you prefer one canonical gist per prompt, copy the gist URL into this README next to the corresponding file.





