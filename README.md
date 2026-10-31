# Weekly Fedora 44 & 45 KDE Builds
![GitHub all releases](https://img.shields.io/github/downloads/veuxit/daily-fedora-builds/total)
![GitHub release (latest by date)](https://img.shields.io/github/v/release/veuxit/daily-fedora-builds) [![Build Fedora 44 & 45 KDE ISO](https://github.com/veuxit/daily-fedora-builds/actions/workflows/build.yaml/badge.svg)](https://github.com/veuxit/daily-fedora-builds/actions/workflows/build.yaml)

In this repo, Github Actions runner builds weekly (every Tuesday) Fedora 44 & 45 KDE ISO with latest packages at 00.00 UTC. [Check releases for builds.](https://github.com/veuxit/daily-fedora-builds/releases)

# How to get ISO?
On Linux systems, download .isoaa and .isoab files from [releases tab](https://github.com/veuxit/daily-fedora-builds/releases) then run this:

~~~
cat Fedora.x86_64-44.isoaa Fedora.x86_64-44.isoab > Fedora.x86_64-44.iso
~~~
On Windows systems, run this instead(cmd):
~~~
copy /b Fedora.x86_64-44.isoaa + Fedora.x86_64-44.isoab Fedora.x86_64-44.iso
~~~
or replace 44 with 45 according to files you downloaded
#### Note that you should be in the same directory as files you downloaded

You will get the Fedora.x86_64-44.iso file with sha256sum from CHECKSUM_f44.txt file

#### Why split into two files? 
GitHub Releases file limit is only 2GB, while Fedora KDE ISO size is nearly 3.5GB

Fedora 44 & 45 KDE ISOs in here are probably same with official releases but updated packages. ISOs are built with kiwi. You can check [actions](https://github.com/veuxit/daily-fedora-builds/actions) page for build output, or [workflow file](.github/workflows/build.yaml) for build stages.
