---
layout: post
title:  "Swift Package Manager caches it heavily!"
date: 2021-03-09 22:02:27 +0100 
categories: Swift Package Manager
---

Halløj! 👋

Today I ran into some weird behaviour while using Swift Package Manager.

While working on a sample app using the awesome [*Composable Architecture*](https://github.com/pointfreeco/swift-composable-architecture) framework (which you should definitely check out!) by [*PointFree*](https://www.pointfree.co/), I wanted to get rid of a package called [*Neumorphic*](https://github.com/costachung/neumorphic/), which is a pretty cool Soft Neumorphism UI framework. I wanted to remove it becuase it isn't strictly necessary to the sample app. Anyway, before doing that I decided to *Update to Latest Package Versions* the packages and then something weird happened: the Composable Architecture package was somehow missing/greyed out in the Project Navigation menu. Then I deleted it in the project's Swift Packages tab

![project-swift-packages](/assets/images/project-swift-packages.png)

and surprisingly it was still visible in the Project Navigation menu.

![project-navigator](/assets/images/cf-prject-navigator.png)

I tried to add it again but I got the following error:

![added-package-again](/assets/images/add-swift-package-again.png)

Since I had created an *internal* swift package which uses the Composable Architecture

![internal-swift-package](/assets/images/swift-package-internal.png)

I looked at its *Package.swift* file and commented out the dependencies that it depended on.

![remove-dependency-in-package-swift](/assets/images/remove-dependency-in-package-swift.png)

then I've added the *Composable Architecture* package once again, uncommented those dependencies in the *Package.swift* and the Swift Packages of the project look fine now. The project and its frameworks are now building.

Well, it looks like SPM caches quite heavily the packages added to the project even if you'll remove one of them, especially if you have other *internal* Swift packages that reference that dependency.

till next time.. 

Hygge!
