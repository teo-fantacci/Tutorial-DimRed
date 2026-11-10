# Dimensionality reduction on neural data: a hands-on tutorial

A single Jupyter notebook ([`DimRed_tutorial.ipynb`](DimRed_tutorial.ipynb)) that takes real
multi-electrode recordings from preprocessing to visualisation and applies six dimensionality
reduction methods side by side: **PCA, Isomap, ICA, factor analysis, locally linear embedding and
linear discriminant analysis**. It then compares the methods, evaluates time-delay embedding, and
builds peri-stimulus mean trajectories in each reduced space. Every section ends with questions to
discuss, so it works for self-study or a classroom session.

**For whom:** students and researchers who know basic Python and NumPy and want a practical
introduction to dimensionality reduction on spiking data.

## Data

The notebook uses one session, `indy_20160930_05.mat`, from

> O'Doherty, J. E., Cardoso, M. M. B., Makin, J. G. & Sabes, P. N. *Nonhuman Primate Reaching with
> Multichannel Sensorimotor Cortex Electrophysiology.* Zenodo (2020).
> [doi:10.5281/zenodo.3854034](https://doi.org/10.5281/zenodo.3854034). License: CC-BY-4.0.

Download that file from the Zenodo record and put it in a `data/` folder next to the notebook.
The data are not stored in this repository.

## How to run

With conda:

```bash
conda env create -f environment.yml
conda activate dimred_tutorial
```

Or with pip, in a Python 3.8 environment:

```bash
pip install -r requirements.txt
```

Then open `DimRed_tutorial.ipynb` in VS Code or Jupyter and run the cells in order. Intermediate
results and figures are written to `processing_folder/`, `results_dim_reduction/` and
`psth_plots/`, which git ignores.

## License

The code is released under the [MIT License](LICENSE). The dataset belongs to its authors and is
distributed by them under CC-BY-4.0; please cite it if you use it.
