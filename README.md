About qupath-feedstock
======================

Feedstock license: [BSD-3-Clause](https://github.com/sdvillal/qupath-feedstock/blob/master/LICENSE.txt)

Home: https://qupath.github.io/

Package license: GPLv3

Summary: QuPath is an open, powerful, flexible, extensible software platform for whole slide image analysis.

Current build status
====================


<table>
    
  <tr>
    <td>Azure</td>
    <td>
      <details>
        <summary>
          <a href="https://dev.azure.com/sdvillal/feedstock-builds/_build/latest?definitionId=2&branchName=master">
            <img src="https://dev.azure.com/sdvillal/feedstock-builds/_apis/build/status/qupath-feedstock?branchName=master">
          </a>
        </summary>
        <table>
          <thead><tr><th>Variant</th><th>Status</th></tr></thead>
          <tbody><tr>
              <td>linux_64</td>
              <td>
                <a href="https://dev.azure.com/sdvillal/feedstock-builds/_build/latest?definitionId=2&branchName=master">
                  <img src="https://dev.azure.com/sdvillal/feedstock-builds/_apis/build/status/qupath-feedstock?branchName=master&jobName=linux&configuration=linux%20linux_64_" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>osx_64</td>
              <td>
                <a href="https://dev.azure.com/sdvillal/feedstock-builds/_build/latest?definitionId=2&branchName=master">
                  <img src="https://dev.azure.com/sdvillal/feedstock-builds/_apis/build/status/qupath-feedstock?branchName=master&jobName=osx&configuration=osx%20osx_64_" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>win_64</td>
              <td>
                <a href="https://dev.azure.com/sdvillal/feedstock-builds/_build/latest?definitionId=2&branchName=master">
                  <img src="https://dev.azure.com/sdvillal/feedstock-builds/_apis/build/status/qupath-feedstock?branchName=master&jobName=win&configuration=win%20win_64_" alt="variant">
                </a>
              </td>
            </tr>
          </tbody>
        </table>
      </details>
    </td>
  </tr>
</table>

Current release info
====================

| Name | Downloads | Version | Platforms |
| --- | --- | --- | --- |
| [![Conda Recipe](https://img.shields.io/badge/recipe-qupath-green.svg)](https://anaconda.org/sdvillal/qupath) | [![Conda Downloads](https://img.shields.io/conda/dn/sdvillal/qupath.svg)](https://anaconda.org/sdvillal/qupath) | [![Conda Version](https://img.shields.io/conda/vn/sdvillal/qupath.svg)](https://anaconda.org/sdvillal/qupath) | [![Conda Platforms](https://img.shields.io/conda/pn/sdvillal/qupath.svg)](https://anaconda.org/sdvillal/qupath) |

Installing qupath
=================

Installing `qupath` from the `sdvillal` channel can be achieved by adding `sdvillal` to your channels with:

```
conda config --add channels sdvillal
conda config --set channel_priority strict
```

Once the `sdvillal` channel has been enabled, `qupath` can be installed with `conda`:

```
conda install qupath
```

or with `mamba`:

```
mamba install qupath
```

It is possible to list all of the versions of `qupath` available on your platform with `conda`:

```
conda search qupath --channel sdvillal
```

or with `mamba`:

```
mamba search qupath --channel sdvillal
```

Alternatively, `mamba repoquery` may provide more information:

```
# Search all versions available on your platform:
mamba repoquery search qupath --channel sdvillal

# List packages depending on `qupath`:
mamba repoquery whoneeds qupath --channel sdvillal

# List dependencies of `qupath`:
mamba repoquery depends qupath --channel sdvillal
```




Updating qupath-feedstock
=========================

If you would like to improve the qupath recipe or build a new
package version, please fork this repository and submit a PR. Upon submission,
your changes will be run on the appropriate platforms to give the reviewer an
opportunity to confirm that the changes result in a successful build. Once
merged, the recipe will be re-built and uploaded automatically to the
`sdvillal` channel, whereupon the built conda packages will be available for
everybody to install and use from the `sdvillal` channel.
Note that all branches in the sdvillal/qupath-feedstock are
immediately built and any created packages are uploaded, so PRs should be based
on branches in forks and branches in the main repository should only be used to
build distinct package versions.

In order to produce a uniquely identifiable distribution:
 * If the version of a package **is not** being increased, please add or increase
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string).
 * If the version of a package **is** being increased, please remember to return
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string)
   back to 0.

Feedstock Maintainers
=====================

* [@sdvillal](https://github.com/sdvillal/)

