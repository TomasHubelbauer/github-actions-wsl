# GitHub Actions WSL

Is there WSL on the Windows-based GitHub Actions agents?

https://docs.microsoft.com/en-us/windows/wsl/install-on-server

Turns out it is impossible to use because enabling WSL requires the agent
to restart which is impossible in the GitHub Actions agents, as confirmed
by GitHub support.

There is a request to add WSL to the default Windows image:

https://github.com/actions/virtual-environments/issues/50

## To-Do
