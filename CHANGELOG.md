## v3.2.1 (2021-08-01)

- Fix `Popup` unmounting logic to unbind from container.
- Fix links to point to Leaflet 1.7.1 docs ([PR #889](https://github.com/PaulLeCam/react-leaflet/pull/889) by [zerekw](https://github.com/zerekw)).

## v3.2.0 (2021-05-15)

- Change unmounting logic for some layers, which should fix issues related to removing or updating elements.
- Make the `style` prop of `GeoJSON` mutable, this prop should be used instead of `pathOptions` (`pathOptions` can still be used but should be considered deprecated).
- Fix documentation about `bounds` prop being an instance of `LatLngBounds`.

## v3.1.0 (2021-01-30)

- Make `Pane` component compatible with React's `StrictMode` ([PR #810](https://github.com/PaulLeCam/react-leaflet/pull/810) by [zmbc](https://github.com/zmbc))
- Fix typo in API Components docs ([PR #827](https://github.com/PaulLeCam/react-leaflet/pull/827) by [arthurdenner](https://github.com/arthurdenner))

## v3.0.5 (2020-12-20)

Use `useState` hook rather than `useMemo` to store immutable values in `MapContainer` and `Pane`

## v3.0.4 (2020-12-13)

Update README

## v3.0.3 (2020-12-13)

- Document pathOptions for GeoJSON ([PR #785](https://github.com/PaulLeCam/react-leaflet/pull/785) by [bb](https://github.com/bb))
- Ensure `MapContainer` props are immutable
- Fix TypeScript definition for `MapContainer` props

## v3.0.2 (2020-11-08)

Additional fixes for panes support

## v3.0.1 (2020-11-07)

- Fixed `pane` prop support
- Use standard SPDX license name ([PR #781](https://github.com/PaulLeCam/react-leaflet/pull/781) by [nertzy](https://github.com/nertzy))

## v3.0.0 (2020-10-31)

v3 is a full rewrite of React Leaflet and contains breaking change from v2.

- Full rewrite based on [React Hooks](https://reactjs.org/docs/hooks-intro.html) (no more extending `Component`)
- Replace Flow by TypeScript for type checking
- Drop IE support (Babel config will only target the "last 2 versions" of modern browsers)
- Switch to the [Hippocratic License](https://firstdonoharm.dev/)
- The `Map` component is replaced by [`MapContainer`](https://react-leaflet.js.org/docs/api-map#mapcontainer), behaving differently
- Event handlers must be attached using the [`eventHandlers prop`](https://react-leaflet.js.org/docs/api-components#evented-behavior) rather than `on*` props, with a similar change for [path options](https://react-leaflet.js.org/docs/api-components#path-behavior) and [WMS params](https://react-leaflet.js.org/docs/api-components#wmstilelayer)
- The `react-leaflet` package only exposes a [public API](https://react-leaflet.js.org/docs/api-map) while a new package, `@react-leaflet/core`, is used to provide the [core APIs](https://react-leaflet.js.org/docs/core-introduction)
- A new documentation website using [Docusaurus v2](https://v2.docusaurus.io/) with live examples

## v3.0.0-rc.0 (2020-10-22)

- Use stable release of React v17
- Fixed incorrect example in docs ([PR #767](https://github.com/PaulLeCam/react-leaflet/pull/767) by [dipiash](https://github.com/dipiash))

## v3.0.0-beta.5 (2020-09-20)

- Remove `preserveAspectRatio` and `viewport` props from `SVGOverlay`, replaced by `attributes` prop
- Add third-party plugins page to documentation website

## v3.0.0-beta.4 (2020-08-16)

- Specify list of supported browsers ([PR #736](https://github.com/PaulLeCam/react-leaflet/pull/736) by [anajavi](https://github.com/anajavi))
- Drop Babel runtime polyfilling ([PR #739](https://github.com/PaulLeCam/react-leaflet/pull/739) by [anajavi](https://github.com/anajavi))
- Upgrade rollup plugins ([PR #740](https://github.com/PaulLeCam/react-leaflet/pull/740) by [anajavi](https://github.com/anajavi))
- Bump React dependency to v17

## v3.0.0-beta.3 (2020-08-16)

Broken build

## v3.0.0-beta.2 (2020-07-25)

- Fix `LayersControl` lifecycle logic causing layer removal
- Use terser instead of uglifyjs to minify the UMD build ([PR #735](https://github.com/PaulLeCam/react-leaflet/pull/735) by [anajavi](https://github.com/anajavi))

## v3.0.0-beta.1 (2020-07-12)

v3 is a full rewrite of React Leaflet and contains breaking change from v2.

- Full rewrite based on [React Hooks](https://reactjs.org/docs/hooks-intro.html) (no more extending `Component`)
- Replace Flow by TypeScript for type checking
- Drop IE support (Babel config will only target the "last 2 versions" of browsers)
- Switch to the [Hippocratic License](https://firstdonoharm.dev/)
- The `Map` component is replaced by [`MapContainer`](https://react-leaflet-v3.now.sh/docs/api-map#mapcontainer), behaving differently
- Event handlers must be attached using the [`eventHandlers prop`](https://react-leaflet-v3.now.sh/docs/api-components#evented-behavior) rather than `on*` props, with a similar change for [path options](https://react-leaflet-v3.now.sh/docs/api-components#path-behavior) and [WMS params](https://react-leaflet-v3.now.sh/docs/api-components#wmstilelayer)
- The `react-leaflet` package only exposes a [public API](https://react-leaflet-v3.now.sh/docs/api-map) while a new package, `@react-leaflet/core`, is used to provide the [core APIs](https://react-leaflet-v3.now.sh/docs/core-introduction)
- A new documentation website using [Docusaurus v2](https://v2.docusaurus.io/) with live examples, currently published on [react-leaflet-v3.now.sh](https://react-leaflet-v3.now.sh/)
