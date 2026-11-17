# Tony's Training Hub

A curated library of AI tools, courses, guides and videos, organised by topic with a sidebar, type filters, search and a "mark as complete" progress tracker saved in your browser.

Live site: https://tony37uk.github.io/tonys-training-hub/

Sister site to the [AI Training Hub](https://github.com/tony37uk/ai-training-hub). The how-to guides and provider resource pages open there.

## Adding a resource

Everything lives in one file, `index.html`. Find `const ITEMS = [` near the bottom and add an entry:

```js
{"title": "My new guide", "topic": "agents", "type": "Guide", "src": "Agents",
 "desc": "One-line description.", "url": "https://example.com"}
```

- `topic`: one of `basics`, `tools`, `prompting`, `claude`, `coding`, `agents`, `courses`
- `type`: one of `Tool`, `Course`, `Guide`, `Video`, `Article`
- Optional `site`: a second "Visit site" link

New topics go in the `TOPICS` list just below.
