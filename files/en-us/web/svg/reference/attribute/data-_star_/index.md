---
title: data-*
slug: Web/SVG/Reference/Attribute/data-*
page-type: svg-attribute
browser-compat: svg.global_attributes.data
sidebar: svgref
---

The **`data-*`** SVG attributes are called custom data attributes. They let SVG markup and its resulting DOM share information that standard attributes can't, usually for scripting purposes. Their custom data are available via the {{domxref("SVGElement")}} interface of the element the attributes belong to, with the {{domxref("SVGElement.dataset")}} property.

The `*` can be replaced by any characters allowed in [XML's rules for names](https://www.w3.org/TR/xml/#NT-Name), with the following restrictions:

- Can't start with `xml`.
- No semicolons (`;`, `U+003A`).
- No capital `A` to `Z` letters.

> [!NOTE]
> The {{domxref("SVGElement.dataset")}} property is a {{domxref("DOMStringMap")}} that provides the attribute `data-test-value` via `SVGElement.dataset.testValue`. Hyphen characters (`-`, `U+002D`) are removed and the next letter is capitalized, resulting in the {{Glossary("camel_case", "camel case")}} format.

You can use this attribute with any SVG element.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- {{domxref("SVGElement")}}
- The {{domxref("SVGElement.dataset")}} property used to access these attributes from scripts.
- [Using data attributes](/en-US/docs/Web/HTML/How_to/Use_data_attributes)
