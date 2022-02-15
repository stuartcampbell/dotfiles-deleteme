# Stuart's dotfiles and associated junk

[![CI](https://github.com/stuartcampbell/dotfiles/actions/workflows/main.yml/badge.svg)](https://github.com/stuartcampbell/dotfiles/actions/workflows/main.yml)

These are my dotfiles, they are managed using [`chezmoi`](https://www.chezmoi.io).

Secrets are stored in [1Password](https://1password.com/), and so we need the 
[1Password CLI](https://support.1password.com/command-line-getting-started/) installed.

Login to 1Password for the first time with:

    eval $(op signin <subdomain>.1password.com <email>)

Then, to login afterwards, run:

    eval $(op signin)

Install them with:

    chezmoi init --apply https://github.com/stuartcampbell/dotfiles.git

Or to be a little more conservative:

    chezmoi init https://github.com/stuartcampbell/dotfiles.git
    
Look at what changes would be applied

    chezmoi diff
    
Now apply them

    chezmoi apply -v

