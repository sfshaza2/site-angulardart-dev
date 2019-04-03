---
layout: components
title: "Codelab: AngularDart Components"
description: "Learn how to use AngularDart Components—a preview of Material Design components that are widely used in Google's Dart apps."
toc: false
permalink: /codelabs/angular_components
nextpage:
  url: /codelabs/angular_components/1-base
  title: "Step 1: Get to Know the Software"
---

This codelab introduces you to a preview release of
[AngularDart Components](/angular/components),
part of a large group of well-tested components that are widely used in
Google’s Dart apps.

To complete this codelab, you need the following:

* A Windows, Mac, or Linux computer with Dart SDK 2.1.0 (or a higher version)
* A web connection and modern browser

This codelab assumes that you are familiar with Dart web app development.
If you aren’t, instead try one of the
[other Dart web codelabs](/codelabs).
Familiarity with AngularDart development isn't required but is helpful, since
this codelab doesn't explain
[Angular concepts](/angular/guide/architecture).

In this codelab, you’ll take a basic AngularDart app, called Lottery Simulator,
and use AngularDart Components to simplify the code and beautify the UI.
You can play with a
{% assign ng-major-vers = site.data.pkg-vers.angular.vers | regex_replace: '\.[^\.]+\.[^\.]+$' -%}
[live copy of the final app](/examples/lottery/4-final/).

Here are screenshots of the app’s UI, before and after conversion to
use AngularDart Components.

|----------------+-----------------------|
| Base app       | Final app             |
|:--------------:|:---------------------:|
| ![HTML app](/codelabs/angular_components/images/app-base.png) | ![AngularDart Components app](/codelabs/angular_components/images/app-final.png) |

<img src="/codelabs/angular_components/images/cartoon-guy.png"
    alt="top-hatted guy from the cartoon that appears in the app's About tab"
    align="right">

## Contents

* [Step 1: Get to Know the Software](/codelabs/angular_components/1-base)
  * Get the app code
  * Get familiar with the base app
  * Get familiar with AngularDart Components
* [Step 2: Start Using AngularDart Components](/codelabs/angular_components/2-starteasy)
  * Copy the source code
  * Depend on `angular_components`
  * Set up the root component’s Dart file
  * Use `<material-progress>`
  * Use `<material-icon>` in buttons<br>
    <i class="fas fa-exclamation-circle"> </i> Common problem: Forgetting to import material icon fonts
  * Use `<material-icon>` in other components<br>
    <i class="fas fa-exclamation-circle"> </i> Common problem: Forgetting to register a component
  * Use `<acx-scorecard>`<br>
    <i class="fas fa-exclamation-circle"> </i> Common problem: Registering the wrong component
* [Step 3: Upgrade Buttons and Inputs](/codelabs/angular_components/3-usebuttons)
  * Use `<material-toggle>`
  * Use `<material-fab>`<br>
    <i class="fas fa-exclamation-circle"> </i> Common pattern: (trigger)
  * Use `<material-checkbox>`
  * Use `<material-radio>` and `<material-radio-group>`
* [Step 4: Add Expansion Panels and Tabs](/codelabs/angular_components/4-final)
  * Use `<material-expansionpanel>` and `<material-expansionpanel-set>`
  * Use `<material-tab>` and `<material-tab-panel>`
* [What Next?](/codelabs/angular_components/what-next)
