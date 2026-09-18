# Reconstructing Computing

A working record of rebuilding the abstractions beneath modern computing.

This repository is intentionally split into two layers:

- **code** — implementations and experiments
- **docs** — raw notes, maps, diary entries, security observations

The polished work belongs elsewhere. This repository is the workshop.

## Documentation

The site lives in `docs/` and is designed for GitHub Pages.

There is:

- no framework
- no build step
- no dependency installation
- no generator required

Open `docs/index.html` directly in a browser or publish the `docs/` folder with GitHub Pages.

## Fast workflow

To document a new topic:

1. Copy `templates/topic.html`
2. Rename it to `docs/topics/<topic>.html`
3. Replace the placeholder text
4. Add one link in `docs/topics/index.html`
5. Optionally add the topic to the ASCII map in `docs/index.html`
6. Commit

To add a diary entry:

1. Open `docs/log/index.html`
2. Duplicate the latest `<article class="log-entry">...</article>`
3. Change the date and write a few lines
4. Commit

That is the entire documentation system.

## Status notation

```text
[ ] unexplored
[~] studying
[*] implementing
[+] implemented
[!] security observation
[#] documented
```

## Published work

https://grimlabs.org
