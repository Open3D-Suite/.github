# Contributing to Open3D

Thank you for wanting to help. Every Open3D app follows the same guidelines, so that the suite feels like
one thing to the people who use it. They are in [Open3D-SDK](https://github.com/Open3D-Suite/Open3D-SDK):
read its guides before you start.

## A change to an app

- Work on a branch and open a pull request to `main`. CI runs the app's `tools\check.ps1` on it; once it
  passes, a maintainer reviews it and merges it.
- Everything in the repository is in English: code, comments, commits, documents.
- Small commits, each one sentence in the imperative ("Make the drop-down remember its choice").
- A bug that is fixed comes with a test that fails without the fix; new logic comes with its tests.
- A change a user can notice gets its line in the app's `CHANGELOG.md`, under `## In development`, in the
  same commit.
- Nothing of your computer goes into a file: no paths with your user name, no addresses of your network.

## A new app

New apps start from the Open3D-SDK template, with a name agreed with the maintainers first (Open + a name).
The maintainers make its repository in this organization. Before it enters the launcher, they review its
code and its security and test it as a user would. See
[Start a new app](https://github.com/Open3D-Suite/Open3D-SDK/blob/main/docs/start-a-new-app.md).

## Releases

A release is made from `main` as a draft; the maintainers publish it, and the launcher then offers it to
everyone. See [Distribution](https://github.com/Open3D-Suite/Open3D-SDK/blob/main/docs/distribution.md).

## Security

Report a security problem privately, never in a public issue: [SECURITY.md](SECURITY.md).
