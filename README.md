# Delta 60 Ltd legal documents

This is the canonical public record of the legal documents for apps published
by Delta 60 Ltd (Company No. 17049123, registered in England and Wales):
privacy policies, terms of service, and data deletion guidance.

The same documents are published, with their hashes, at
[delta60.com](https://delta60.com), for example
[delta60.com/apps/osce-countdown/privacy-policy](https://delta60.com/apps/osce-countdown/privacy-policy).
This repository is the master copy: the website and the apps take their legal
text from here, so every surface shows the same document.

## Structure

- `<app>/<document>.md`: the current version of each document, exactly as
  published. The bytes of this file are what each published SHA-256 refers to.
- `<app>/archive/`: superseded versions, kept forever, named
  `<document>-<version>.md`.
- `manifest.json`: the current version, effective date, SHA-256 hash, and
  canonical URL for every document.

## Verifying a document

To check that a document you downloaded is the one we published, compare its
SHA-256 hash with the one in `manifest.json` (or on the document's page at
delta60.com):

```
sha256sum osce-countdown/privacy-policy.md
```

The git history of this repository is the public record of what changed and
when. A document is only ever changed by publishing a new version: the old
file moves into `archive/` and the manifest is updated to the new version and
hash.

## Contact

hello@delta60.com
