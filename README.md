Suckless DWM with patches.

One branch for each patch:

1 Fake fullscreen
2 PerTag
3 NoBorder
4 MoveStack
5 Fullscreen
6 ... and a Config Branch

## Building DWM
dwm can be built using the script `suckmerge` or alternativly:
```
For each branch:
git merge BRANCH_NAME -m BRANCH_NAME
make && sudo make clean install
```

Then restart dwm.

## Adding new patches
To add a new patch download the diff from https://dwm.suckless.org and:
```
[CLEANUP MASTER FIRST!]
git checkout -b NAME_OF_FEATURE
git apply /path/to/dwm-PATCH.diff
git add -a
git commit -m "Applied patch PATCH"
```
