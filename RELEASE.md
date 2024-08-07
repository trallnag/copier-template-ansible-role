# Release

This document describes the release process and is targeted at maintainers.

Check the existing tags:

```sh
git tag
```

Pick the next version:

```sh
VERSION=8
```

Create the new tag:

```sh
git tag -s v$VERSION -m ""
```

Push it:

```sh
git push origin master
git push origin v$VERSION
```
