# Merge Upstream Changes

```
git fetch upstream
git checkout ubc
git merge upstream/master

```

# Sync missing files from Contrib

We only need to bring the missing files from Contrib/UBC to OpenProblemLibrary/UBC. No overwrite. All other changes should come from upstream. Never merge UBC back to master.
```
rsync -a -v --ignore-existing Contrib/UBC OpenProblemLibrary/

```
