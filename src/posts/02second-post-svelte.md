---
title: 02 Creating Your First Svelte Application
description: Creating Your First Svelte Application
date: '2023-11-15'
categories:
  - svelte
coverImage: /images/svelte.webp
published: true
---

### Creating Your First Svelte Application

In this tutorial, we'll walk through the process of setting up your development environment and creating your very first Svelte application. Svelte is a component framework designed for building high-performance web applications, and we'll be focusing on the core concepts of Svelte in this series.

### Setting Up Your Development Environment

Before we dive into the code, let's make sure your development environment is set up correctly. You'll need to have Node.js installed and a text editor of your choice. Here's how you can set it up:

1. Node.js Installation:

   - Go to nodejs.org.
   - Download and install the latest stable release of Node.js.
   - If you already have it installed, make sure to update it to the latest version.

2. Text Editor:

   - I recommend using Visual Studio Code (VS Code). You can download and install it from code.visualstudio.com.
   - After installing VS Code, open the Extensions tab and install the following extensions:
     Svelte for VS Code
     Svelte 3 Snippets
     These extensions provide syntax highlighting, code snippets, linting, formatting support, auto-completion, and more features tailored for Svelte development.

Now that your environment is set up, let's address an important point before we proceed with the code.

### Svelte vs. Svelte Kit

In the world of Svelte, there are two key terms to be aware of: Svelte and Svelte Kit.

- Svelte Kit: This is an application framework powered by Svelte. Similar to frameworks like Next.js (powered by React) and Nuxt.js (powered by Vue), Svelte Kit adds features like routing and server-side rendering, suitable for medium to large-scale applications.

For this tutorial series, we're focusing solely on learning the concepts of Svelte and not Svelte Kit. It's advisable to grasp Svelte before diving into Svelte Kit. Now, let's proceed with creating our first Svelte application.

### Creating a New Svelte Project

- Create a folder for your Svelte workspace. In this example, I've named it "svelte" and opened VS Code inside that folder.

- Open the terminal and run the following command to create a new Svelte project named "hello-world":

```
npx degit sveltejs/template hello-world
This command clones the Svelte template repository without the git history.
```

- Navigate inside the project folder:

```
cd hello-world
```

- Install dependencies:

```
yarn
```

or

```
npm install
```

- Run the development server:

```
yarn dev
```

or

```
npm run dev
```

- Open the provided link in your browser (usually `localhost:5000`). You should see your "Hello World" Svelte application up and running.

Congratulations! You've just created your first Svelte application. In the next blog post, we'll explore the folder structure of the project.
