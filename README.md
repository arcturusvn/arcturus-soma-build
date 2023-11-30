# Arcturus Soma Build

Arcturus Soma Build is a common utility project for Arcturus SDK to use for plugin and dependency
management. This is not intended for library users.

![workflow](https://github.com/arcturusvn/arcturus-soma-build/actions/workflows/build.yml/badge.svg)
![GitHub License](https://img.shields.io/github/license/arcturusvn/arcturus-soma-build)


## Quickstart

If you are using Maven, use this artifact as your project's parent.

```xml
<parent>
  <groupId>vn.arcturus.soma</groupId>
  <artifactId>arcturus-soma-build</artifactId>
  <version>1.0.0-RELEASE</version>
</parent>
```

## Build & Publish

### Setup CLI Tool

```shell
npm install -g @arcturusvn/arcturus-neural-cli
```

### Setup environment:

**Step 1**: Create a GitHub access token.

**Step 2**: Add to Environment

- `GITHUB_USERNAME`: [github-username]
- `GITHUB_TOKEN`: [access-token]

### Build locally:

```shell
neural build [--profile=maven,coverage,...] [--skip-test] [--debug]
```

### Publish SDK to Package Registry:

- `SNAPSHOT`: please check out to `build` branch (Ex: 1.0.x).

```shell
neural publish SNAPSHOT
```

- `RELEASE CANDIDATE (RC)`: please check out to `main` branch.

```shell
neural publish RC [--tag]
```

- `RELEASE`: please check out to `main` branch.

```shell
neural publish RELEASE [--tag] [--bump]
```

## Usages

Declare this artifact as the parent of Maven projects of Arcturus SDK. This brings useful
Maven plugins and their configurations to the Maven projects, such as compilations, document
generation, and library publication.

## Contributing

Contributions to this library are always welcome and highly encouraged.

See [CONTRIBUTING.md](CONTRIBUTING.md) documentation for more information on how to get started.

Please note that this project is released with a Contributor Code of Conduct. By participating in
this project you agree to abide by its terms. See [Code of Conduct](CODE_OF_CONDUCT.md) for more
information.

## License

Apache 2.0 - See [LICENSE](LICENSE) for more information.
