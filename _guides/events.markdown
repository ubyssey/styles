---
title: Events
slug: events
---

# Events

## Event Date Box

Used inside event widgets and components. Displays the month and day in condensed form. Can be used with or without a border.

### Preview

<div class="guide__preview">
  <div class="c-event-date c-event-date--bordered">
    <div class="c-event-date__month">Jun</div>
    <div class="c-event-date__day">26</div>
  </div>
</div>

### HTML

```html
<div class="c-event-date c-event-date--bordered">
  <div class="c-event-date__month">Jun</div>
  <div class="c-event-date__day">26</div>
</div>
```

### SASS

```scss
.c-event-date {
  // Structure
  width: 3rem;
  padding-top: 0.5rem;
  padding-bottom: 0.5rem;

  // Text
  text-align: center;
}

.c-event-date--bordered {
  // Border
  border: 1px solid $color-border-gray-light;
  border-radius: 2px;
}

.c-event-date__month {
  // Structure
  margin-bottom: 0.25rem;

  // Text
  font-weight: $font-weight-semi-bold;
  font-size: 10px;
  letter-spacing: 1px;
  text-transform: uppercase;
  color: $color-text-gray-light;
  line-height: 1em;
}

.c-event-date__day {
  // Text
  color: $color-accent-blue;
  font-size: 24px;
  font-weight: $font-weight-semi-bold;
  line-height: 0.85em;
}
```

## Event Box

An event box is a versatile component for displaying events across our digital platform. It is intended to offer a brief representation of an event, and works well as a supplement alongside primary content. The box can be displayed with or without an image and in several size variations.

### Preview

<div class="guide__preview">
  <div class="c-event">
    <div class="c-event__image" style="background-image: url('{{ site.url }}/images/event.jpg')"></div>
    <div class="c-event__meta">
      <div class="c-event-date">
        <div class="c-event-date__month">Jun</div>
        <div class="c-event-date__day">26</div>
      </div>
      <div class="c-event__info">
        <h3 class="c-event__title">Jacob Collier</h3>
        <p class="c-event__time">Tuesday, June 27 at 9 PM - 11:30 PM</p>
        <p class="c-event__location">HR MacMillan Space Center</p>
      </div>
    </div>
  </div>

  <br/>

  <div class="c-event">
    <div class="c-event__meta">
      <div class="c-event-date">
        <div class="c-event-date__month">Jun</div>
        <div class="c-event-date__day">26</div>
      </div>
      <div class="c-event__info">
        <h3 class="c-event__title">Jacob Collier</h3>
        <p class="c-event__time">Tuesday, June 27 at 9 PM - 11:30 PM</p>
        <p class="c-event__location">HR MacMillan Space Center</p>
      </div>
    </div>
  </div>
</div>

### HTML

```html
<div class="c-event">
  <div class="c-event__image" style="background-image: url('{{ site.url }}/images/event.jpg')"></div>
  <div class="c-event__meta">
    <div class="c-event-date">
      <div class="c-event-date__month">Jun</div>
      <div class="c-event-date__day">26</div>
    </div>
    <div class="c-event__info">
      <h3 class="c-event__title">Jacob Collier</h3>
      <p class="c-event__time">Tuesday, June 27 at 9 PM - 11:30 PM</p>
      <p class="c-event__location">HR MacMillan Space Center</p>
    </div>
  </div>
</div>
```

### SASS

```scss
.c-event {
  // Background
  background: #fff;

  // Border
  border: solid 0.5px #e6e6e6;
  box-shadow: 0 1px 1px 0 rgba(0, 0, 0, 0.05);
  border-radius: 2px;

  // Text
  font-family: 'ub-lft-etica';
}

.c-event__image {
  position: relative;
  padding-top: 60%;
  background-position: center;
  background-size: cover;
}

.c-event__meta {
  // Structure
  display: flex;
  padding-top: 1rem;
  padding-bottom: 1rem;
  padding-left: 0.75rem;
  padding-right: 0.75rem;
}

.c-event__info {
  // Structure
  flex: 1;
  padding-left: 0.5rem;

  // Text
  line-height: 1.4em;
}

.c-event__title {
  // Text
  font-weight: $font-weight-semi-bold;
}

.c-event__time,
.c-event__location {
  // Text
  font-size: 13px;
  color: $color-text-gray;
}

.c-event__time {
  // Text
  font-weight: $font-weight-semi-bold;
}
```
