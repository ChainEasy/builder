### 0.3.1

- Feature: Added SDK version to data sent to visual editor for improved debugging.
- Fix: Columns block: removed redundant margin-left in first column.

### 0.3.0

- No Changes.

### 0.2.3

- No Changes.

### 0.2.2

- Fix: dynamic bindings for Link URLs.
- Fix: previewing content that includes a symbol whose `model` property is a `page`.
- Fix: "Show If"/"Hide If" bindings when the initial value is `undefined`.

### 0.2.1

- No Changes.

### 0.2.0

- Sets the default `apiVersion` to `v3`.

In case you feel the need to use our older API Version `v2`, reach out to us at support@builder.io first. But you can override the default by setting `apiVersion` explicitly to `v2` as follows:

```jsx
<RenderContent apiVersion="v2" />
```

```js
getContent({ apiVersion: 'v2' });
```

More details on the Builder API Versions visit [this link](https://www.builder.io/c/docs/content-api-versions).

### 0.1.16

- No changes.

### 0.1.15

- No changes.

### 0.1.14

- No changes.

### 0.1.13

- Fix: Columns block styling & `stackColumnsAt` prop

### 0.1.12

- Fix: `RenderContent` not re-rendering when its `content` updates. This fixes Symbol rendering in the visual editor.
- Feature: `RenderContent` and `getContent` now have an `apiVersion` field that can be set to `v2` or `v3` to target specific Builder API versions. Current default is `v2`

### 0.1.11

- No changes.

### 0.1.10

- Fix: Text blocks styles (remove initial top padding)

### 0.1.9

- No changes.

### 0.1.8

- Added support for "Show If" & "Hide If" dynamic bindings to elements.

### 0.1.7

- No changes.

### 0.1.6

- Types: removed redundant `builtIn` field in `customComponents` prop types

### 0.1.5

- Feature: Global CSS Nesting (`&` operator) support

### 0.1.4

No Changes.

### 0.1.3

- Support Heatmaps
- Support Insights data filtering by URL & Device

### 0.1.2

- Fix: respect when `canTrack` is set to `false`
- Fix: issues sending session and visitor IDs with tracking events

### 0.1.1

🧨 Breaking change: we no longer provide a `node-fetch` polyfill. See [the docs](./README.md#fetch) for more information.

### 0.0.1-9

🐛 Fix: custom components were not rendering correctly
🐛 Fix: Image component's `srcSet` was not being set correctly

### 0.0.1-8

🧨 Breaking change: the format of the `customComponents` prop has changed from `[{ component, info }]` to `[{ component, ...info }]`.
See [builder-registered-components.ts](/packages/sdks/src/constants/builder-registered-components.ts) for examples of how to do so, or see the example provided for this SDK.

### 0.0.1-7

⚠️ Deprecation notice: Registering components via `registerComponent(component, info)` is now deprecated.
To register your custom components in Builder, you must now provide a `customComponents` array to the `RenderContent` component containing `[{ component, info }]`.
See [builder-registered-components.ts](/packages/sdks/src/constants/builder-registered-components.ts) for examples of how to do so, or see the example provided for this SDK.

### 0.0.1-5

First working release
