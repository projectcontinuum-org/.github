# Getting Support

Where to go depends on what you need.

| I want to... | Go to |
|---|---|
| Learn how Continuum works, deploy it, or build nodes | [Documentation](https://docs.projectcontinuum.org) |
| Run the whole stack on my machine | [continuum-local-setup](https://github.com/projectcontinuum-org/continuum-local-setup) |
| Ask a question or share an idea | [Discussions](https://github.com/projectcontinuum-org/continuum-platform-core/discussions) |
| Report a bug or request a feature | [Open an issue](https://github.com/projectcontinuum-org) in the relevant repository |
| Report a security vulnerability | Follow the [security policy](SECURITY.md). Don't open a public issue. |
| Report a conduct problem | See the [Code of Conduct](CODE_OF_CONDUCT.md) |

## Before opening an issue

- Search existing issues and discussions to see whether it has been reported.
- Check the version you are running and try the latest release.
- Include steps to reproduce, what you expected, what happened, and relevant logs.

## Choosing a repository

| Problem is in... | Repository |
|---|---|
| API server, orchestration, workers framework, message bridge | [continuum-platform-core](https://github.com/projectcontinuum-org/continuum-platform-core) |
| The browser editor or node dialogs | [continuum-workbench](https://github.com/projectcontinuum-org/continuum-workbench) |
| A specific node | The matching `continuum-feature-*` repository |
| Kubernetes install | [continuum-charts](https://github.com/projectcontinuum-org/continuum-charts) |
| Docker Compose install | [continuum-local-setup](https://github.com/projectcontinuum-org/continuum-local-setup) |
| The docs | [continuum-docs](https://github.com/projectcontinuum-org/continuum-docs) |

If you are not sure, open an issue in `continuum-platform-core` and we will move it.
