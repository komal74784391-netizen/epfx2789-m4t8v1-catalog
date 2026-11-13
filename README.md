# Lumen Component Catalog

Source content for the public Lumen component showcase.  Every rendered page
comes from one Markdown file under `content/items/`, and the YAML front matter
of that file is the source of truth for the site.

Front-matter fields:

| field      | meaning                                                              |
|------------|----------------------------------------------------------------------|
| `title`    | display name of the component                                        |
| `slug`     | stable identifier, matches the file name                             |
| `status`   | `published` for live entries, `draft` for work in progress           |
| `category` | showcase grouping                                                    |
| `code_url` | link to the companion implementation repository, once it is released |
| `date`     | notice date recorded for the entry                                   |

Editorial rules:

- Only entries with `status: published` are rendered on the site.  Drafts are
  internal and must not be edited during routine maintenance.
- `code_url` is either a full `https://` URL or empty.  It may only point at a
  repository that we maintain and that already ships the implementation.
- `date` is an ISO `YYYY-MM-DD` value derived from the entry's release notice.
