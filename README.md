# GDS FakeNewsProject
Students: Lasse Helmer Larsen (rmj762), Oskar Thorvald Andersen (grf587) og Valdemar Kragh (lnk952)

To get our environment use:
```
conda env create -f environment.yml
```

### If something is updated in the venv, we should use to update:

conda env export --from-history > environment.yml

### After pulling, to update the environment use:

conda env update -f environment.yml --prune