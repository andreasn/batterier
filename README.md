# Sweden's grid batteries

A one-page site listing grid-scale battery storage projects in Sweden, from about 1 MW upward: who is building them, how big they are, where they are and when they go online. Home batteries and smaller units are not included.

**Live site:** https://andreasn.github.io/sweden-battery-storage/

## Data

[`data/projects.csv`](data/projects.csv) has one row per project, with these columns:

| Column | Meaning |
|---|---|
| `project` | Project or site name |
| `developer` | Developer and/or owner |
| `location` | Municipality or nearest town, and county |
| `price_area` | Electricity price area (SE1–SE4): from a source where stated, otherwise worked out from the location; blank if the location is unknown |
| `power_mw` | Rated power in MW, blank if not published |
| `energy_mwh` | Storage capacity in MWh, blank if not published |
| `status` | `Operational`, `Under construction`, `Planned` or `Permitting` |
| `online` | Actual or planned date the battery went or goes online |
| `date_reported` | Date of the main source |
| `source` | Link to the main source |
| `notes` | Other details, including conflicting figures between sources |

Planned projects need an investment decision, a signed construction contract or a building permit; projects with only an announcement, land agreement or letter of intent are not listed. Each project is checked against at least one public source: a company press release, an annual report, a project page or a news article. Where sources disagree, the most recent figure is used and the disagreement is noted.

On the site, a size filter splits projects at 10 MWh (by MWh, or MW where MWh is not published), matching the size classes Statistics Sweden uses.

The list is not complete. Green Power Sweden counted 130 approved battery parks totalling about 5,100 MW at the end of 2025, most without a published developer or size.

## Updating

The data is also embedded in `index.html`, in the `<script id="data">` block. When adding or changing a project, update both that block and the CSV.
