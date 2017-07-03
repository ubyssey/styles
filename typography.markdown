---
title: Typography
slug: typography
layout: default
---

# Typography

## Typefaces

*The Ubyssey* makes use of three main typefaces throughout our website and digital applications.

<a class="button is-primary" href="{{ "/files/fonts.zip" | prepend: site.baseurl }}">Download font pack (297 KB)</a>

**Minion Pro**

`ub-minion-pro`

Minion Pro is reserved for headlines, image captions and other components that require a classic yet legible type. We currently use two weights, `600` and `800`.

### Sample

<p style="font-family: 'ub-minion-pro'; color: #2b2b2b;">
  <span style="font-size: 32px; font-weight: 800;">The quick brown fox jumps over the lazy dog</span><br/>
  <span style="font-size: 24px; font-weight: 800;">The quick brown fox jumps over the lazy dog</span><br/>
  <span style="font-size: 16px; line-height: 32px;">The quick brown fox jumps over the lazy dog</span>
</p>

---

**LFT Etica**

`ub-lft-etica`

LFT Etica is our sans-serif workhorse. It's used mainly for user interface components, labels and secondary content.

### Sample

<p style="font-family: 'ub-lft-etica'; color: #2b2b2b;">
  <span style="font-size: 32px; font-weight: 800;">The quick brown fox jumps over the lazy dog</span><br/>
  <span style="font-size: 24px; font-weight: 800;">The quick brown fox jumps over the lazy dog</span><br/>
  <span style="font-size: 16px; line-height: 32px;">The quick brown fox jumps over the lazy dog</span>
</p>

---

**Georgia**

`Georgia`

Georgia is used for article body text due to its high readability and consistency across platforms.

### Sample

<p style="font-family: 'Georgia'; color: #2b2b2b;">
  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam egestas viverra massa, tincidunt gravida diam laoreet ullamcorper. Vestibulum sed pharetra neque. Nunc sagittis enim nec sapien euismod, eget posuere mi cursus. Nam a lorem ligula. Maecenas fringilla elementum dui.
</p>

---

## Headlines

### Headline 1

<div class="preview">
<h1 class="c-headline c-headline--1">New housing program approved as a strategy to recruit and retain staff and faculty</h1>
</div>

### Headline 2

<div class="preview">
<h2 class="c-headline c-headline--2">New housing program approved as a strategy to recruit and retain staff and faculty</h2>
</div>

### Headline 3

<div class="preview">
<h3 class="c-headline c-headline--3">New housing program approved as a strategy to recruit and retain staff and faculty</h3>
</div>

### Headline 4

<div class="preview">
<h4 class="c-headline c-headline--4">New housing program approved as a strategy to recruit and retain staff and faculty</h4>
</div>

### SASS

```scss
.c-headline {
  // Text
  font-family: 'ub-minion-pro';
  font-weight: 800;
  color: $color-text-black;
  line-height: 1.2em;
}

h1.c-headline { font-size: 36px; }
h2.c-headline { font-size: 28px; }
h3.c-headline { font-size: 26px; }
h4.c-headline { font-size: 18px; }
```

---

## Body Text

Article body text is `Georgia/17px` with off-black colouring and a medium line height.

### Sample

<div class="preview c-article__content">
<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam egestas viverra massa, tincidunt gravida diam laoreet ullamcorper. Vestibulum sed pharetra neque. Nunc sagittis enim nec sapien euismod, eget posuere mi cursus. Nam a lorem ligula. Maecenas fringilla elementum dui. Vivamus a rutrum metus. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Duis eget eros vel neque ornare pharetra a vitae lorem. Aliquam luctus dignissim nulla vel varius.</p><p>Etiam vitae enim ex. Vivamus commodo interdum elit, a eleifend nibh ultricies a. Sed bibendum porttitor felis, vitae dictum odio. Duis a rhoncus ex. Suspendisse nisi neque, aliquet sit amet aliquet sed, finibus eu nibh. Proin ornare venenatis lobortis. Aliquam dignissim viverra ex id sodales. Pellentesque non est id est facilisis feugiat quis eu urna. Proin commodo nunc pretium bibendum tincidunt.</p>
</div>

### SASS

```scss
.c-article__content > p {
  // Structure
  margin-bottom: 1.4rem;
  max-width: 585px;

  // Text
  font-family: 'Georgia';
  font-size: 17px;
  color: $color-text-default;
  line-height: 1.625rem;
}
```

---

## Links

Anchor links are underlined and coloured with *Ubyssey* blue.

### Sample

<div class="preview c-article__content">
<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam egestas viverra massa, tincidunt gravida diam laoreet ullamcorper. Vestibulum sed pharetra neque. Nunc sagittis enim nec sapien euismod, eget posuere mi cursus. Nam a lorem ligula. <a>Maecenas fringilla elementum dui. Vivamus a rutrum metus</a>. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Duis eget eros vel neque ornare pharetra a vitae lorem. Aliquam luctus dignissim nulla vel varius.</p>
</div>

### SASS

```scss
.c-article__content > p a {
  // Text
  color: $color-accent-blue;
  text-decoration: underline;
}
```
