# Requirements Checklist: 44943 Lab: Filtering, Ordering, Limiting, and Grouping Data with SQL

Source: Canvas description + rubric (latest_assignments.json), plus the starter notebook/repo instructions.

Deliverable: `SQLFilterOrderGroupLab.ipynb`

| # | Requirement (explicit or implied) | Rubric criterion | How it's met | Status |
|---|---|---|---|---|
| 1 | Step 1: all columns, planets with 0 moons (WHERE =) | Basic Filtering | `df_no_moons` (Mercury, Venus) | ✅ |
| 2 | Step 2: name, mass where name has 7 letters, no hard coding (LENGTH) | Basic Filtering | `df_name_seven` uses LENGTH(name) = 7 | ✅ |
| 3 | Step 3: name, mass with mass <= 1.00 | Advanced Filtering | `df_mass` | ✅ |
| 4 | Step 4: all columns, >=1 moon AND mass < 1.00 | Advanced Filtering (AND) | `df_mass_moon` (Mars) | ✅ |
| 5 | Step 5: name, color LIKE '%blue%' | Advanced Filtering (LIKE) | `df_blue` (Earth, Uranus, Neptune) | ✅ |
| 6 | Step 6: hungry dogs name/age/breed youngest -> oldest | Ordering and Limiting | `df_hungry` ORDER BY age ASC | ✅ |
| 7 | Step 7: hungry dogs aged 2-7, name/age/hungry, alphabetical | Ordering and Limiting | `df_hungry_ages` BETWEEN + ORDER BY name | ✅ |
| 8 | Step 8: 4 oldest dogs name/age/breed sorted by breed | Ordering and Limiting (LIMIT) | `df_4_oldest` subquery ORDER BY age DESC LIMIT 4, re-sorted by breed | ✅ |
| 9 | Step 9: total years played (aggregate, no GROUP BY) | Aggregation | `df_ruth_years` = 22 | ✅ |
| 10 | Step 10: total HR | Aggregation | `df_hr_total` = 714 | ✅ |
| 11 | Step 11: team + number_years | Grouping and Aggregation | `df_teams_years` GROUP BY team | ✅ |
| 12 | Step 12: teams averaging >200 at bats, alias average_at_bats, HAVING | Grouping and Aggregation (HAVING) | `df_at_bats` | ✅ |
| 13 | Executes top to bottom | AutoTests | nbconvert --execute passed | ✅ |
