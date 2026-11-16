# Mosquito Data Analysis Notebook (*Aedes aegypti*)

**Author:** Jillian Higbee

A Jupyter notebook that merges, summarizes and visualizes experimental data from a wet-lab study on *Aedes aegypti* mosquitoes: development time, mortality and sex ratio across genotypes and larval densities.

This was my first coding project, done during my transition from wet-lab biology into computational analysis. It is shared as a **code sample**. The data and results are not published here, and the notebook's saved outputs are cleared.

## What the code does

1. **Load and merge:** read trial and key sheets from an Excel workbook and merge each trial with its blind-ID key using pandas.
2. **Summarize:** a function groups the data by genotype and density and computes average pupation day, average emergence day, mortality and male-to-female sex ratio.
3. **Visualize:** matplotlib and seaborn charts for each trial, plus an exploratory joint plot of larval counts over time.

## Skills practiced

- Structuring and cleaning experimental data in pandas (merges, group-by summaries, reshaping)
- Writing a reusable analysis function and looping it over multiple trials
- Plotting with matplotlib and seaborn
- Working in Jupyter notebooks

## Limitations

- Exploratory analysis only, with no statistical tests or error bars.
- Average pupation and emergence day are unweighted means of the days on which any pupae or adults were recorded.
- The notebook cannot be run without the original workbook. See [`data/README.md`](data/README.md) for the expected format.

## Run it

1. Put a workbook with the expected structure at `data/MosquitoDat.xlsx`.
2. Install the packages and open the notebook:

   ```bash
   pip install -r requirements.txt
   jupyter lab
   ```

3. Open `notebooks/mosquito_analysis.ipynb` and run all cells.

## Repository structure

```
.
├── data/
│   └── README.md                # expected data format (data not included)
├── notebooks/
│   └── mosquito_analysis.ipynb  # analysis code, outputs cleared
├── requirements.txt
└── README.md
```

## Relevance to bioinformatics

This project was the starting point of my move from wet-lab biology to computational biology. It led to my later work in Python, Linux, RNA-seq analysis and protein structure analysis.
