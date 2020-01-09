# react-native-drax

**A drag-and-drop system for React Native**

*"Not to be confused with react-native-picksaw"*

[![npm version](https://badge.fury.io/js/react-native-drax.svg)](https://badge.fury.io/js/react-native-drax)
[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg)](CODE-OF-CONDUCT.md)

## Overview

Drax is a declarative drag-and-drop system for React Native, written in TypeScript. It is designed to be flexible and powerful with the goal of supporting many use cases, while its stock components and default settings should cover the most common scenarios with minimal configuration.

#### Contents

* [Status](#status)
* [Background](#background)
* [Concept](#concept)
* [Installation](#installation)
* [Usage](#usage)
* [Caveats](#caveats)
* [Examples](#examples)
* [Contributing](#contributing)
* [Code of Conduct](#code-of-conduct)
* [License](#license)
* [Acknowledgments](#acknowledgments)

<a name="status"></a>
## Status

This library adheres to [Semantic Versioning (semver)](https://semver.org/) and is in its [0.y.z initial development phase](https://semver.org/#how-should-i-deal-with-revisions-in-the-0yz-initial-development-phase). It has been released so that early adopters (such as the project author) can begin to use it in production and identify gaps in the functionality. The API is subject to potentially significant rework until version 1.0.0 is released, and any minor version increment before then may include breaking changes. Documentation and full examples are still being written.

<a name="background"></a>
## Background

To give an idea of the problem this library is trying to solve, here is some informal background from the creator:

> In our React Native application we had a screen which showed a
> FlatList of cards that could be scrolled through or individually
> tapped to view details. We wanted to add the ability for a user
> to long-press a card then drag it into a different position in
> the list; in other words, we needed a reorderable list.
>
> I figured there must already be a library out there that would
> suit our needs. I tried out a few different packages, which each
> looked to have pros and cons, but nothing quite worked right how
> we expected. To complicate things further, our application used
> `react-navigation`, which seemed to conflict with some of them.
>
> We also had future features on our roadmap which would necessitate
> a more generic drag-and-drop solution. I found it a bit odd that,
> although reorderable lists and drag-and-drop have much functional
> overlap, there didn't seem to be a package for React Native which
> did both. It looked like React for the web was a little more mature
> in this arena, but that didn't help us. I asked some other
> developers if they knew of a solid React Native library for this,
> but they agreed that it was a gap in the ecosystem.
>
> I decided to create my own drag-and-drop library, including
> stock components for common behaviors. The goal, first and
> foremost, was to fulfill our draggable reorderable list wish.
> But beyond that, I wanted a robust foundation that could be
> used to flexibly implement various drag-and-drop-related
> solutions. I am sure that there are scenarios I have not
> yet considered, and I am open to input from other people
> who are working in this space.

<a name="concept"></a>
## Concept

Details on the underlying approach, basic terms, and drag-and-drop event lifecycle can be found in the [Concept Document](docs/concept.md).

<a name="installation"></a>
## Installation

First you must have a project using `react-native` version `>=0.61`, including `react-native-gesture-handler` version `>=1.5.0`. For further information on installing the latter, see [that library's documentation](https://software-mansion.github.io/react-native-gesture-handler/docs/getting-started.html).

Then simply install Drax with:

`yarn add react-native-drax`

or

`npm install react-native-drax`

There is no Cocoapods or native linking step here. You've already covered those needs with `react-native-gesture-handler`.

<a name="usage"></a>
## Usage

*coming soon*

<a name="caveats"></a>
## Caveats

*coming soon*

<a name="examples"></a>
## Examples

For now, here are two simple Snack examples:

- [Basic drag-and-drop](https://snack.expo.io/@lafiosca/react-native-drax---basic-drag-and-drop?platform=ios)
- [Basic reorderable list](https://snack.expo.io/@lafiosca/react-native-drax---basic-reorderable-list?platform=ios)

Note: these Snack examples will not work in the Web device. You must use an iOS (default) or Android device.

<a name="contributing"></a>
## Contributing

See the [Contribution Guidelines](CONTRIBUTING.md) for details.

<a name="code-of-conduct"></a>
## Code of Conduct

Please note that this project is released with a [Contributor Code of Conduct](CODE-OF-CONDUCT.md). By participating in this project you agree to abide by its terms.

<a name="license"></a>
## License

This software library is licensed under the [MIT License](LICENSE.md).

<a name="acknowledgements"></a>
## Acknowledgments

The bulk of this library was written by [Joe Lafiosca](https://twitter.com/joelafiosca) over the course of December 2019. Joe would like to give thanks to co-founder Mark Thomas for being patient with the development process. Joe would also like to give thanks to Lena Raine, Tom Jenkinson, Rollie Pemberton, David Minnick, Tim Smith, and Danny Baranowsky for providing most of the coding background music that inspired this work.
