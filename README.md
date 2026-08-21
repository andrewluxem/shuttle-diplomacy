# shuttle-diplomacy

Organizes separate supplied accounts into a neutral mediation brief without adjudicating intent or fault.

It produces:

- **Neutral Mediation Brief and Conversation Plan:** a working artifact built from supplied facts, labeled inference, and visible missing fields.

It executes the [Shuttle Diplomacy playbook](https://www.andrewluxem.com/playbooks/shuttle-diplomacy). The playbook teaches the framework. This skill runs it and returns a working artifact.

**Static by construction: no dependencies, executable code, telemetry, network calls, remote instructions, auto-update, scheduled work, or background behavior.** It reads only the files in its own skill folder. Nothing happens until a user or agent invokes it.

## Install

Clone and copy the skill into Claude Code:

```bash
git clone https://github.com/andrewluxem/shuttle-diplomacy.git
cp -r shuttle-diplomacy/skills/shuttle-diplomacy ~/.claude/skills/
```

For Codex, copy the same complete folder to the Codex skills directory:

```bash
cp -r shuttle-diplomacy/skills/shuttle-diplomacy ~/.codex/skills/
```

Or install it as a Claude Code plugin:

```text
/plugin marketplace add andrewluxem/shuttle-diplomacy
/plugin install shuttle-diplomacy@shuttle-diplomacy
```

For clients that install from an archive, use the versioned [shuttle-diplomacy v1.0.0 ZIP](https://www.andrewluxem.com/downloads/shuttle-diplomacy-v1.0.0.zip).

## Invoke it

```text
Prepare a neutral mediation brief and conversation plan
Use the shuttle-diplomacy skill.
```

Naming the skill is always valid: `use the shuttle-diplomacy skill`.

## Files

```text
.claude-plugin/
  plugin.json
  marketplace.json
skills/shuttle-diplomacy/
  assets/neutral-mediation-brief-template.md
  LICENSE.md
  meta.yaml
  references/mediation-standard.md
  SKILL.md
README.md
LICENSE
```

The complete canonical package is copied under `skills/shuttle-diplomacy/`, including every asset, reference, test prompt, source note, changelog entry, and license file present in the source.

## Versioning

Plugin installation is version-pinned. When behavior changes, update the version consistently in `SKILL.md`, `meta.yaml`, `.claude-plugin/plugin.json`, and `.claude-plugin/marketplace.json`, then add a changelog entry. Reinstalling is an explicit update; this repository never auto-updates itself.

## License

MIT. See [LICENSE](LICENSE). The canonical skill folder carries the same authorization in [skills/shuttle-diplomacy/LICENSE.md](skills/shuttle-diplomacy/LICENSE.md).

---

## More playbooks

This skill packages one playbook from the free library at [github.com/andrewluxem/playbooks](https://github.com/andrewluxem/playbooks). Every playbook is free to read, with no email required.
