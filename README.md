# Codervisor Skills (archived)

> **This repository is archived.** The `leanspec` skill now ships from the LeanSpec
> monorepo itself, alongside the code it documents.

## New install path

```bash
npx skills add codervisor/lean-spec@leanspec
```

(After the upcoming `codervisor/lean-spec` → `codervisor/leanspec` repo rename,
GitHub's auto-redirect keeps the command above working, and
`npx skills add codervisor/leanspec@leanspec` will also resolve.)

The skill source lives at:
- https://github.com/codervisor/lean-spec/tree/main/skills/leanspec

## Why the move?

Two reasons:

1. **Colocate skill with code.** The `leanspec` skill teaches AI agents how to use
   the `leanspec` CLI. Shipping it from the same repo means it can't drift from the
   command surface it documents.
2. **One repo, one source.** The vercel-labs/skills CLI gates internal-only skills
   via `metadata.internal: true`, so the LeanSpec monorepo can host both the
   public skill and internal contributor skills without leaking the latter via
   `npx skills add`.

## License

MIT.
