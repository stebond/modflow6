# Notice on this fork (FULL_3D DISU extension)

This repository is an **unofficial fork** of the MODFLOW 6 source code
([MODFLOW-ORG/modflow6](https://github.com/MODFLOW-ORG/modflow6)).
It adds a `FULL_3D` option to the DISU package, so that fully unstructured 3D
grids (for example 3D Voronoi grids, where each cell is a polyhedron) can be
used, together with native VTU output of the geometry and results.

## Non-affiliation

* This fork is **not** maintained, reviewed, approved or endorsed by the
  U.S. Geological Survey (USGS), by the MODFLOW development team or by the
  U.S. Government.
* The USGS and the U.S. Government are not responsible for this modified
  version, and no support for it should be requested from them.
* The modifications are provided for research and verification purposes and
  have not received any USGS approval. Official MODFLOW 6 releases are
  available only from the
  [USGS MODFLOW and Related Programs page](https://water.usgs.gov/ogw/modflow/MODFLOW.html).
* The name "MODFLOW" is used here only to identify the original software on
  which this work is based.

## License and disclaimer

The original MODFLOW 6 files keep their original public-domain status and the
original [LICENSE.md](LICENSE.md) and [DISCLAIMER.md](DISCLAIMER.md), which are
unchanged and apply to this fork as well. The modified and added files are
released under the same terms. The software is provided "as is", without
warranty of any kind.

## Scope of the modification

* Based on MODFLOW 6 `develop` (version 6.9.0.dev0, commit `6565dc81`).
* The changes are limited to the DISU discretization and to the packages
  needed to use it (see the commit history of branch `full3d-disu`).
* Classic DISU, DIS and DISV models are not affected.
* Tests: `autotest/test_gwf_disu_full3d.py`, `test_gwf_disu_full3d_ext.py`,
  `test_gwf_disu_full3d_vtu.py`. The complete upstream test suite passes on this
  branch (1223 passed, 0 failed; skipped tests need the optional `--netcdf` and
  `--parallel` options).

## How to cite

If this work is used, please cite the associated paper and the archived
version of this repository:

* Bonduà, S. (2026). *[Title of the paper, to be inserted].* [Journal, to be inserted].
* Bonduà, S. (2026). MODFLOW 6 with FULL_3D DISU option for fully unstructured
  3D grids (unofficial fork), version v0.1.0-full3d (software). Zenodo.
  https://doi.org/10.5281/zenodo.24495201

The original program should be cited as well, as indicated in
[CITATION.cff](CITATION.cff) and in the
[MODFLOW 6 documentation](https://water.usgs.gov/ogw/modflow/MODFLOW.html).

## Contact

Stefano Bonduà, Department of Civil, Chemical, Environmental and Materials
Engineering (DICAM), University of Bologna.
