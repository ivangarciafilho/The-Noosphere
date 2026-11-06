# Card illustrations

`manifest.js` maps exact invocation or spell `data-name` values to external WebP assets.
The inline loader in `index.html` handles initial and dynamically rendered cards without changing their rules or seal controls. Artwork is visible above the seal, as in the incumbent layout; rules remain sealed.

To add a card, append an entry to `window.NOOSPHERE_CARD_ART`:

```js
"Exact Card Name": {
  src: "art/card-slug.webp",
  width: 1600,
  height: 900,
  status: "muse-endpoint",
  alt: "A concise description of the visible scene.",
  provenance: "Original source file and completed generation stage.",
  reviewNotes: "Any known unresolved visual ambiguity."
}
```

Use actual image dimensions. Preserve the source artwork; optimize only a delivery copy. Status is internal provenance, not a claim that an illustration has passed every visual check. Existing finals inherit their status from the publishing checkout.

Keep `index.html`, this directory, and `F:/AI_Tools/noosphere-overhaul/final/living-codex-v30.html` plus its adjacent `art/` directory synchronized. Do not patch the older `final/index.html` editor target.
