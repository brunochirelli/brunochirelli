---
title: How to Organize Component Text
slug: how-to-organize-component-text
tag: react,pattern
---

## Why

Thinking in a way to consolidate all texts in a component, I came to this idea of organization:

```jsx
const content = {
  title: "Component Title",
  disclaimer: "Disclaimer",
  info: "Some info",
};

const SomeComponent = ({
  title = "Component title",
  disclaimer = "Disclaimer",
  info = "Some Info",
}) => {
  return (
    <div>
      <h1>{title}</h1>
      <p>{disclaimer}</p>
      <info>{info}</info>
    </div>
  );
};
```

Maybe it's a good practice cause all of the component text is in one place, making adjustments far easy than scrolling down the entire implementation.

What do you think about it? Leave a reply!
