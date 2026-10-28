<div align="center">

# Project Continuum

**Visual workflows that actually run, and survive.**

An open-source, cloud-native, no-code workflow platform for ML, cheminformatics and ETL.
Drag-and-drop nodes in the browser. Durable execution on [Temporal](https://temporal.io).

[Website](https://projectcontinuum.org) · [Documentation](https://docs.projectcontinuum.org) · [Quick start](https://github.com/projectcontinuum-org/continuum-local-setup) · [Discussions](https://github.com/projectcontinuum-org/continuum-platform-core/discussions)

</div>

---

## Why Continuum

- **Browser-native.** A full IDE-style workflow editor (Eclipse Theia and React Flow). Nothing to install.
- **Crash-proof.** Workflows survive process crashes, network failures and restarts, because execution runs on Temporal.
- **Live.** Node execution streams back to the editor in real time.
- **Fast data passing.** Nodes exchange Apache Parquet tables, not JSON blobs.
- **Extensible.** Add capabilities by deploying new workers, without touching existing ones.

## Get started

You need Docker with Docker Compose v2.

```bash
git clone https://github.com/projectcontinuum-org/continuum-local-setup
cd continuum-local-setup/docker
docker compose up -d
```

See the [local setup guide](https://github.com/projectcontinuum-org/continuum-local-setup) for details.

## Repositories

### Platform

| Repository | Description |
|---|---|
| [continuum-platform-core](https://github.com/projectcontinuum-org/continuum-platform-core) | Core backend: API server, worker framework, shared libraries |
| [continuum-workbench](https://github.com/projectcontinuum-org/continuum-workbench) | Browser IDE and workflow editor |
| [continuum-charts](https://github.com/projectcontinuum-org/continuum-charts) | Helm charts for Kubernetes deployment |
| [continuum-local-setup](https://github.com/projectcontinuum-org/continuum-local-setup) | Run the full stack locally with Docker Compose |

### Node libraries (feature workers)

| Repository | Description |
|---|---|
| [continuum-feature-base](https://github.com/projectcontinuum-org/continuum-feature-base) | Core data transformation, REST, scripting and anomaly detection nodes |
| [continuum-feature-cheminformatics](https://github.com/projectcontinuum-org/continuum-feature-cheminformatics) | RDKit-powered cheminformatics nodes |
| [continuum-feature-ai](https://github.com/projectcontinuum-org/continuum-feature-ai) | AI/ML nodes, including LLM fine-tuning |
| [continuum-feature-knime](https://github.com/projectcontinuum-org/continuum-feature-knime) | KNIME workflow executors |

### Starter template, docs and tooling

| Repository | Description |
|---|---|
| [continuum-feature-template](https://github.com/projectcontinuum-org/continuum-feature-template) | Starter template for building your own feature worker and nodes (not a production node library) |
| [continuum-docs](https://github.com/projectcontinuum-org/continuum-docs) | Documentation site source |
| [continuum-website](https://github.com/projectcontinuum-org/continuum-website) | Project website source |
| [continuum-jsonform-playground](https://github.com/projectcontinuum-org/continuum-jsonform-playground) | Playground for node dialog schemas and UI |

## Contributing

Contributions are welcome. Start with a [good first issue](https://github.com/search?q=org%3Aprojectcontinuum-org+label%3A%22good+first+issue%22+state%3Aopen&type=issues), or ask questions and share ideas in [Discussions](https://github.com/projectcontinuum-org/continuum-platform-core/discussions). To build your own nodes, start from [continuum-feature-template](https://github.com/projectcontinuum-org/continuum-feature-template). Please read our [Code of Conduct](https://github.com/projectcontinuum-org/.github/blob/main/CODE_OF_CONDUCT.md) first.

## Security

To report a vulnerability, follow our [security policy](https://github.com/projectcontinuum-org/.github/blob/main/SECURITY.md). Please don't open a public issue.
