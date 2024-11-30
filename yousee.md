---
layout: page
title: YouSee Play
description: A video streaming application.
permalink: /work/yousee-play/
---

<link rel="stylesheet" href="/assets/css/styles.css">

At YouSee/Nuuday I have been developing the YouSee Play app which is available on iPhone, iPad and Apple TV.

> Endless Entertainment with YouSee Play
>
> The YouSee Play app lets you enjoy TV, movies, and series on your mobile or tablet, giving you unlimited access to hours of entertainment anytime, anywhere. It brings together your favorite TV channels, a vast library of movies and series, and Denmark’s largest kids’ universe – all in one app.
>
> Here’s what you get with the YouSee Play app:
>
> - Live TV – Watch your favorite channels wherever you are, whenever you want.
> - Restart – Missed the beginning of a show? Simply restart it from the beginning.
> - TV Archive – Explore thousands of new programs every week in the TV archive.
> - Manage Your Viewing – Easily switch TV channels or streaming services directly within the app.
> - Movies & Series – Enjoy unlimited access to a rich selection of movies and series for the whole family, with fresh titles added weekly.
> - Children’s Universe – Dive into hours of fun with a dedicated library of movies and series for kids of all ages.
>
> At YouSee, we’re constantly enhancing and updating our app to deliver the best experience possible. To make the most of YouSee Play, we recommend enabling automatic updates to ensure you’re always using the latest version.

## Achievement 🎉

- From 75% to **99.8% crash-free rate** 🚀
- **Improved ratings from 2.0 to 4.3** ✨
- Significantly improved video start failures and video startup time by more than 20%. 💪
- Development efficiency significantly improved through the use of shared code across all Apple platforms. 👨🏻‍💻

## Features, projects, tasks & responsibilities 📖

- Redesigning the Synopsis, and other part of the UI using UIKit & SwiftUI:
  - Rewriting how an asset and related content is presented to the user, so that it is presented in a cleaner and more applealing way to the user.
- Redesigning and rewriting the core architecture of the app's architecture using MVVM and [The Composable Architecture](https://github.com/pointfreeco/swift-composable-architecture). The company is now positioned to innovate more rapidly, unlocking new possibilities for users and enhancing customer retention and acquisition.
- Integration with third-party C++ DRM Library. Only users that have proper rights can watch contents in the app.
- Player: rewritten the entire architecture and logic.
- Bringing together two applications doing the same thing, with different code bases, into one single app (and source code!). Moving business logic in reusable and modular swift packages. This has the benefit of improving development efficiency, reducing bugs, complexity and making it easier to develop feature.
- Integrate third-party analytics frameworks (Conviva, Agama), for data analysis, for example: Video startup time. This gave us lots of data and great insight into our app, so that we could take decisions that were backed by data.
- Build UI automation test workflow on Bitrise, using Appium. This helped a lot the QA team, by saving time and improving the quality of the verification process.

You can find the [YouSee Play](https://apps.apple.com/dk/app/yousee-play/id476306715) application on the AppStore

## Languages, Tools and Technologies 🛠️

- Swift/Objective-C.
- Xcode, Swift Package Manager, git, Bitrise.
- UIKit, Combine, SwiftUI, Alamofire, AppCenter, Firebase, AppSpector, The Composable Architecture.
