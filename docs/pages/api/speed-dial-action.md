---
filename: /packages/material-ui-lab/src/SpeedDialAction/SpeedDialAction.js
---

<!--- This documentation is automatically generated, do not try to edit it. -->

# SpeedDialAction API

<p class="description">The API documentation of the SpeedDialAction React component. Learn more about the props and the CSS customization points.</p>

## Import

```js
import SpeedDialAction from '@material-ui/lab/SpeedDialAction';
// or
import { SpeedDialAction } from '@material-ui/lab';
```

You can learn more about the difference by [reading our guide](/guides/minimizing-bundle-size/).



## Props

| Name | Type | Default | Description |
|:-----|:-----|:--------|:------------|
| <span class="prop-name">ButtonProps</span> | <span class="prop-type">object</span> |  | Props applied to the [`Button`](/api/button/) component. |
| <span class="prop-name">classes</span> | <span class="prop-type">object</span> |  | Override or extend the styles applied to the component. See [CSS API](#css) below for more details. |
| <span class="prop-name">delay</span> | <span class="prop-type">number</span> | <span class="prop-default">0</span> | Adds a transition delay, to allow a series of SpeedDialActions to be animated. |
| <span class="prop-name required">icon&nbsp;*</span> | <span class="prop-type">node</span> |  | The Icon to display in the SpeedDial Floating Action Button. |
| <span class="prop-name">TooltipClasses</span> | <span class="prop-type">object</span> |  | Classes applied to the [`Tooltip`](/api/tooltip/) element. |
| <span class="prop-name">tooltipOpen</span> | <span class="prop-type">bool</span> | <span class="prop-default">false</span> | Make the tooltip always visible when the SpeedDial is open. |
| <span class="prop-name">tooltipPlacement</span> | <span class="prop-type">'bottom-end'<br>&#124;&nbsp;'bottom-start'<br>&#124;&nbsp;'bottom'<br>&#124;&nbsp;'left-end'<br>&#124;&nbsp;'left-start'<br>&#124;&nbsp;'left'<br>&#124;&nbsp;'right-end'<br>&#124;&nbsp;'right-start'<br>&#124;&nbsp;'right'<br>&#124;&nbsp;'top-end'<br>&#124;&nbsp;'top-start'<br>&#124;&nbsp;'top'</span> | <span class="prop-default">'left'</span> | Placement of the tooltip. |
| <span class="prop-name required">tooltipTitle&nbsp;*</span> | <span class="prop-type">node</span> |  | Label to display in the tooltip. |

The component cannot hold a ref.

Any other props supplied will be provided to the root element ([Tooltip](/api/tooltip/)).

## CSS

- Style sheet name: `MuiSpeedDialAction`.
- Style sheet details:

| Rule name | Global class | Description |
|:-----|:-------------|:------------|
| <span class="prop-name">button</span> | <span class="prop-name">MuiSpeedDialAction-button</span> | Styles applied to the `Button` component.
| <span class="prop-name">buttonClosed</span> | <span class="prop-name">MuiSpeedDialAction-buttonClosed</span> | Styles applied to the `Button` component if `open={false}`.

You can override the style of the component thanks to one of these customization points:

- With a rule name of the [`classes` object prop](/customization/components/#overriding-styles-with-classes).
- With a [global class name](/customization/components/#overriding-styles-with-global-class-names).
- With a theme and an [`overrides` property](/customization/globals/#css).

If that's not sufficient, you can check the [implementation of the component](https://github.com/mui-org/material-ui/blob/master/packages/material-ui-lab/src/SpeedDialAction/SpeedDialAction.js) for more detail.

## Inheritance

The props of the [Tooltip](/api/tooltip/) component are also available.
You can take advantage of this behavior to [target nested components](/guides/api/#spread).

## Demos

- [Speed Dial](/components/speed-dial/)

