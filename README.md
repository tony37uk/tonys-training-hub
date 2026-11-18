# Tony's Training Hub

A curated library of AI tools, courses, guides and videos. It opens on a home page (starter path, colour-coded topics, recently added, guides) with a topic sidebar, type filters, search and a "mark as complete" progress tracker saved in your browser.

Live site: https://tony37uk.github.io/tonys-training-hub/

Sister site to the [AI Training Hub](https://github.com/tony37uk/ai-training-hub).

## What's here

- `index.html`: the hub (sidebar, filters, search, progress tracker)
- `guide-*.html`: how-to guides
- `resources-*.html`: resource pages for each training provider

## Adding a resource

Everything lives in one file, `index.html`. Find `const ITEMS = [` near the bottom and add an entry:

```js
{"title": "My new guide", "topic": "agents", "type": "Guide", "src": "Agents",
 "desc": "One-line description.", "url": "guide-my-new-guide.html"}
```

- `topic`: one of `basics`, `tools`, `prompting`, `claude`, `coding`, `agents`, `courses`
- `type`: one of `Tool`, `Course`, `Guide`, `Video`, `Article`
- `url`: a full web address, or a page in this repo like `guide-my-new-guide.html`
- Optional `site`: a second "Visit site" link
- Optional `added`: the date you added it, e.g. `"2026-11-18"`. It then appears under **Recently added** on the home page and shows a **New** label for 30 days

New topics go in the `TOPICS` list just below.
