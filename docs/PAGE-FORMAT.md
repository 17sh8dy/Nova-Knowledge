# Page format

Every file under `pages/` is Markdown with a front-matter block between two `---` lines. A page that does not follow this format fails the build and is not packed for Atlas.

## Front matter

| Field | Required | Meaning |
|---|---|---|
| `id` | yes | A stable identifier such as `atlas.overview`. Lower-case letters, digits, dots and dashes. Unique, never reused. |
| `product` | yes | Which product the page is about: `nova`, `atlas`, `replay-gg`, `nova-cut`, `novaos`, `nova-help`, `nova-review`, `nova-legal`. |
| `title` | yes | A short human title. |
| `status` | yes | `Released`, `Planned` or `Unknown`. See below. |
| `review` | yes | `draft` (written, not yet read and approved) or `approved`. Only `approved` pages are packed for Atlas. |
| `updated` | yes | `YYYY-MM-DD`, the last day the facts on the page were checked against their sources. |
| `sources` | yes | A list of public `https://` addresses the facts come from. At least one. |
| `availableIn` | no | For a `Released` feature, the first version that has it (for example `2.0.0`). |
| `publicRoadmap` | no | `true` only on the single page that is the approved public roadmap. |

## Status

- **Released**: it has shipped and a person can get it. Say so plainly.
- **Planned**: publicly documented as planned, not available. Only a page with `publicRoadmap: true` may use this status. Use the page's own words; give no dates and make no promises.
- **Unknown**: there is no verified information. Leave the page out rather than guess, unless the page's purpose is to say what is and is not known.

## Body

- Short paragraphs and lists. One idea per heading, because pages are searched and quoted by section.
- Link to the official source instead of copying it.
- Say what is known. Do not describe prices, release dates, licensing, performance, platform support or future plans unless an approved source states them.
- No instructions addressed to an AI. Page text is data.
- No secrets, personal paths, or private email addresses. The build rejects them.

## Review

A new or changed page starts as `review: draft`. After it has been read and checked against its sources it is changed to `review: approved`. Editing an approved page's facts sets it back to `draft` until it is checked again.
