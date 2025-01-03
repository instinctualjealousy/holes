# 🕳️holes🕳️
[![Tests](https://github.com/instinctualjealousy/holes/actions/workflows/ci.yml/badge.svg)](https://github.com/instinctualjealousy/holes/actions/workflows/ci.yml)

Diggin', diggin'. Mostly holes. When I'm done, I buries them again all neat and tidy. With manifests, I do.<br />
This is a bucket (repository) for [Scoop](https://scoop.sh), the Windows command-line installer.<br />
<br />
The main point of this bucket is to handle all the programs I use that either still haven't had manifests made, or have manifests with outstanding issues that I fixed for my own personal use. I hope someone finds it of use!

How do I install this bucket?
---------------------------------

To add this bucket, run `scoop bucket add holes https://github.com/instinctualjealousy/holes`. To install applications from this bucket, do `scoop install holes\<app>` or simply `scoop install <app>` if it doesn't exist on any other claimed buckets.

Notes:
---------------------------------

* I will put notes in the manifests for programs that have first-run, cleanup, or persistence concerns that are beyond the scope of Scoop
* A few manifests do not have checkver/autoupdate routines due to being:
   * Unnecessary, as the software has not been maintained for years, or was a single-release that was never maintained
   * Difficult to implement, due to poor documentation or website design
* The rare manifest that doesn't have $version in URL or filename will result in hash fails when the referenced software is updated on server- if I don't keep up on updating the manifests, of course
* Some manifests point to mirrored and repacked archives because they aren't hosted anywhere easily accessible by scoop (check `mirror` directory)
