# convoo-starter

<p align="center">
  <a href="https://convoo.me" target="_blank"><img alt="Convoo" src="Convoo.png" width="300"></a>
</p>

<p align="center">
A starter for your Polymer app using Firebase and Redux
</p>

<p align="center">
  <a href="http://waffle.io/convoo/roadmap" target="_blank"><img src="https://badge.waffle.io/convoo/roadmap.svg?label=In%20Progress&title=In%20Progress"></a>
  <a href="https://gitter.im/convoo/General" target="_blank"><img src="https://img.shields.io/badge/gitter-join%20chat-brightgreen.svg"></a>
  <a href="https://www.webcomponents.org/author/convoo" target="_blank"><img src="https://img.shields.io/badge/webcomponents.org-published-blue.svg"></a>
</p>

---


Convoo's starter is a starting point for Polymer apps built on top of the [Polymer Starter Kit](https://github.com/PolymerElements/polymer-starter-kit). Convoo's starter targets
applications that are built using Firebase and Redux.

It comes with:

* Firebase authentication already set up for email as well as social providers
* Redux with polymer-redux set up
* Internationalization set up with a locales.json file for you to edit
* Example iron-list view displaying a stream of information from firebase
* Example form saving to firebase

## Setup

1. Get the starter

Using the Polymer CLI:

```
npm install -g polymer-cli
npm install -g generator-polymer-init-convoo-starter
polymer init convoo-starter
```

[Simple Download](https://github.com/convoo/convoo-starter/releases).

2. Setup firebase

```
npm install -g firebase-tools
firebase init
```

When Firebase asks you for your public directory enter `build/unbundled`. Since [Firebase uses HTTP 2](https://firebase.googleblog.com/2016/09/http2-comes-to-firebase-hosting.html) this should be fine.
You can also use `build/bundled` if you prefer.

3. Serving while developing

While developing, you can quickly view wha tyou're working on using:

```
polymer serve
```

4. Build & Deploy

When you're ready to deploy, first build your work and double check it locally:

```
polymer build
firebase serve
```

If everything works as expected then go ahead and deploy using:

```
firebase deploy
```
