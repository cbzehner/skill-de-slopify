# De Slopify

Clean up prose that sounds machine-written. The skill removes filler, generic structure, over-polished transitions, and other patterns that make useful writing feel synthetic.

## Use It For

- Editing README, docs, blog, or product copy
- Making AI-assisted writing sound like a person wrote it
- Cutting boilerplate without losing the point

## Install

Clone the repo and run the installer:

```bash
git clone https://github.com/cbzehner/skill-de-slopify.git
cd skill-de-slopify
./install.sh all
```

Install targets:

- `./install.sh claude` installs to `~/.claude/skills/de-slopify`
- `./install.sh codex` installs to `~/.codex/skills/de-slopify`
- `./install.sh agents` installs to `~/.agents/skills/de-slopify`
- `./install.sh opencode` installs to `~/.config/opencode/skills/de-slopify`
- `./install.sh all --copy` copies files instead of symlinking

Manual install works too: symlink or copy `skills/de-slopify` into your agent's skills directory.

## Agent Support

This repo uses the plain `skills/de-slopify/SKILL.md` layout. Claude Code and Codex also get small plugin manifests at `.claude-plugin/plugin.json` and `.codex-plugin/plugin.json`.

Other agents can read the same `SKILL.md` file. If a host does not support a frontmatter field or tool name, ignore that field and follow the workflow text.

## Layout

```text
.claude-plugin/plugin.json
.codex-plugin/plugin.json
install.sh
skills/de-slopify/SKILL.md
README.md
LICENSE
```

## Public Notes

These repos are public. Keep private repo names, secrets, customer data, raw logs, cookies, and absolute filesystem paths out of examples.

## License

MIT
