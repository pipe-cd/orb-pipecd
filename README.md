# PipeCD Orb
Orb for interacting with PipeCD on CircleCI. See: [the documentation](https://pipecd.dev/docs/user-guide/command-line-tool).

# Usage
Explore the src/examples directories to get an idea of how this works. If you feel there is something we could clarify, please let us know!
_For full usage guidelines, see the [orb registry listing](https://circleci.com/developer/orbs/orb/pipe-cd/pipecd)._

# Contributing
We welcome [issues](https://github.com/pipe-cd/orb-pipecd/issues) to and [pull requests](https://github.com/pipe-cd/orb-pipecd/pulls) against this repository!

## How to Publish
* Create and push a branch with your new features.
* When ready to publish a new production version, create a Pull Request from _feature branch_ to `master`.
* The title of the pull request must contain a special semver tag: `[semver:<segement>]` where `<segment>` is replaced by one of the following values.

| Increment | Description|
| ----------| -----------|
| major     | Issue a 1.0.0 incremented release|
| minor     | Issue a x.1.0 incremented release|
| patch     | Issue a x.x.1 incremented release|
| skip      | Do not issue a release|

Example: `[semver:major]`

* Squash and merge. Ensure the semver tag is preserved and entered as a part of the commit message.
* On merge, after manual approval, the orb will automatically be published to the Orb Registry.
