# About me

Contains repo manifest for HLOS (High Level Operating System).

# Install

```
#Debian/Ubuntu
$ sudo apt install repo

# Gentoo
$ sudo emerge dev-vcs/repo
```

Or install manually

```
$ curl https://storage.googleapis.com/git-repo-downloads/repo > ~/bin/repo
$ chmod +x ~/bin/repo
$ export PATH=$HOME/bin:$PATH
```

# Download codes

```
$ mkdir HLOS
$ cd HLOS
$ repo init -u https://github.com/aeroratech/manifest.git -b release -m LU.UM.3.3.1.r1-25900-QRB5165.0.xml --repo-url=https://gerrit-googlesource.proxy.ustclug.org/git-repo
$ repo sync -j $(nproc)
```

# Next steps

Apply patches, download non-HLOS components: XBL, cDSP/aDSP, CHI-CDK, CamX and so on.

# Build instructions

TODO
