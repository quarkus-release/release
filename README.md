# Releasing Quarkus, the supersonic subatomic way

<p align="center"><img src="https://design.jboss.org/quarkus/bot/final/images/quarkusbot_full.svg" width="128" height="128" /></p>

## About

This repository is used to release the [Quarkus framework](https://quarkus.io/).

Releases are handled automatically by GitHub Actions (with some human interactions and a few manual steps - they are clearly described) using the the [Conversational Release Action](https://github.com/quarkusio/conversational-release-action) which orchestrates the [historical release scripts](https://github.com/quarkusio/quarkus-release) (these scripts are still usable directly if needed).

Even if the process is far more guided with this new approach, releases should still be started by Quarkus maintainers who are aware of the release process.

## Starting a release

To start a release, create a [new issue](https://github.com/quarkus-release/release/issues/new?assignees=&labels=kind%2Frelease&projects=&template=release.yml).
It will start a workflow run that will guide you through the release process.

Just keep the issue open in a browser tab and have a look when you are notified of new issue comments in the tab.

:rotating_light: When starting a new LTS release cycle, you need to declare the new LTS version [here](https://github.com/quarkusio/conversational-release-action/blob/main/src/main/java/io/quarkus/bot/release/util/Branches.java#L10).

### Examples

#### 3.2.x.Final

- <kbd>Branch</kbd> `3.2`
- <kbd>Qualifier</kbd>
- <kbd>Major version</kbd>

There is no need for a qualifier. `.Final` will be added automatically.

#### 3.8.0.CR1

- <kbd>Branch</kbd> `3.8` (the branch will be created automatically)
- <kbd>Qualifier</kbd> `CR1`
- <kbd>Major version</kbd>

#### 3.8.x

- <kbd>Branch</kbd> `3.8`
- <kbd>Qualifier</kbd>
- <kbd>Major version</kbd>

#### 4.0.0.CR1

- <kbd>Branch</kbd> `4.0` (the branch will be created automatically)
- <kbd>Qualifier</kbd> `CR1`
- <kbd>Major version</kbd> ✔️

## Questions

If you have any questions about the process, please ping `@gsmet`.
