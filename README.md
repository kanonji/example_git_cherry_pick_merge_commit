```
$ git log --all --graph --oneline --decorate
*   88f95d2 (origin/dev, dev) Merge branch 'fix' into dev
|\
| * 08f352b (origin/fix, fix) 3fix
| * 47ba60c 2fix
| * f0247eb 1fix
|/
| * 303443b (HEAD, origin/master, master) 9master
|/
* f4209b4 init
```

```
$ git checkout master
$ git show dev
commit 88f95d25770fb192233fc7fbec0ea18430c91280
Merge: f4209b4 08f352b
Author: kanonji <kanonji@users.noreply.github.com>
Date:   Tue May 12 19:52:22 2015 +0900

    Merge branch 'fix' into dev

$ git cherry-pick -m 1 88f95d25770fb192233fc7fbec0ea18430c91280
[master d7d90e5] Merge branch 'fix' into dev
 1 file changed, 3 insertions(+), 3 deletions(-)
```

```
$ git log --all --graph --oneline --decorate
 * d7d90e5 (HEAD, master) Merge branch 'fix' into dev
 * 303443b (origin/master) 9master
 | *   88f95d2 (origin/dev, dev) Merge branch 'fix' into dev
 | |\
 |/ /
 | * 08f352b (origin/fix, fix) 3fix
 | * 47ba60c 2fix
 | * f0247eb 1fix
 |/
 * f4209b4 init
```
