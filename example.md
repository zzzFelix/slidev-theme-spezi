---
# try also 'default' to start simple
theme: ./
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://source.unsplash.com/collection/94734566/1920x1080
# apply any windi css classes to the current slide
class: 'text-center'
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: false
# some information about the slides, markdown enabled
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# persist drawings in exports and build
drawings:
  persist: false
# page transition
transition: slide-left
# use UnoCSS
css: unocss

colorSchema: dark
---

# Accessibility for All

## The Benefits of Inclusive Design

---

# Design for accessibility

- Users of screen readers
- Users with low vision
- Users with dyslexia
- Users with limited motor skills

---
layout: fact
---

# 1.6 billion
## 1 in 6 people experience significant disability

---
layout: quote
quote: "The design of mainstream products and/or services that are accessible to, and usable by, as many people as reasonably possible … without the need for special adaptation or specialised design."
author: "The British Standards Institute (2005)"
cite: "https://knowledge.bsigroup.com/products/design-management-systems-managing-inclusive-design-guide/standard"
---

::header::
# Inclusive design

---
layout: two-cols-header
---

::header::
# Semantic HTML

::left::

```html
<nav>
  <ul>
    <li><a href="/link">Menu item 1</a></li>
    <li><a href="/link">Menu item 2</a></li>
    <li><a href="/link">Menu item 3</a></li>
  </ul>
</nav>

<main>
  <h1>Accessibility</h1>

  <section>
    ...
  </section>
</main>
```
::right::

<v-click>
```html
<div>
  <div>
    <div><span @click="jsAction()">Item 1</span></div>
    <div><span @click="jsAction()">Item 2</span></div>
    <div><span @click="jsAction()">Item 3</span></div>
  </div>
</div>

<div>
  <span>Accessibility</span>

  <div>
    ...
  </div>
</div>
```
</v-click>


---
layout: image-right
image: 'bendy-straw.webp'
---

# Joseph Friedman and the bendy-straw
