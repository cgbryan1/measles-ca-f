# California data source

The state and county tables in `data/` were copied from the `main` branch of
[`cgbryan1/carol-measles-CA`](https://github.com/cgbryan1/carol-measles-CA):

- `public/data/states.csv` → `data/state.csv`
- `public/data/states/ca.csv` → `data/counties.csv`

The CSV contents, including all measurement values, were copied unchanged.
`data/schools.csv` contains only the required header because the source
repository has no school-level table; the receiving repository permits this
when school data is unavailable.

The `sourceUrl` and `sourceLabel` in `data/meta.json` use the attribution
provided for this submission: the dashboard's `dev` branch public data
directory, labeled `measles-dashboard`.

Coverage values remain as supplied and are interpreted as proportions under
the receiving schema. The source columns include K–5 estimates. The source
files do not state the reporting period, target population, MMR dose,
suppression rules, or whether the estimates are reported or modeled; these
details are not inferred.
