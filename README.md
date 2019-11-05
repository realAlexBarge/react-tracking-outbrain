# React Tracking Outbrain

[![Build Status](https://travis-ci.org/realalexbarge/react-tracking-outbrain.svg?branch=master)](https://travis-ci.org/realalexbarge/react-tracking-outbrain) [![dependencies Status](https://david-dm.org/realalexbarge/react-tracking-outbrain/status.svg)](https://david-dm.org/realalexbarge/react-tracking-outbrain) [![devDependencies Status](https://david-dm.org/realalexbarge/react-tracking-outbrain/dev-status.svg)](https://david-dm.org/realalexbarge/react-tracking-outbrain?type=dev) [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

Un-official module to easily add Outbrain pageview tracking to react apps. It functions as a tiny wrapper for the native script tag and window api. After initialization the Outbrain script is injected into the document.

# Installation

With [npm](https://www.npmjs.com/):

```bash
npm install react-tracking-outbrain --save
```

# Usage

Before tracking any page views or events the tracker needs to be imported and initialized with the custom tracking id:

```js
import OutbrainTracking from 'react-tracking-outbrain';
OutbrainTracking.initialize('TRACKING_ID');
```

After initializing page views can be tracked like this:

```js
OutbrainTracking.trackPageview();
```

There is also the option to track custom events with event action:

```js
OutbrainTracking.trackEvent(eventAction);
```

There is also a method to expose the raw obApi tracking function api from the window:

```js
OutbrainTracking.getTracker();
```

# How this works

This modules takes care of injecting the provider specific tracking script into the document and provides a tiny wrapper for the tracking api. It also exposes the tracker object api for direct access.

Documentation for the raw tracker api can be found [here](https://www.outbrain.com/help/advertisers/multiple-conversions/).
