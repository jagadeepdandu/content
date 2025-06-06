---
title: <set>
slug: Web/SVG/Reference/Element/set
page-type: svg-element
browser-compat: svg.elements.set
sidebar: svgref
---

The **`<set>`** [SVG](/en-US/docs/Web/SVG) element provides a method of setting the value of an attribute for a specified duration.

It supports all attribute types, including those that cannot reasonably be interpolated, such as string and boolean values. For attributes that can be reasonably be interpolated, the {{SVGElement('animate')}} is usually preferred.

> [!NOTE]
> The `<set>` element is non-additive. The {{SVGAttr('additive')}} and {{SVGAttr('accumulate')}} attributes are not allowed, and will be ignored if specified.

## Usage context

{{svginfo}}

## Attributes

- {{SVGAttr("to")}}
  - : This attribute defines the value to be applied to the target attribute for the duration of the animation. The value must match the requirements of the target attribute.
    _Value type_: [**\<anything>**](/en-US/docs/Web/SVG/Guides/Content_type#anything); _Default value_: none; _Animatable_: **no**

## DOM Interface

This element implements the {{domxref("SVGSetElement")}} interface.

## Example

```css hidden
html,
body,
svg {
  height: 100%;
}
```

```html
<svg viewBox="0 0 10 10" xmlns="http://www.w3.org/2000/svg">
  <style>
    rect {
      cursor: pointer;
    }
    .round {
      rx: 5px;
      fill: green;
    }
  </style>

  <rect id="me" width="10" height="10">
    <set attributeName="class" to="round" begin="me.click" dur="2s" />
  </rect>
</svg>
```

{{EmbedLiveSample('Example', 150, '100%')}}

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- {{SVGAttr("attributeName")}} attribute
- [Animation timing attributes](/en-US/docs/Web/SVG/Reference/Attribute#animation_timing_attributes), including {{SVGAttr("begin")}}, {{SVGAttr("dur")}}, {{SVGAttr("end")}}, {{SVGAttr("min")}}, {{SVGAttr("max")}}, {{SVGAttr("restart")}}, {{SVGAttr("repeatCount")}}, {{SVGAttr("repeatDur")}}, and {{SVGAttr("fill")}}.
- {{SVGElement("animate")}}
