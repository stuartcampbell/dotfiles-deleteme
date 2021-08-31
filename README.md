# Stuart's dotfiles and associated junk

These are my dotfiles, they are managed using [`chezmoi`](https://www.chezmoi.io).

Secrets are stored in [1Password](https://1password.com/), and so we need the 
[1Password CLI](https://support.1password.com/command-line-getting-started/) installed.

Login to 1Password for the first time with:

    eval $(op signin <subdomain>.1password.com <email>)

Then, to login afterwards, run:

    eval $(op signin)

Install them with:

    chezmoi init stuartcampbell

