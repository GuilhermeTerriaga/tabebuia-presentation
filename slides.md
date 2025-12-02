---
# try also 'default' to start simple
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://cover.sli.dev
# some information about your slides (markdown enabled)
title: Tabebuia
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# apply UnoCSS classes to the current slide
class: text-center
# https://sli.dev/features/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations.html#slide-transitions
transition: slide-left
# enable MDC Syntax: https://sli.dev/features/mdc
mdc: true
# duration of the presentation
duration: 10min
---

# Welcome to Tabebuia

The tar implementation made with elixir 

<div @click="$slidev.nav.next" class="mt-12 py-1" hover:bg="white op-10">
  Press Space for next page <carbon:arrow-right />
</div>

<div class="abs-br m-6 text-xl">
  <button @click="$slidev.nav.openInEditor()" title="Open in Editor" class="slidev-icon-btn">
    <carbon:edit />
  </button>
  <a href="https://github.com/slidevjs/slidev" target="_blank" class="slidev-icon-btn">
    <carbon:logo-github />
  </a>
</div>

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

---
transition: fade-out
---

# What is Tabebuia?

Tabebuia is a implementation of tar using functional programming.

- **CLI** - you can call it from cli
- **Lib interface** - you can use it as a library
- **Read and unroll** - it can read tar files and untar them
- **Roll** - it can create tar files
<br>
<br>

<!--
You can have `style` tag in markdown to override the style for the current page.
Learn more: https://sli.dev/features/slide-scope-style
-->

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

<!--
Here is another comment.
-->

---
transition: slide-up
level: 1
layout: image-left
image: ipe-pod.jpg
---

# Why the name?

Tabebuia is the genus of Ipê trees and the Ipê seeds are compressed together in pods just like some files grouped in a tar file.
Also the seeds themselves have some kind of involucre that reminds me of compression.


---
layout: image
image: ./Iperosaibira.jpg
hideInToc: true
---
---
layout: image-left
layoutClass: gap-16
hideInToc: true
image: https://cover.sli.dev
---

# Table of contents

<Toc text-sm minDepth="1" maxDepth="2" />

---
layout: image-left
image: https://cover.sli.dev
---

# Code structure 

The main module is Tabebuia itself, it have three functions
- create/2
- list/1 - to be implemented
- extract/2 - to be implemented

All the hard work are done by other modules:
- Builder
- Collector
- Header

---
layout: image-left
image: https://cover.sli.dev
---

What is a tarfile?


Tarfile is also called tarball that consists of a series of file objects. Each object is made up of a 512-byte header, followed by as many 512-byte blocks as are needed to contain the file contents, rounded up to the nearest full block. After the final file object there is at least two consecutive 512-bytes blocks of zero-filled records.

---
layout: image-left
image: https://cover.sli.dev
---

# Demo 

Let's try!

---
layout: center
class: text-center
---

# Learn More
This slide was create with sli.dev
[Documentation](https://sli.dev) · [GitHub](https://github.com/slidevjs/slidev) · [Showcases](https://sli.dev/resources/showcases)

Documentation:
[Tabebuia](https://hexdocs.pm/tabebuia/0.1.0/Tabebuia.html)


