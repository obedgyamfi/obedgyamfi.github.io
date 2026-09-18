# Documentation Workflow

The rule: **documentation must never become a reason not to code.**

## New topic — under one minute

```bash
cp templates/topic.html docs/topics/utf8.html
```

Then edit only:

```text
TOPIC TITLE
status
started
language
depends
unlocks
code
00. Question
```

Everything else can remain incomplete until you actually learn something worth recording.

Add one line to:

```text
docs/topics/index.html
```

Example:

```html
<li><a href="./utf8.html">[*] UTF-8</a></li>
```

That is enough.

---

## While coding

Do **not** continuously write polished prose.

Keep rough bullets under:

```text
03. Implementation
04. Invariants
05. Break It
06. What Changed In My Understanding?
```

Examples:

```text
- continuation bytes always begin with 10xxxxxx
- accidentally accepted an overlong encoding
- assumed one visible character == one code point; false
```

Clean it up only if you feel like it.

---

## Daily log

A daily log is optional.

If something interesting happened, append:

```html
<article class="log-entry">
...
</article>
```

to:

```text
docs/log/index.html
```

Five lines is enough.

---

## What deserves documentation?

Document something when one of these happens:

```text
[+] I implemented something.
[?] My mental model changed.
[!] An assumption broke.
[!] I found a security-relevant edge case.
[*] I discovered a dependency I did not know existed.
```

Do not document routine syntax or every function you write.

---

## Suggested commit rhythm

```text
representation/int: decode little-endian u32
representation/int: add signed overflow tests
docs/int: note truncation behavior
```

Code first. Notes second.
