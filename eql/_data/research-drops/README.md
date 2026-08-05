# Research Drops

The Research Agent saves each finished research pass here as a dated
markdown file: `YYYY-MM-DD-topic-slug.md`, using the standard
Confirmed / Unconfirmed / Notes for Build Agent structure.

The Integration Agent (polling on a schedule) picks up any file in this
folder that isn't yet in `processed/`, applies the Confirmed facts as
targeted diffs to the relevant HTML, appends a summary to
`eql/_data/research-log.md`, and moves the source file into
`processed/` once applied.

Files in `processed/` are kept for history — don't delete them.
