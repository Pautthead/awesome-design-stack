# Contributing

Thanks for helping keep this list useful and alive. This list is maintained bilingually: `README.md` (English) and `README.es.md` (Spanish). Both must stay in sync.

## Inclusion criteria

An entry is accepted when it meets **all** of these:

1. **Real and alive.** The URL responds 200 and the product/site is maintained.
2. **Useful for building.** It helps someone design or build a website or app: inspiration, system, skill, component, tool, or knowledge.
3. **Free, open source, or with a meaningful free tier.** Paid-only products are generally rejected.
4. **Curated, not dumped.** One entry per resource; no link farms, no SEO-bait directories, no listicles.
5. **No affiliate links, ever.**

Additionally:

- Repos should be maintained (activity in the last ~12 months) unless they are canonical references (e.g. a classic book or a foundational spec).
- Sites that block automated link checkers (403/429 to bots) will fail CI; prefer an alternative resource that can be verified automatically.
- No self-promotion unless the resource is notable beyond your own project.

## Entry format

One line per entry, in the correct category section, in both READMEs:

```md
- [Name](https://example.com) - One-line description that says what it is and why it matters.
```

Rules:

- Description: one line, starts with a capital letter, ends with a period, in English for `README.md` and Spanish for `README.es.md`.
- No marketing superlatives ("the best ever"). Say what the tool does.
- Star counts (`128k★`) are only used for large repos, written as `NNNk&#9733;`, and must be roughly current at the time of the PR.
- Keep both files in sync: an entry added to one must be added to the other in the same PR.

## Categories

If a new entry does not fit any existing category, propose a new one in an issue first. New categories must have at least 5 entries to be created.

## How to contribute

**Easiest:** open an issue using the "Suggest an entry" template. The maintainer will verify and add it.

**By PR:**

1. Fork the repo (once it is published).
2. Add the entry to `README.md` and `README.es.md` in the right category.
3. Update the count in the Contents list for that category.
4. Run the link check locally if you can:

   ```sh
   curl -s -o /dev/null -w "%{http_code}" -L -A "Mozilla/5.0" "https://your-url.example"
   ```

   It must return `200`.

5. Open the PR using the template.

All PRs are checked by the automated [link-check workflow](.github/workflows/link-check.yml) (lychee). If your link fails it, the PR cannot be merged.

## Reporting a broken link

Open an issue titled `Broken link: <name>` with the URL and what you see (404, redirect, parked domain). Alternatively, just submit a PR removing or replacing the entry in both READMEs.

## Code of conduct

Be civil. Entries about (or links to) harassment, hate, gambling, crypto-pump or adult content will be rejected and the issue closed.

## License

By contributing, you agree that your contributions are released under [CC0](LICENSE).
