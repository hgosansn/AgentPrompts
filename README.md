![Last commit](https://img.shields.io/github/last-commit/hgosansn/AgentPrompts?style=for-the-badge)

Agent Prompts
=============

- [baseline-agent.md](baseline-agent.md)
  - Public gist: https://gist.github.com/hgosansn/ad10c24d74b402d15f77a632fe010f7d
- [grunt-developer-agent.md](grunt-developer-agent.md)
  - Public gist: https://gist.github.com/hgosansn/be19039b46a6a247bd1e7cab0c6037bc

Fetching a prompt from a gist
-----------------------

To fetch the latest version of a prompt from a gist:

```bash
gh gist view <gist-id> --raw >> AGENTS.md
```


Updating an existing prompt
-----------------------


To update an existing gist with changes from a prompt file:

```bash
gh gist edit <gist-id> <prompt-file>
```

Replace `<gist-id>` with the actual ID of the gist you want to update and `<prompt-file>` with the name of the prompt file. This command uploads the latest version of the file to the gist.



Adding a new prompt
-------------------

1. Create a new Markdown file under `AgentPrompts`, e.g. `new-agent-prompt.md`.
2. Add the prompt contents and save.
3. Publish as a gist:

```bash
gh gist create new-agent-prompt.md --public --desc "Short description"
```





