## visible
- Overflow content is not clipped and may be visible outside the element's padding box. The element box is not a scroll container. This is the default value of the overflow property.

## hidden
- Overflow content is clipped at the element's padding box. There are no scroll bars, and the clipped content is not visible (i.e., clipped content is hidden), but the content still exists. User agents do not add scroll bars and also do not allow users to view the content outside the clipped region by actions such as dragging on a touch screen or using the scroll wheel on a mouse. The content can be scrolled programmatically (for example, by linking to anchor text, by tabbing to a hidden yet focusable element, or by setting the value of the scrollLeft property or the scrollTo() method), in which case the element box is a scroll container.

## clip
- Overflow content is clipped at the element's overflow clip edge that is defined using the overflow-clip-margin property. As a result, content overflows the element's padding box by the <length> value of overflow-clip-margin or by 0px if not set. Overflow content outside the clipped region is not visible, user agents do not add a scroll bar, and programmatic scrolling is also not supported. No new formatting context is created. To establish a formatting context, use overflow: clip along with display: flow-root. The element box is not a scroll container.

## scroll
- Overflow content is clipped at the element's padding box, and overflow content can be scrolled into view using scroll bars. User agents display scroll bars whether or not any content is overflowing, so in the horizontal and vertical directions if the value applies to both directions. The use of this keyword, therefore, can prevent scroll bars from appearing and disappearing as content changes. Printers may still print overflow content. The element box is a scroll container.

## auto
- Overflow content is clipped at the element's padding box, and overflow content can be scrolled into view using scroll bars. Unlike scroll, user agents display scroll bars only if the content is overflowing. If content fits inside the element's padding box, it looks the same as with visible but still establishes a new formatting context. The element box is a scroll container.

```bash
/* Keyword values */
overflow: visible;
overflow: hidden;
overflow: clip;
overflow: scroll;
overflow: auto;
overflow: hidden visible;

/* Global values */
overflow: inherit;
overflow: initial;
overflow: revert;
overflow: revert-layer;
overflow: unset;
```
