# English prototype — War in Iran

This directory contains the **English version** of the prototype. It is a fictional news story about an emergency session of the U.N. Security Council, displayed as if on a real news website.

## Files

| File | What it is |
|---|---|
| `index.html` | The complete prototype — open in any browser |

## How to view

Just open `index.html` in your browser. If the repository is published via GitHub Pages, the same content is available at:

```
https://liviasouzavieira.github.io/prototipo-correcao-jornalismo/en/
```

## What to look for

The fictional story shows, within a normal news-reading context, the **eight signaling patterns** proposed by the protocol:

- **Headline and standfirst** with corrections: hover over the colored words ("meeting" in indigo, "Friday" in red) — the ✎ icon signals a correction.
- **Story body** with collapsible errata below paragraphs: each errata has a title, reason, before/after diff, and date/time of the change.
- **Yellow "new content" boxes** at points where information was added after initial publication.
- **Corrections tab**: at the top of the story, click on "Corrections" to see every errata in the coverage, with type filters.
- **Visual legend**: in the right sidebar, see the meaning of each color.
- **Report-an-error button**: at the end of the story, click "Report an error" to see the reader communication modal.

## Testing the 24-hour behavior

Add `?simulate=25h` to the URL to see the story's state after 24 hours:

```
index.html?simulate=25h
```

Other options: `+2h`, `+12h`, `+23h`, `+72h`. Click-through shortcuts are also available in the discreet banner at the top of the story.

**What changes after 24h:**

- The yellow "new content" boxes lose their marking (text flows into the article naturally)
- The "NEW · added Xh ago" pills disappear
- The "removed passage" block vanishes entirely
- Corrections (factual, spelling, imprecision, statement rectification) and right of reply **always remain**

## Back to the index

Go back to the [main prototype index](../) to see both versions (PT and EN) and the project description.
