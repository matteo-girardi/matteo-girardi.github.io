---
layout: post
title:  "Hundreds of merge conflicts in Pods/Pods.xcodeproj/project.pbxproj ?"
date: 2021-03-07 21:28:52 +0100 
categories: Dependency Manager, Merge conflicts
---

Halløj! 👋

Do you use *CocoaPods* as a dependency manager?
Are you in the middle of a big merge and you have hundreds of *merge conflicts* in *Pods/Pods.xcodeproj/project.pbxproj* ?

Then follow these steps:

* remove the *Pods/* folder
* run pod install

The merge conflicts should now be fixes and you can finish your merge.

till next time.. 

Hygge!
