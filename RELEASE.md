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

Make sure that the tree looks good:

```sh
git log --graph --oneline --all -n 5
```

Push it:

```sh
git push origin master
git push origin v$VERSION
```

Done. In repositories that use this template, update to the new version using
for example the following command (for more information, check the
[Copier documentation](https://copier.readthedocs.io/en/stable/updating/)):

```sh
copier update --defaults
```
