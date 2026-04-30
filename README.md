# Daily Fedora 43 & 44 KDE Builds
![GitHub all releases](https://img.shields.io/github/downloads/veuxit/daily-fedora-builds/total)
![GitHub release (latest by date)](https://img.shields.io/github/v/release/veuxit/daily-fedora-builds)

In this repo, Github Actions runner builds daily Fedora 43 & 44 KDE ISO with latest packages at 00.00 UTC. [Check releases for builds.](https://github.com/veuxit/daily-fedora-builds/releases)

# How to get ISO?
On Linux systems, download .isoaa and .isoab files from [releases tab](https://github.com/veuxit/daily-fedora-builds/releases) then run this:

~~~
cat Fedora.x86_64-43.isoaa Fedora.x86_64-43.isoab > Fedora.x86_64-43.iso
~~~
On Windows systems, run this instead(cmd):
~~~
copy /b Fedora.x86_64-43.isoaa + Fedora.x86_64-43.isoab Fedora.x86_64-43.iso
~~~
or replace 43 with 44 according to files you downloaded
#### Note that you should be in the same directory as files you downloaded

You will get the Fedora.x86_64-43.iso file with sha256sum from CHECKSUM_f43.txt file

#### Why split into two files? 
GitHub Releases file limit is only 2GB, while Fedora KDE ISO size is over 3.5GB

Fedora 43 & 44 KDE ISOs in here are probably same with official releases but updated packages. ISOs are built with kiwi. You can check [actions](https://github.com/veuxit/daily-fedora-builds/actions) page for build output, or [workflow file](.github/workflows/build.yaml) for build stages.
