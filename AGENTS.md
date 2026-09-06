# Agent instructions

## Domain docs

This is a single-context repository. Before changing JB Clarity behavior or
vocabulary, read `CONTEXT.md` for the canonical domain language and every
relevant decision in `docs/adr/`; see `docs/agents/domain.md`. Surface any
conflict with an ADR instead of silently overriding it.

## JB Clarity work

- **Current phase:** prototype implementation. The separate UI-comparison prototype was deliberately skipped; the specification selects the Command Centre information architecture directly.
- `docs/SPEC.md` is the finalized local behavioral source of truth.
- The original build briefs are archived under `docs/briefs/`. They describe how each slice was commissioned and remain the reference for the acceptance criteria that slice was built against.
- Completed slices are recorded in `docs/handoff/`.
- The shared integration boundary is `contracts/workbench.schema.json`. `artifacts/workbench.fixture.json` was Builder 2's temporary input; the generated `artifacts/workbench.json` replaces it without changing the presentation contract.
- For dataset interpretation, read `singhacks-jb-wealth-intelligence/README.md` and `singhacks-jb-wealth-intelligence/docs/DATA_DICTIONARY.md`. Treat `event_log.csv` as the Controlled Event Source for 2026 events.
- Preserve the separation between deterministic analytics, Evidence Packets, presentation, and optional language generation.
- Use the glossary's canonical terms in code, tests, UI copy, and documentation.
- Implement only the assigned vertical slice. Treat unrelated working-tree changes as user-owned.

## Repository

`origin` is this fork, `YXY4NG/SINGHACKS-AAActual-Intelligence`. `upstream` is
the shared team repository, `realjunjiejj/singhack`.

## Completion

Work is complete only when its acceptance criteria pass, relevant tests have
been run, and the result records verification evidence and any remaining
uncertainty.
