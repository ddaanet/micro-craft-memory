---
name: ghmem-operating-the-pipeline
description: "running ghmem on this corpus: topic space looks fragmented (`atomic-file-save` beside `backup-filename-encoding`) — read the routing notes, not the names; a topic holding a single item is not synthesized yet; four concurrent `ghmem:ghmem-triage` workers is this box's ceiling; changing heat weights needs a demonstrated ranking gain; `ghmem heat` / `ghmem show` answer corpus questions without spending routes"
metadata:
  type: project
---

## Dispatching workers

Four concurrent `ghmem:ghmem-triage` workers is what this box takes — my
human partner's measurement, not a guess.

A topic holding a single item is not synthesized: its siblings arrive with
later triage batches, and the topic doc is then paid for twice.

## Judging the topic space

Read the routing notes, not the topic names, before calling the space
fragmented. `atomic-file-save` beside `backup-filename-encoding` looks like
one theme split in two; the notes show temp-file-plus-rename semantics
against path-length overflow, and they are correctly distinct.

## Touching the heat weights

The bar for changing the weights is a demonstrated ranking gain, measured as
in `docs/ghmem-heat-weights.md`: the order mints topic names, so a change
reorders them.

Corpus questions are answerable read-only — `ghmem heat` emits the whole
ranking as CSV and `ghmem show` renders any item — so sample and classify
rather than spend routes.
