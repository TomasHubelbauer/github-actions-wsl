# GitHub Actions WSL

Is there WSL on the Windows-based GitHub Actions agents?

https://docs.microsoft.com/en-us/windows/wsl/install-on-server

## To-Do

### Await reply on the `-NoRestart` request

https://github.com/microsoft/WSL/issues/4743

### Determine if `bash` in the workflow is a Windows one or a WSL one

It looks like it is the Windows one according to `--version`.
(Compare with WSL on a desktop and see the difference in build.)
It is a bit of a red herring because `wsl` and `ubuntu` don't exist but
`bash` does but it is most likely not the one installed in WSL.
It likely exists even before enabling WSL.
