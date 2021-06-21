# dotfiles

You're probably looking for [wincent/wincent](https://github.com/wincent/wincent).

## Details

I started [my dotfiles repo](https://github.com/wincent/wincent) back in 2009 and called it `wincent`, in part because I knew it would eventually contain much more than just "dotfiles".

GitHub has since added some features that rely on a `dotfiles` repo under your user to do special things automatically: for example a `$USER/dotfiles` repo containing a `script/setup` script (or one of several other names) can be used to [customize a Codespaces environment](https://docs.github.com/en/codespaces/setting-up-your-codespace/personalizing-codespaces-for-your-account#dotfiles).

So, the purpose of this repo is:

1. To serve as a pointer towards [wincent/wincent](https://github.com/wincent/wincent) for human beings.
2. To serve as a wrapper around the _real dotfiles_ for GitHub tools like Codespaces.

To that end, this repo incorporates the other one via a submodule reference, and contains [some scripts](script) that run in the Codespaces environment in order to do set-up.

## Addendum

Speaking of "convention over configuration", GitHub also treats a repo at `$USER/$USER` as special. If it contains a README file, the contents of that file will be used to [customize your profile](https://docs.github.com/en/github/setting-up-and-managing-your-github-profile/customizing-your-profile/managing-your-profile-readme).

I did think about using GitHub's rename tool to rename `wincent/wincent` to `wincent/dotfiles`, and that would at least mean that any URLs out there pointing at the former would continue to work (via redirects), but if I ever want to put up a profile README that will mean creating a new repo at `wincent/wincent`, at which point all the redirects will stop working. So, for now, using this repo as a wrapper is the workaround I'm going with.
