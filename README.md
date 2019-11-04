# React Tracking Outbrain

[![Build Status](https://travis-ci.org/realalexbarge/react-tracking-outbrain.svg?branch=master)](https://travis-ci.org/realalexbarge/react-tracking-outbrain) [![dependencies Status](https://david-dm.org/realalexbarge/react-tracking-outbrain/status.svg)](https://david-dm.org/realalexbarge/react-tracking-outbrain) [![devDependencies Status](https://david-dm.org/realalexbarge/react-tracking-outbrain/dev-status.svg)](https://david-dm.org/realalexbarge/react-tracking-outbrain?type=dev) [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

Un-official module to easily add Outbrain pageview tracking to react apps.

# Installation

With [npm](https://www.npmjs.com/):

```bash
npm install react-tracking-outbrain --save
```

# Usage

### With npm

Initializing OutbrainTracking and tracking pageviews:

```js
import OutbrainTracking from 'react-tracking-outbrain';
OutbrainTracking.initialize('TRACKING_ID');
OutbrainTracking.pageview();
```
