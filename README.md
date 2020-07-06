[![Actions Status](https://github.com/brianferguson/auto-rmskin-package/workflows/auto-rmskin-package/badge.svg)](https://github.com/brianferguson/auto-rmskin-package/actions)

# auto-rmskin-package

This is a <ins>sample</ins> github action that creates an rmskin package and automatically uploads it to a github release. Simply create a tagged release and the github action will automatically create the rmskin and upload it the newly created release for you.

**Caution**: This script is NON-VALIDATING, meaning the folder structure is archived AS IS. Also, plugins are NOT checked for the correct bitness.

---

# How it works:

When a [release](https://github.com/brianferguson/auto-rmskin-package/releases/) is published, the github action will automatically start running. Using Powershell, the action will first archive the contents of the `RMSKIN` folder to a .zip file. Then the Rainmeter custom footer is written to the file. It then changes the extension of the .zip file to a .rmskin file. Then the .rmksin file is automatically uploaded to your previously created release as an asset.

This makes it really easy to make a few changes to your skin files, create a new release, and have the new .rmskin automatically created and uploaded for you.

#### Notes:

With this script, the folder structure needs to be exactly the same as how the Rainmeter rmskin packager does it. The folder `RMSKIN` contains an unzipped rmskin file previously created with Rainmeter.


# Links:
[Releases](https://github.com/brianferguson/auto-rmskin-package/releases/)
[Workflow](https://github.com/brianferguson/auto-rmskin-package/blob/master/.github/workflows/release.yml)
[Actions](https://github.com/brianferguson/auto-rmskin-package/actions/)
