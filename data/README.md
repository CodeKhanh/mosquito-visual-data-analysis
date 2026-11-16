# Data

The data are **not included** in this repository. They were collected in a research lab and are not published here.

To run the notebook, place an Excel workbook with the structure below at:

```
data/MosquitoDat.xlsx
```

## Expected structure

| Sheet | Contents |
|---|---|
| `Trial1`, `Trial2` | One row per container per day: `Trial Day`, `Blind ID`, `Density`, `Larvae Count`, `Pupae Emerged`, `# of Deceased`, `Mosquitoes Emerged`, `Males Emerged`, `Females Emerged` |
| `Key1`, `Key2` | Keys that map each `Blind ID` to its `Genotype` and `Density` |

Blind IDs are reused between trials, so each trial is merged with its own key.
