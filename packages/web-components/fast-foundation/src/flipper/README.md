---
id: flipper
title: fast-flipper
sidebar_label: flipper
custom_edit_url: https://github.com/microsoft/fast/edit/master/packages/web-components/fast-foundation/src/flipper/README.md
---

The flipper component is most often used to page through blocks of content or collections of ui elements. As flippers are often a supplemental form of navigation, the flippers are hidden by default to avoid duplicate keyboard interaction. Passing an attribute of `aria-hidden="false"` will expose the flippers to assistive technology.

## Usage

```html live
<fast-design-system-provider use-defaults>
    <fast-flipper direction="previous"></fast-flipper>
</fast-design-system-provider>
```

## Applying custom styles

```ts
import { customElement } from "@microsoft/fast-element";
import { Flipper, FlipperTemplate as template } from "@microsoft/fast-foundation";
import { FlipperStyles as styles } from "./flipper.styles";

@customElement({
    name: "fast-flipper",
    template,
    styles,
})
export class FASTFlipper extends Flipper {}
```