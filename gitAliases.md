## Alias!

No not the [show](https://en.wikipedia.org/wiki/Alias_(TV_series)) that ran from 2001 until 2006, directed by Abrams...with Jennifer Garner in it. Definitely not that one.

I'm particularly ~~talking~~ writing about using an `alias` to shorten down commonly used Git commands to save you some time. The great thing about this is that you can do this Globally on your machine, or if you are like me and work across multiple devices, send your `.gitconfig` file to a repo and use that as a template for future device usage so you never have to remember what you set up before. 🕹 Magic! Think of it like when you were a teenager, and short-text was a thing...but for productivity!📦↗

### Quick breakdown/context:

Say for example you are always doing the following:
* `git add .` to add all chenged files to the stagin area
* then we do our normal `git commit -m "meaningful message 🎀"` to add some context to what the commit is
* and finally a `git push` or _other_ to send your code up to the repo

That's great, nice and dandy and most likely doesn't take longer then a few seconds if even that as soon as you have some confidence and understanding of the pseudo-science of Git.👾But what if we could shorten those commands down, or even chain a few of them together? 🤔 Now wouldn't that be dandy!? But let's start smaller, how do we even set up an alias?

> Disclaimer: Chaing git methods coming in future article🔗🔗

### Setup

Take `git init`, it's already small, but it can be smaller. And it's a good one to use as an example.😅Why not just make this command be `git i`; we've lost three letters in the mix. And to make that happen, open up your terminal and type this (or copy/paste):

```
git config --global alias.i 'init'
```

Broken down, that command is telling your locally installed git to:
* go to the config file, `git config`
* make this a global asset/command for the current user on your machine, `--global`
* setup an alias of "*_i_*", `alias.i` <--- notice this is the `alias` keyword first, followed by the dot, then the alias address itself
* and replace the normal command of `init` and that command is surrounded in quotes

Phew! Take a breath, muse over that a few times.... 🎓 you've now just taken an absolutely arbitrary command that initialises a local repository, and made it even shorter.😂👏 But that's only the beginning.😈

Replicate the above as many times as you feel necessary. We are in the realm of making time where time is hard to come by. And starting small, can sometimes be the biggest wins. Take note of your most used commands, and shorten them down. 🤏

Want a quick example of something even longer? Sure thing 🎉
`git push --set-upstream origin <branch-name>` <-- this one in particular was enough to send me over the edge a few times when racing against the clock to get a feature/ticket over the hurdle!

It could just be... `git su <branch-name>`, or "git set upstream to this branch, please" in pseudo-speak. And to make that happen, we just:

```
git config --global alias.su 'push --set-upstream origin'
```

And from that moment on, whenever you need to track the direction of a workflow to a new branch, you can just do `git su fantastic-new-branch`. Unfortunately, I have no idea how to shorten down branch names conditionally in an Alias command (and I'm sure that much doesn't yet exist anyway 😆).🌳

#### Extra tip:

_Want to see what's in your config file already, or maybe where it is on your machine?_

`git config --global --list --show-origin` should do the trick 😉 Try it!