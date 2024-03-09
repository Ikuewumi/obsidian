---
sticker: lucide//laptop
---

This documents some of the weirdest bugs I've seen and some tricks to fix it

## `Esc` key is equal to `Ctrl+[` 

Not really a bug, but something to note. In Linux it just so happens that the combination of the keys `Ctrl` and `[` gives the keycode for the `Esc` key, so just a tip for the future


## `Astro-lsp` doesn't work!

This one's actually pretty annoying, as at 2024-14-02, the astro-lsp on neovim dosen't work the only solution I found was to install a previous version 
```bash
:MasonInstall astro-language-server@1.0.8
```

Hope it's fixed soon

---
## Accessing WSL files with `\\wsl$`

As a windows user, you can access your WSL files in the files explorer by opening the path `\\wsl$`, from here, you should be able to navigate the machine securely, copy or paste files.

Useful for a state where one downloads a binary on the windows, but wants to use it on their WSL

---
##  Git Problems

```
remote: Enumerating objects: 17, done.
remote: Counting objects: 100% (17/17), done.
remote: Compressing objects: 100% (12/12), done.
remote: Total 12 (delta 10), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (12/12), 2.20 KiB | 451.00 KiB/s, done.
fatal: bad object refs/remotes/origin/main
error: https://github.com/Ikuewumi/medcross.git did not send all necessary objects
```

This error just popped out of nowhere, but here's how I fixed it...
I deleted the remote folder for that branch

```
rm -rf .git/refs/remotes/origin/<name of branch>
```

then I pulled again, and now all's good 🎉🎉

```
git pull
```

My response from `git pull`

```
From https://github.com/Ikuewumi/medcross
 * [new branch]      astro      -> origin/astro
 * [new branch]      main       -> origin/main
There is no tracking information for the current branch.
Please specify which branch you want to merge with.
See git-pull(1) for details.

    git pull <remote> <branch>

If you wish to set tracking information for this branch you can do so with:

    git branch --set-upstream-to=origin/<branch> main
```