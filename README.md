# 🕳️holes🕳️
[![Tests](https://github.com/instinctualjealousy/holes/actions/workflows/ci.yml/badge.svg)](https://github.com/instinctualjealousy/holes/actions/workflows/ci.yml) [![Excavator](https://github.com/instinctualjealousy/holes/actions/workflows/excavator.yml/badge.svg)](https://github.com/instinctualjealousy/holes/actions/workflows/excavator.yml)

Diggin', diggin'. Mostly holes. When I'm done, I buries them again all neat and tidy. With manifests, I do.<br />
This is a bucket (repository) for [Scoop](https://scoop.sh), the Windows command-line installer.<br />
<br />
The main point of this bucket is to handle all the programs I use that either still haven't had manifests made, or have manifests with outstanding issues that I fixed for my own personal use. I hope someone finds it of use!

How do I install this bucket?
---------------------------------

To add this bucket, run `scoop bucket add holes https://github.com/instinctualjealousy/holes`. To install applications from this bucket, do `scoop install holes\<app>` or simply `scoop install <app>` if it doesn't exist on any other claimed buckets.

Notes:
---------------------------------

* Some manifests point to self-hosted URLs and connect with insecure HTTP (be sure to read JSONs so you know what you're doing)
* I will put notes in the manifests for programs that have first-run, cleanup, or persistence concerns that are beyond the scope of Scoop
* A few manifests do not have checkver/autoupdate routines due to being:
   * Unnecessary, as the software has not been maintained for years, or was a single-release that was never maintained
   * Difficult to implement, due to poor documentation or website design
* The rare manifest that doesn't have $version in URL or filename will result in hash fails when it's updated on server- that is, if I don't keep up on autoupdates as fast as possible
