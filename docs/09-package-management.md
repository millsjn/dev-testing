---
title: Package Management
description: Learn how to install additional R and Python packages in the ADRF workspace.
order: 9
lastUpdated: 2026-03-31
---

# Adding Additional Packages in R/Python

The ADRF has an internal package repository, so users can install packages for R and Python themselves.

The repositories that are currently mirrored in the ADRF are [CRAN](https://cran.r-project.org/) for R packages and [PyPi.org](https://pypi.org/) for Python. There is currently no access to packages hosted on Github or other mirrors.

**Important Note**: If you are working in a shared workspace for a project, each user in the project must install the packages. There is no shared package installation for projects.

## Add Additional R Packages

To install R packages, simply use the code below and the package will be installed from the repository. You will not have to re-install the package again, and to use the package load it with the `library()` function.

```r
install.packages("packagename")
```

### Example: Installing tidyverse

```r
install.packages("tidyverse")
```

### Installing Specific Package Versions

To install a specific package version you can specify:

```r
install.packages("remotes")

remotes::install_version("tidyverse", "1.3.2")
```

**Recommendation**: We recommend starting R using RStudio for best results, instead of double-clicking on an R or Rmarkdown script.

## Add Additional Python Packages

Similar to R packages, Python packages may be installed using the Package Installer for Python (pip).

**Recommendation**: We recommend installing Python packages from the command line. 

If you start **JupyterLab**, choose the **Terminal tab**. Then install your package using pip. For example, to install the pandas package, type `pip install pandas`.

Then you may use the package within your Jupyter notebook as usual.

### Installing Specific Package Versions

To install a specific package version, type:

```python
pip install pandas==1.2.3
```

## Troubleshooting

### Package Not Found

If you receive an error that a package cannot be found:
- Verify the package name is spelled correctly
- Check that the package exists on CRAN (for R) or PyPI (for Python)
- Remember that GitHub-hosted packages are not accessible

### Permission Errors

If you encounter permission errors when installing packages:
- Ensure you're using the Terminal in JupyterLab for Python packages
- For R packages, ensure you're using RStudio
- Contact ADRF support if issues persist

### Package Version Conflicts

If you experience conflicts between package versions:
- Try installing specific versions known to be compatible
- Document your package versions for reproducibility
- Consider using virtual environments for Python projects

## Best Practices

1. **Document Your Dependencies**: Keep a list of all packages and versions you install
2. **Install Early**: Install necessary packages at the beginning of your project
3. **Test After Installation**: Verify packages work correctly after installation
4. **Coordinate with Team**: If working on a shared project, ensure all team members install the same package versions


<br>

---
# Support & Navigation

**Need help?**
- Email: support@coleridgeinitiative.org
- Hours: Monday-Friday, 9 AM - 5 PM ET

**Navigation**
- ⬅️ [Back to Home](../README.md)
