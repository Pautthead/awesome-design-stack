## What does this PR do?

- [ ] Adds a new entry
- [ ] Fixes a broken link
- [ ] Removes an entry
- [ ] Other

## Entry details

- Name:
- URL:
- Category:

## Checklist

- [ ] Entry added to **both** `README.md` (English) and `README.es.md` (Spanish), in the same category.
- [ ] Entry count updated in the Contents list of both files.
- [ ] Entry follows the format: `- [Name](url) - One-line description.`
- [ ] The URL responds `200` and does not block automated link checkers.
- [ ] No affiliate links.
- [ ] Description has no marketing superlatives.
- [ ] Star counts (if used) are roughly current.

## Link check

The automated workflow must pass before merge. You can pre-check locally:

```sh
curl -s -o /dev/null -w "%{http_code}\n" -L -A "Mozilla/5.0" "https://your-url.example"
```
