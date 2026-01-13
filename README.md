# University Public Content Repository

This repository serves as the canonical source of structured public information about the university—its people, academic programs, events, locations, student clubs, and more. All content is stored in human-readable [TOML](https://toml.io) format and can be consumed by websites, apps, or static site generators.

---

## Repository Structure

Content is organized by category under the `content/` directory:

```
config.toml

content/
├── events/
│   └── open-day-2025.toml
├── news/
│   ├── memorial.toml
│   └── card-loss-guideline.toml
├── tracks/
│   ├── physics.nano.toml
│   ├── physics.cosmos.toml
│   └── bioinformatics.toml
├── courses/
│   └── algebra.toml
├── people/
│   ├── alferov.toml
│   └── konstantinov.toml
├── locations/
│   ├── slc.304.toml
│   ├── slc.506.toml
│   ├── fts.411.toml
└── clubs/
    ├── tabletop.toml
    └── tourism.toml
```

## Example: `people/*.toml`

```toml
[person.name]
family = "Federiakin"
given = "Kirill"
middle = "Vladimirovich"

[person]
role = "student"
office = "dorm::1::410"
email = [
	"exomoonhowl@gmail.com"
	"imbexe@gmail.com"
]
phone = [
	"+7 (999) 750-22-86"
	"+7 (900) 600-17-01"
]

[content]
md = """
	Bio.
"""

[links]
orcid = "0000-0000-0000-0000"
github = "reklle"

[[project]]
title = "Some groovy project"
url = "https://groovy.project"
description = """
Explanation why is this interesting.
"""

```
