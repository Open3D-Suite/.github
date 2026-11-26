# Contributing to Open3D

Thank you for wanting to help. Every Open3D app follows the same guidelines, so that the suite feels like
one thing to the people who use it. They are in [Open3D-SDK](https://github.com/Open3D-Suite/Open3D-SDK):
read its guides before you start.

## A change to an app

- Work on a branch and open a pull request to `main`. Only an app's author writes in its repository, so
  for an app that is not yours the branch is on your fork. CI runs the app's `tools\check.ps1` on it; once
  it passes, the app's author reviews it and merges it.
- Everything in the repository is in English: code, comments, commits, documents.
- Small commits, each one sentence in the imperative ("Make the drop-down remember its choice").
- A bug that is fixed comes with a test that fails without the fix; new logic comes with its tests.
- A change a user can notice gets its line in the app's `CHANGELOG.md`, under `## In development`, in the
  same commit.
- Nothing of your computer goes into a file: no paths with your user name, no addresses of your network.

## A new app

New apps start from the Open3D-SDK template, with a name agreed with the other members first (Open + a
name). Its author makes its repository in this organization and runs it. It enters the launcher through
a pull request to [Open3D-Launcher](https://github.com/Open3D-Suite/Open3D-Launcher) that another member
approves after reviewing its code and its security and testing it as a user would; GitHub then signs the
launcher's catalog, once a member other than whoever asked for the signature approves it. See
[Start a new app](https://github.com/Open3D-Suite/Open3D-SDK/blob/main/docs/start-a-new-app.md).

## Releases

A release is made from `main` as a draft, and the app's author publishes it once it has been tested as a
user would; the launcher then offers it to everyone. A published release cannot change: a mistake in it
is fixed by a new version. See
[Distribution](https://github.com/Open3D-Suite/Open3D-SDK/blob/main/docs/distribution.md).

## Security

Report a security problem privately, never in a public issue: [SECURITY.md](SECURITY.md).
