# Youtube-DL automated Gentoo overlay

## Description

**WARNING**: This overlay is **experimental**.

This overlay is designed to offer latest stable Youtube-DL version as soon as possible.

For this to be possible, it is necessary that this overlay is automated.

A cron script is run every hour to update this overlay if a new version is available.

## Installation

### with `app-eselect/eselect-repository`
```
eselect repository add youtube-dl git https://github.com/CaseOf/youtube-dl-overlay.git
```

### via `/etc/portage/repos.conf/youtube-dl.conf`
```
[youtube-dl]
location = /path/to/youtube-dl-overlay
sync-type = git
sync-uri = https://github.com/CaseOf/youtube-dl-overlay.git
```

## Signature

Even if this repository is automated, commits are still signed.
When doing commits manually, my own PGP key is used.
When the script is committing new Youtube-DL versions, it signs with its PGP key.
