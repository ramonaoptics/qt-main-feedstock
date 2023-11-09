About qt-main-feedstock
=======================

Feedstock license: [BSD-3-Clause](https://github.com/ramonaoptics/qt-main-feedstock/blob/main/LICENSE.txt)

Home: https://qt.io

Package license: LGPL-3.0-only

Summary: Qt is a cross-platform application and UI framework.

Development: https://github.com/qt

Documentation: https://doc.qt.io/

Qt helps you create connected devices, UIs & applications that run
anywhere on any device, on any operating system at any time.


Current build status
====================


<table><tr>
    <td>Travis</td>
    <td>
      <a href="https://app.travis-ci.com/ramonaoptics/qt-main-feedstock">
        <img alt="linux" src="https://img.shields.io/travis/com/ramonaoptics/qt-main-feedstock/main.svg?label=Linux">
      </a>
    </td>
  </tr>
    
  <tr>
    <td>Azure</td>
    <td>
      <details>
        <summary>
          <a href="https://dev.azure.com/ramonaoptics/feedstock-builds/_build/latest?definitionId=&branchName=main">
            <img src="https://dev.azure.com/ramonaoptics/feedstock-builds/_apis/build/status/qt-main-feedstock?branchName=main">
          </a>
        </summary>
        <table>
          <thead><tr><th>Variant</th><th>Status</th></tr></thead>
          <tbody><tr>
              <td>linux_64</td>
              <td>
                <a href="https://dev.azure.com/ramonaoptics/feedstock-builds/_build/latest?definitionId=&branchName=main">
                  <img src="https://dev.azure.com/ramonaoptics/feedstock-builds/_apis/build/status/qt-main-feedstock?branchName=main&jobName=linux&configuration=linux%20linux_64_" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>linux_aarch64</td>
              <td>
                <a href="https://dev.azure.com/ramonaoptics/feedstock-builds/_build/latest?definitionId=&branchName=main">
                  <img src="https://dev.azure.com/ramonaoptics/feedstock-builds/_apis/build/status/qt-main-feedstock?branchName=main&jobName=linux&configuration=linux%20linux_aarch64_" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>linux_ppc64le</td>
              <td>
                <a href="https://dev.azure.com/ramonaoptics/feedstock-builds/_build/latest?definitionId=&branchName=main">
                  <img src="https://dev.azure.com/ramonaoptics/feedstock-builds/_apis/build/status/qt-main-feedstock?branchName=main&jobName=linux&configuration=linux%20linux_ppc64le_" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>osx_64</td>
              <td>
                <a href="https://dev.azure.com/ramonaoptics/feedstock-builds/_build/latest?definitionId=&branchName=main">
                  <img src="https://dev.azure.com/ramonaoptics/feedstock-builds/_apis/build/status/qt-main-feedstock?branchName=main&jobName=osx&configuration=osx%20osx_64_" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>osx_arm64</td>
              <td>
                <a href="https://dev.azure.com/ramonaoptics/feedstock-builds/_build/latest?definitionId=&branchName=main">
                  <img src="https://dev.azure.com/ramonaoptics/feedstock-builds/_apis/build/status/qt-main-feedstock?branchName=main&jobName=osx&configuration=osx%20osx_arm64_" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>win_64</td>
              <td>
                <a href="https://dev.azure.com/ramonaoptics/feedstock-builds/_build/latest?definitionId=&branchName=main">
                  <img src="https://dev.azure.com/ramonaoptics/feedstock-builds/_apis/build/status/qt-main-feedstock?branchName=main&jobName=win&configuration=win%20win_64_" alt="variant">
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
| [![Conda Recipe](https://img.shields.io/badge/recipe-qt--main-green.svg)](https://anaconda.org/ramonaoptics/qt-main) | [![Conda Downloads](https://img.shields.io/conda/dn/ramonaoptics/qt-main.svg)](https://anaconda.org/ramonaoptics/qt-main) | [![Conda Version](https://img.shields.io/conda/vn/ramonaoptics/qt-main.svg)](https://anaconda.org/ramonaoptics/qt-main) | [![Conda Platforms](https://img.shields.io/conda/pn/ramonaoptics/qt-main.svg)](https://anaconda.org/ramonaoptics/qt-main) |

Installing qt-main
==================

Installing `qt-main` from the `ramonaoptics` channel can be achieved by adding `ramonaoptics` to your channels with:

```
conda config --add channels ramonaoptics
conda config --set channel_priority strict
```

Once the `ramonaoptics` channel has been enabled, `qt-main` can be installed with `conda`:

```
conda install qt-main
```

or with `mamba`:

```
mamba install qt-main
```

It is possible to list all of the versions of `qt-main` available on your platform with `conda`:

```
conda search qt-main --channel ramonaoptics
```

or with `mamba`:

```
mamba search qt-main --channel ramonaoptics
```

Alternatively, `mamba repoquery` may provide more information:

```
# Search all versions available on your platform:
mamba repoquery search qt-main --channel ramonaoptics

# List packages depending on `qt-main`:
mamba repoquery whoneeds qt-main --channel ramonaoptics

# List dependencies of `qt-main`:
mamba repoquery depends qt-main --channel ramonaoptics
```




Updating qt-main-feedstock
==========================

If you would like to improve the qt-main recipe or build a new
package version, please fork this repository and submit a PR. Upon submission,
your changes will be run on the appropriate platforms to give the reviewer an
opportunity to confirm that the changes result in a successful build. Once
merged, the recipe will be re-built and uploaded automatically to the
`ramonaoptics` channel, whereupon the built conda packages will be available for
everybody to install and use from the `ramonaoptics` channel.
Note that all branches in the ramonaoptics/qt-main-feedstock are
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

* [@Tobias-Fischer](https://github.com/Tobias-Fischer/)
* [@andfoy](https://github.com/andfoy/)
* [@ccordoba12](https://github.com/ccordoba12/)
* [@duncanmmacleod](https://github.com/duncanmmacleod/)
* [@gillins](https://github.com/gillins/)
* [@jschueller](https://github.com/jschueller/)
* [@matthiasdiener](https://github.com/matthiasdiener/)
* [@mingwandroid](https://github.com/mingwandroid/)
* [@msarahan](https://github.com/msarahan/)
* [@ocefpaf](https://github.com/ocefpaf/)
* [@stuarteberg](https://github.com/stuarteberg/)

