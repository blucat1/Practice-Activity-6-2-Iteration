# Practice Activity 6.2: Iteration

Completed solutions to all eight exercises in `GSB_5544_Practice_Activity_6_2_Iteration.ipynb`.

- [Completed notebook](GSB_5544_Practice_Activity_6_2_Iteration.ipynb)
- [Rendered notebook](GSB_5544_Practice_Activity_6_2_Iteration.html)

The notebook covers verse lists, scalar and vectorized conditional square roots, multiple-iterable `map()`, lambda functions, row-wise penguin classification, and category counts. It preserves the original exercise prompts and includes explanations and assertions for strict thresholds, fractional roots, shorter map inputs, and missing penguin data.

## Run

Use Python 3.11 or newer (validated with Python 3.14.6):

```bash
python3 -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
python -m ipykernel install --user --name pa-6-2 --display-name "Practice Activity 6.2"
python -m jupyter lab
```

Open the notebook, select the **Practice Activity 6.2** kernel, and select **Run → Run All Cells**. The `palmerpenguins` package includes the dataset, so the notebook does not download data at runtime.

To execute without opening Jupyter:

```bash
python -m jupyter nbconvert --to notebook --execute --inplace \
  --ExecutePreprocessor.kernel_name=pa-6-2 \
  GSB_5544_Practice_Activity_6_2_Iteration.ipynb
```

The `setuptools` compatibility pin supports the legacy resource loader used by `palmerpenguins`. See the [Setuptools documentation](https://setuptools.pypa.io/en/stable/deprecated/pkg_resources.html).

## Notes

- The first song examples follow the course chapter's range of 100, 99, and 98.
- Zero and negative values are unchanged by both square-root functions.
- `map()` stops at the shortest iterable.
- Every penguin receives a label; missing information does not qualify a penguin for a rule requiring that information.
- The label `Average Adelie:` includes the trailing colon exactly as quoted in the prompt.
- The Dainty Daisy rule uses `flipper_length_mm < 0.05 * body_mass_g` as stated in the activity.

Reference: [course textbook, Iteration](https://ds-ml-with-python.github.io/Course-Textbook/06-iteration.html).
