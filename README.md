# Software Carpentry — Programming with Python (University of Twente)

Worked notebooks, exercise templates and datasets from the **University of Twente Software Carpentry
Python training**, May 2026. The material follows the Software Carpentry lesson
[*Programming with Python*](https://swcarpentry.github.io/python-novice-inflammation/) and is kept here
as a complete, runnable copy — exercise templates alongside worked solutions — for participants who want
to revisit the workshop afterwards.

> **Trainer:** Néstor DelaPaz-Ruíz (UT-LISA).
> This repository is a participant/assistant copy of the workshop material, not the canonical lesson.
> The upstream lesson lives with [The Carpentries](https://swcarpentry.github.io/python-novice-inflammation/).

## Contents

| Folder | What is in it |
| --- | --- |
| `Python_Day1/` | Six notebooks — intro, analysing data with NumPy, visualising with Matplotlib, lists & dictionaries, loops, and analysing multiple files. `templates/` holds the blank versions handed out in the session; the top-level notebooks hold the worked solutions. |
| `Python_Day1/data/` | The `inflammation-*.csv` clinical-trial dataset (12 files) plus the `small-*.csv` toy tables used in the early exercises. |
| `Python_Day2/` | Errors and exceptions, defensive programming, debugging, and command-line programs — `Python_Day2.ipynb` plus `exercises_Python_2.ipynb`. |
| `Python_Day2/code/` | Standalone scripts built up over Day 2: the `readings_01…09.py` progression from a bare script to a full CLI tool, plus `argv_list.py`, `count_stdin.py`, `line_count.py`, `my_ls.py`, `rectangle.py`. |

## What the lesson covers

**Day 1 — analysing tabular data.** Loading CSV data with NumPy, slicing and aggregating arrays,
plotting with Matplotlib, Python's core collection types, writing loops, and generalising a single-file
analysis to a whole directory of files.

**Day 2 — writing programs that survive contact with reality.** Raising and handling exceptions,
assertions and defensive programming, using a debugger, splitting code into modules, and turning a script
into a command-line program that reads `sys.argv` and standard input.

## Running the material

```bash
git clone https://github.com/apkirana/carpentry_python.git
cd carpentry_python
python3 -m venv .venv && source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -r Python_Day1/requirements.txt
jupyter notebook
```

Open `Python_Day1/templates/01-intro.ipynb` to work through the exercises yourself, or the matching
notebook one level up to read the solution.

Day 2 scripts run directly from the command line:

```bash
cd Python_Day2/code
python readings_09.py --mean ../data/inflammation-*.csv
```

## Licence and attribution

The lesson content is derived from The Carpentries' *Programming with Python*, released under
[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Reuse under the same terms, crediting
The Carpentries and the workshop trainer.

## Maintainer

**Annisa Puspa Kirana** — PhD researcher, Faculty of Geo-Information Science and Earth Observation (ITC),
University of Twente.
[Google Scholar](https://scholar.google.com/citations?user=BQl6KOsAAAAJ&hl=en) ·
[ORCID](https://orcid.org/0000-0002-4622-1445) ·
[LinkedIn](https://www.linkedin.com/in/annisapuspakirana) ·
[GitHub](https://github.com/apkirana)
