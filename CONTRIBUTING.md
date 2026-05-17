# Contributing to claude-skills-starter

claude-skills-starter is a curated subset of the [claude-skills](https://github.com/rampstackco/claude-skills) catalog. Contributions are limited in scope by design.

## Where to contribute

### Skill content changes

All skill content changes (improvements to a SKILL.md, additions to a skill's reference files, bug fixes in skill instructions) should be made to the source repository at [claude-skills](https://github.com/rampstackco/claude-skills). Once accepted there, the change can be re-synced to this starter set.

### Adding or removing a skill from the starter set

Open a discussion at [claude-skills discussions](https://github.com/rampstackco/claude-skills/discussions) proposing the change. The discussion should include:

- The skill name and what it does
- Why it belongs (or does not belong) in the starter set
- Which skill, if any, you would remove to keep the set focused

### Bug reports for the starter repo

If you spot a problem with how the starter repository has copied or referenced a skill (missing files, broken cross-references, README inaccuracies), open an issue here.

## What's out of scope

- New skills not in claude-skills
- Significant edits to skill content (those belong upstream)
- Major reorganization of the skill structure
- Additional tooling (the linter is enough for now)
- Plugin packaging for specific Claude Code harnesses

## Linting

The repository ships a Python linter that validates structural conventions across all skills:

```bash
pip install pyyaml
python .github/scripts/lint_skills.py
```

CI runs this on every push and pull request to `main`. It is adapted from the claude-skills linter, with two checks omitted because this repo is a curated subset rather than the full catalog (cross-skill reference validation and generated-README validation).

## License

By contributing, you agree that your contributions will be licensed under the MIT License.
