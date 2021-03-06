---
title: Area
description: This page describes Area.
demo:
  pages:
  - name: Main Example
    slug: example-index
  - name: Make the Tooltip Formatted (Currency)
    slug: example-formatter
  - name: Set animation speed
    slug: example-animation
  - name: Make a slice selected by default
    slug: example-selected
  - name: Example showing Get Selected value
    slug: example-get-selected
  - name: Example showing Set Selected value
    slug: example-set-selected
---

The area chart is a line chart with the isArea set that adds the fills. See the [line chart api]( ../components/line) for more details.

## Code Example

This example shows how to invoke the area chart option using the charts component. In this example
we pass a dataset with x and y axis values to make three lines.

```javascript
var dataset = [{
  data: [{
      name: 'Jan',
      value: 12
  }, {
      name: 'Feb',
      value: 11
  }, {
      name: 'Mar',
      value: 14
  }, {
      name: 'Apr',
      value: 10
  }, {
      name: 'May',
      value: 14
  }, {
      name: 'Jun',
      value: 8
  }],
  name: 'Component A'
}, {
  data: [{
      name: 'Jan',
      value: 22
  }, {
      name: 'Feb',
      value: 21
  }, {
      name: 'Mar',
      value: 24
  }, {
      name: 'Apr',
      value: 20
  }, {
      name: 'May',
      value: 24
  }, {
      name: 'Jun',
      value: 28
  }],
  name: 'Component B'
}, {
  data: [{
      name: 'Jan',
      value: 32
  }, {
      name: 'Feb',
      value: 31
  }, {
      name: 'Mar',
      value: 34
  }, {
      name: 'Apr',
      value: 30
  }, {
      name: 'May',
      value: 34
  }, {
      name: 'Jun',
      value: 38
  }],
  name: 'Component C'
}];

$('#area-example').chart({type: 'area', dataset: dataset});
```

## Accessibility

- The contrast and actual colors can be a concern for visibility impaired and color blind people. However, you can customize the color by passing higher contrast colors.

```javascript
color: '#1a1a1a'
name: 'Component C'
```

## Keyboard Shortcuts

- <kbd>Tab</kbd> You can tab into the chart area and through the legend values as each has a focus state.
- <kbd>Enter/Space</kbd> Will select the area the corresponds with the focus'd legend item.

## Upgrading from 3.X

- The area chart was added after version 3.X
