# gradle-pages

[![Bintray](https://img.shields.io/bintray/v/ajoberstar/maven/gradle-git.svg?style=flat-square)](https://bintray.com/ajoberstar/maven/gradle-git/_latestVersion)
[![Travis](https://img.shields.io/travis/ajoberstar/gradle-git.svg?style=flat-square)](https://travis-ci.org/ajoberstar/gradle-git)
[![GitHub license](https://img.shields.io/github/license/ajoberstar/gradle-git.svg?style=flat-square)](https://github.com/ajoberstar/gradle-git/blob/master/LICENSE)

## Project Status

gradle-git has been around since 2012 and has evolved quite a bit from the original release. In order to continue to evolve these features, this project is being broken up into multiple repositories. As such:

- gradle-git will no longer be maintained

| feature | replacement | comments |
|---------|-------------|----------|
| `org.ajoberstar.grgit` | [grgit](https://github.com/ajoberstar/grgit) | Grgit has been an independent project since 2013 and has been stable for quite a while. Version 2.0 removed some deprecated features, but otherwise is fully compatible with existing usage. It also integrates the `org.ajoberstar.grgit` plugin directly into the project. |
| `org.ajoberstar.github-pages` | [gradle-git-publish](https://github.com/ajoberstar/gradle-git-publish) | `org.ajoberstar.git-publish` is a more robust version of the old plugin. It is functionally equivalent (or better), but does require porting configuration over as noted in the README. |
| `org.ajoberstar.release-*` | [reckon](https://github.com/ajoberstar/reckon) | Reckon focuses solely on determining your project version (and assisting with tagging and pushing that tag). It provides an opinionated model of how to apply [semantic versioning](http://semver.org), with more finite configuration options. |
| `org.ajoberstar.release-*` | [nebula-release](https://github.com/nebula-plugins/nebula-release-plugin) | If reckon doesn't suit your needs, nebula-release has forked the gradle-git release plugin and can serve as a replacement for this. |

## Why do you care?

Git is immensely popular and being able to interact with it as part of a build process can be very valuable
to provide a more powerful and consistent result.

## What is it?

gradle-git is a set of [Gradle](http://gradle.org) plugins:

* `org.ajoberstar.grgit` - provides a `Grgit` instance, allowing interaction with the Git repository
the Gradle project is contained in
* `org.ajoberstar.github-pages` - publishes files to the `gh-pages` branch of a Github repository
* `org.ajoberstar.release-base` - general structure for inferring a project version and releasing it
* `org.ajoberstar.release-opinion` - opinionated defaults for `org.ajoberstar.release-base`

See [Grgit](https://github.com/ajoberstar/grgit) for details on the Git library used underneath, including
configuration for authentication.

## Usage

**NOTE:** gradle-git modules require Java 7 (or higher).

* [Release Notes](https://github.com/ajoberstar/gradle-git/releases)
* [Wiki](https://github.com/ajoberstar/gradle-git/wiki)
* [Javadoc](http://ajoberstar.org/gradle-git/docs/javadoc)
* [Groovydoc](http://ajoberstar.org/gradle-git/docs/groovydoc)

## Questions, Bugs, and Features

gradle-git is not maintained anymore. See the _Project Status_ section above for details.

## Contributing

gradle-git is not maintained anymore. See the _Project Status_ section above for details.

## Acknowledgements

Thanks to all of the [contributors](https://github.com/ajoberstar/gradle-git/graphs/contributors).

Credit goes to [Peter Ledbrook](https://github.com/pledbrook) for the initial
idea for the `org.ajoberstar.github-pages` plugin.

Thanks to [Zafar Khaja](https://github.com/zafarkhaja) for the very helpful
[java-semver](https://github.com/zafarkhaja/jsemver) library.
