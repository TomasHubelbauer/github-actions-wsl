# GitHub Actions WSL

GitHub Actions Windows images have WSL.

## To-Do

### Study actions/setup-wsl to see how it could be useful to me

https://github.com/marketplace/actions/setup-wsl

### Fix the issue with the kernel and figure out why "no installed distros"

The current workflow fails `wsl whoami` because thee is distro installed even
though `wsl --list --all` shows Ubuntu got installed correctyly.

Another issue I was facing was about the kernel with a link to this:
https://docs.microsoft.com/en-us/windows/wsl/install-manual#step-4---download-the-linux-kernel-update-package

This will fix WSL2 I guess but I wonder if WSL1 can be made to work, too.

I would like to find the most minimal scripts needed to get WSL1 and WSL2 print
`whoami`.

`wsl --update` won't run because of this error:

> The service cannot be started, either because it is disabled or because it has
no enabled devices associated with it. 

`wsl --set-default-version 2` just prints as if it was started with no options.
