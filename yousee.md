---
layout: page
title: YouSee Play
description: A video streaming application.
permalink: /work/yousee-play/
---

<link rel="stylesheet" href="/assets/css/styles.css">

At YouSee/Nuuday I have been developing the YouSee Play app which is available on iPhone, iPad and Apple TV.

Achievement:

- **99.8% crash-free rate**
- **Improve ratings from 2.0 to 4.3**

My responsibilities and tasks were the following:

- UI development using UIKit & SwiftUI
- Architecture development using MVVM and Redux patterns (TCA)
- Integration with third-party C++ DRM Library

Features & projects I have worked on:

- Player: rewritten the entire architecture and logic
- Synopsis: rewritten how an asset and related content is presented to the user
- Bringing together two apps (different code bases) doing the same thing into one single app (and source code!), moving business logic in reusable swift packages. One code base was for iOS/iPad, and the other was for tvOS, which was developed by a third-party company (outsourced).
- Integrate third-party analytics frameworks (Conviva, Agama), for data analytics, for example:
  - Video startup time - the time it takes for the stream to start playing.
- Build UI automation test workflow on Bitrise

You can find the [YouSee Play](https://apps.apple.com/dk/app/yousee-play/id476306715) application on the AppStore

Languages, Tools and Technologies:

- Swift/Objective-C.
- Xcode, Swift Package Manager, git, Bitrise.
- UIKit, Combine, SwiftUI, Alamofire, AppCenter, Firebase, AppSpector, The Composable Architecture.
