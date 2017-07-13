---
title: Inputs
slug: inputs
layout: default
---

# Inputs

## Text Input

### Preview

<div class="preview">
  <input class="c-input c-input--text" type="text" placeholder="Name" />
  <input class="c-input c-input--text" type="email" placeholder="Email address" value="contact@ubyssey.ca" />
</div>

### SASS

```scss
.c-input--text {
  // Structure
  display: block;
  padding: 0.75rem 1rem;
  margin-bottom: 1rem;
  width: 100%;
  max-width: 400px;

  // Border
  border: 1px solid $color-border-gray-light;
  border-radius: 2px;

  // Text
  font-family: 'ub-lft-etica';
  font-size: 16px;
  color: $color-text-black;

  // Extra
  transition: border-color 0.4s;

  &:focus {
    // Border
    border-color: #86c5f9;

    // Extra
    box-shadow: 0 0 2px 0px rgba(134, 197, 249, 0.15);
    outline: none;
  }
}
```
