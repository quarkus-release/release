# Releasing Quarkus, the supersonic subatomic way

<p align="center"><img src="https://design.jboss.org/quarkus/bot/final/images/quarkusbot_full.svg" width="128" height="128" /></p>

This repository is used to release the [Quarkus framework](https://quarkus.io/).

Releases are handled automatically by GitHub Actions (with some human interactions and a few manual steps - they are clearly described) using the the [Conversational Release Action](https://github.com/quarkusio/conversational-release-action) which orchestrates the [historical release scripts](https://github.com/quarkusio/quarkus-release) (these scripts are still usable directly if needed).

Even if the process is far more guided with this new approach, releases should still be started by Quarkus maintainers who are aware of the release process.

To start a release, create a [new issue](https://github.com/quarkus-release/release/issues/new?assignees=&labels=kind%2Frelease&projects=&template=release.yml).
It will start a workflow run that will guide you through the release process.

If you have any questions about the process, please ping `@gsmet`.
