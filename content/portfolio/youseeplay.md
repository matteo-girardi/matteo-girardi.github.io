---
title: YouSee Play 📺📱👀▶️
description: A mobile application for streaming Live TV, Movies & TV series.
---

<style type="text/css">
.yousee-banner {
	background-color: #092119;
  padding: 10px;
  border: 3px solid black;
  margin: 15px 0;
  box-shadow: -7px 7px #2f2f2f;
}
mark {
 	background-image: linear-gradient(to left,#ff79c6,#bd93f9);
  color: black;
  padding: 0.11em;
  border-radius: 4px;
}
</style>

# YouSee Play is the <mark>biggest streaming platform in Denmark 🇩🇰 </mark>

At [YouSee](https://yousee.dk/play#forside)/[Nuuday](https://nuuday.com/) I have been working on the YouSee Play mobile app which is available for iPhone, iPad and Apple TV.

<div class="yousee-banner">
	<h2>Endless Entertainment with YouSee Play</h2>
	<p>The YouSee Play app lets you enjoy TV, movies, and series on your mobile or tablet, giving you unlimited access to hours of entertainment anytime, anywhere. It brings together your favorite TV channels, a vast library of movies and series, and Denmark’s largest kids’ universe – all in one app. Here’s what you get with the YouSee Play app:

  - Live TV – Watch your favorite channels wherever you are, whenever you want.
  - Restart – Missed the beginning of a show? Simply restart it from the beginning.
  - TV Archive – Explore thousands of new programs every week in the TV archive.
  - Manage Your Viewing – Easily switch TV channels or streaming services directly within the app.
  - Movies & Series – Enjoy unlimited access to a rich selection of movies and series for the whole family, with fresh titles added weekly.
  - Children’s Universe – Dive into hours of fun with a dedicated library of movies and series for kids of all ages.</p>
</div>



## Achievement 🎉

- From 75% to <mark>**99.8% crash-free rate**</mark> 🚀
- <mark>**Improved AppStore ratings from 2.0 to 4.3**</mark> ✨
- Significantly improved video start failures and video startup time by <mark>**more than 20%**</mark> 💪
- <mark>**Significantly improved development efficiency**</mark> by having a single source code on all Apple platforms. 👨🏻‍💻

## Features, projects, tasks & responsibilities 📖

- Synopsis feature:
	- Redesigned the Synopsis on client apps (iOS/iPad and tvOS), and other parts of the UI using UIKit & SwiftUI.
  - Rewritten how an asset and related content is shown to the user, so that it is presented in a cleaner and more appealing way to the user.
  - Implemented several sub-features: Recordings, Reminders & Start Over.
- Core architecture project:
	- The core architecture of the application has been redisigned and rewritten using MVVM and [The Composable Architecture](https://github.com/pointfreeco/swift-composable-architecture). This approach came with several benefits: <mark>consistent way of implementing features, which are easier to implement and integrate with the souce code, easier to write unit tests</mark>.
- Integrated third-party C++ library for Digital Rights Management. Only entitled users can watch contents in the app.
- Native Player feature:
	- The old, legacy, custom player written in ObjC was removed. The Apple's native player has been used instead on all platforms. This approach had several benefits: <mark>same native behaviour on all platforms, less code maintanance, up to date with latest native features</mark>.
- Scrubbing rights feature:
	- Implemented the business logic that handles scrubbing rights.
- One source code project:
	- Initially the iOS and tvOS app had two different source code, doing the same thing. Together with my team, we merged these into one single source code. We moved business logic, features, and UI into reusable and modular swift packages. We have implemented platform-dependent UI only when necessary. This has the benefit of <mark>improving development efficiency, reducing bugs, complexity and making it easier to develop features</mark>.
- Integrated third-party analytics frameworks (Conviva, Agama), for data analysis; for example: Video startup time. This gave us lots of data and great insight into our app, so that we could <mark>take decisions that were backed by data</mark>.
- UI Automation Tests project:
	- Built UI automation tests workflow on Bitrise, using Appium. This helped a lot the QA team, by <mark>saving time and improving the quality of the verification process</mark>.
- CI/CD: built pipelines and workflows on Bitrise.
- Concurrency feature:
	- Users may have a limited amount on concurrent streams, depending on the content provider. For example: a TV channel may have two concurrent streams.
- Fallback feature:
	- In case of accidents, this feature can be activated using a remote feature flag, so that users can enjoy contents that are not affected by issues from back-end. It also informs users of unavailable services in a user-friendly way.

You can find the [YouSee Play](https://apps.apple.com/dk/app/yousee-play/id476306715) application on the AppStore

## Languages, Tools and Technologies 🛠️

- Swift/Objective-C.
- Xcode, Swift Package Manager, git, Bitrise.
- UIKit, Combine, SwiftUI, Alamofire, AppCenter, Firebase, AppSpector, The Composable Architecture.
