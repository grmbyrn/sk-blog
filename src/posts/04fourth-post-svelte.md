---
title: 04 Understanding Svelte Files and Getting Ready for Code
description: Understanding Svelte Files and Getting Ready for Code
date: '2023-11-15'
categories:
  - svelte
coverImage: /images/svelte.webp
published: true
---

Welcome back! Before we dive into the concepts of Svelte, there's one more topic that's crucial for you to understand – the `.svelte file`. In the previous post, I briefly mentioned this file type, and now, let's explore it a bit more.

### What is a .svelte file?

A `.svelte` file is a custom file format in Svelte where we write our code using a superset of HTML. These files are used to describe a specific portion of the user interface (UI). In our "Hello World" project, we have an app.svelte file responsible for the heading and paragraph in the UI.

So, in a nutshell, a .svelte file is responsible for a distinct part of the UI.

### Anatomy of a `.svelte` file

Each `.svelte` file consists of three main sections:

- #### Script:

  - This is where data and logic for the markup are maintained. It's essentially the JavaScript of your UI.

```
<script>
  // Data and logic go here
</script>
```

- #### Markup:
  - This section contains the HTML structure of your UI.

```
<main>
  <!-- HTML structure -->
</main>
```

- #### Style:
  - Here, you specify styles related to the HTML written in the markup section.

```
<style>
  /* CSS styles go here */
</style>
```

### The Role of `.svelte` Files in Svelte
Unlike traditional frameworks that divide the codebase into three layers, Svelte takes a different approach. In Svelte, the codebase is divided into one or more `.svelte` files. Each file is responsible for its own markup, styles, and logic.

It's essential to note that browsers don't understand `.svelte` files directly. Rollup, with the Svelte plugin, parses these files, extracts the three sections, and assembles them into a format browsers can understand.

Now that we have a bit more information about `.svelte` files, let's cover two additional points to prepare us for actual coding in the next video.

### Components in Svelte

In Svelte, a `.svelte` file represents a component. A Svelte app can contain one or more of these components. However, as beginners, we'll focus on learning the concepts using just one `.svelte` file initially. We'll keep it simple and postpone diving into multiple files and the component architecture until later in the series.

### Declarative Programming in Svelte

A significant portion of working with a `.svelte` file involves wiring up data and logic to the markup. This is about connecting the data present in the script section to the HTML present in the markup section. Svelte follows a declarative programming approach, where you let Svelte know how to bind your data to the HTML, and Svelte takes care of the rest.

This declarative approach is a fundamental concept, and we'll spend the first half of the series understanding how to express what we want the UI to look like using Svelte.

Stay tuned for the next blog post, where we'll finally start writing some code and put these concepts into practice!
