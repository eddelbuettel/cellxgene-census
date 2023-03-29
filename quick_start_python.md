```python
import cell_census
census = cell_census.open_soma()
adata = cell_census.get_anndata(
    census=census,
    organism="Homo sapiens",
    var_value_filter="feature_id in ['ENSG00000161798', 'ENSG00000188229']",
    obs_value_filter="cell_type == 'B cell' and disease == 'COVID-19'",
)

# AnnData object with n_obs × n_vars = 481155 × 2
# From more than 10 datasets
```
