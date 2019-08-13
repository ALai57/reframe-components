# Reframe components

A [re-frame](https://github.com/Day8/re-frame) library that contains custom components. Based on Day8's re-com library

### Development setup:

Once a clojure repl has started
```
(use 'figwheel-sidecar.repl-api)
(start-figwheel!)
(cljs-repl)
```

Figwheel will automatically push cljs changes to the browser.

Wait a bit, then browse to [http://localhost:3450](http://localhost:3450).

## Production Build

To compile clojurescript to javascript:

```
lein clean
lein cljsbuild once min
```

## Deploying to Clojars

Make sure code is committed to master

```
lein deploy clojars
```

This will automatically increment the version number
