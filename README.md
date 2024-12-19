# Ambient Sonos Fallback

A plugin for [Ambient](https://github.com/jthawme/ambient). The Spotify API restricts control on sonos playback devices, so when this error is thrown, this plugin steps in and controls the sonos directly

## Usage

```
// ambient.config.js

import * as SonosFallback from "ambient-sonos-fallback";

/** @type {import('./server/types/options.js').Config} */
export default {
  ...,
  plugins: [SonosFallback],
  pluginOptions: {
    sonos: {
      ...
    }
  }
};
```

## Config

| Key | Type | Description | Default |
| --- | ---- | ----------- | ------- |
