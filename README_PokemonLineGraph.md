# Pokémon Line Graph

**Course:** IB Computer Science HL
**Year:** Junior Year, December 2025

## Description

An introductory data visualization project exploring the relationship between Attack and HP stats across all Pokémon generations. Computes a manual line of best fit (slope and intercept calculated from scratch using sum formulas), identifies statistical outliers using a ±2 standard deviation residual threshold, and offers two interactive annotation modes: outlier labeling or pseudo-legendary/legendary highlighting.

## Files

| File | Purpose |
|---|---|
| `main.py` | Main script — loads CSV, computes regression manually, plots scatter with annotations |
| `pokemon 2.csv` | Dataset of ~1,000+ Pokémon including all forms, with stats and legendary status |

## Requirements

```bash
pip install pandas numpy matplotlib
```

## How to Run

```bash
python main.py
```

When prompted, enter:
- `1` — Highlight statistical outliers and label notable Pokémon by name
- `2` — Highlight all nine pseudo-legendary dragon lines in purple
- `3` — Highlight all legendary Pokémon in gold

## Key Concepts

- Manual linear regression (slope and intercept from summation formulas)
- Pearson correlation coefficient computed from scratch
- Residual-based outlier detection
- Conditional scatter plot annotation using `matplotlib`

## Dataset

`pokemon 2.csv` contains entries for all Pokémon through Generation 8, including regional forms and Gigantamax variants. Columns used: `name`, `hp`, `attack`, `legendary`.
