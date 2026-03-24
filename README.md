# scripts

This repo contains a random collection of scripts that **I have written** over the years, that I'm happy enough with to share with the world.

I also have a non-public scripts repo, where I've been gathering scripts from everywhere I've stored them over the years. I still need to go through and clean these up, but once they're ready I plan to move them to this repo.

The scripts in *this* repo are all released under open-source licenses - mostly MIT, but each script should contain an explicit license statement in the script itself.

## &#x1F6D1; Github is a secondary server

If you're seeing this on Github, be aware that you're looking at a *backup copy* of the actual scripts repo. On my workstations where I have this repo cloned, the list of remotes looks like this:

```
$ git remote -v
origin  foks://SERVER/t:TEAM/scripts-public (fetch)
origin  foks://SERVER/t:TEAM/scripts-public (push)
origin  git@github.com:kg4zow/scripts (push)
```

This means that ...

* When I run `git fetch` or `git pull`, it pulls from [FOKS](https://foks.pub/).
* When I run `git push`, it pushes to FOKS *and* Github.

I'm planning to add a page on [jms1.info](https://jms1.info/) which explains how to do this. Until I write that page, the short version is:

```
git remote remove origin
git remote add origin foks://SERVER/t:TEAM/scripts-public
git remote set-url --add --push origin foks://SERVER/t:TEAM/scripts-public
git remote set-url --add --push origin git@github.com:kg4zow/scripts
```

**Because Github is a *secondary* server, pull requests are disabled for this repo.** If you find anything in this repo that you think needs to be corrected, or if you've seen some of my other scripts and think they might belong here, please [open an issue](https://github.com/kg4zow/scripts/issues) and let me know.
