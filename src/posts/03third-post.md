---
title: Project Structure
description: Understanding the Structure of a SvelteKit Project
date: '2023-11-09'
categories:
  - sveltekit
  - svelte
published: true
---

SvelteKit is known for its simplicity and ease of use when creating web applications. Before diving into the core concepts and features, it's crucial to understand the basic structure of a SvelteKit project. In this article, we'll walk you through the files and folders that are typically present in a generated SvelteKit project.

### Exploring the Project Structure

To get started, let's take a look at the structure of a typical SvelteKit project. I have opened a "Hello World" project in Visual Studio Code, and at the root level, we can find four folders and 11 files (excluding the `.vscode` folder).

### `package.json`

The `package.json` file is a critical piece of the project. It contains information about the project's dependencies and scripts. In a SvelteKit project, you will find dependencies like `sveltekit` and `svelte`, which are the core packages. The version of SvelteKit may vary depending on when you're watching this video, but the core concepts remain the same. Additionally, you'll find tools like `vite` for building, `eslint` for linting, and `prettier` for code formatting.

In simple terms, `eslint` highlights warnings and errors in your code, while `prettier` ensures your code is well-formatted and easy to read. The `package.json` file also includes a list of scripts for various tasks, such as development, building, linting, and formatting.

### `package-lock.json`

The `package-lock.json` file ensures the consistent installation of project dependencies. You don't need to worry about it, as it's automatically generated.

### `gitignore`, `.npmrc`, and `README`

These three files, namely `.gitignore`, `.npmrc`, and `README`, are not directly related to the SvelteKit application but serve important purposes. `.gitignore` is used for version control with Git, `.npmrc` enforces Node.js and npm versions, and `README` contains instructions related to running, building, and deploying the application.

### `svelte.config.js`

The `svelte.config.js` file is the SvelteKit configuration file. It exports a config object used by other tools that integrate with Svelte. At this point, it includes one configuration for adapters, which are small plugins responsible for generating output for deployment. As a beginner, you don't need to worry about this in detail.

### `vite.config.js`

`vite.config.js` is the configuration file for Vite, the underlying build tool for your SvelteKit project. SvelteKit projects are essentially Vite projects with the SvelteKit/Wind configuration. You can specify additional Vite plugins in this file.

### `.eslintrc.js`

The `.eslintrc.js` file is the configuration file for ESLint, a popular JavaScript linter. It extends the recommended ESLint rules and adds Svelte as a plugin. Additionally, there's an `.eslintignore` file to specify files that should be ignored during linting.

### `.prettierrc.js` and `.prettierignore`

`.prettierrc.js` is Prettier's configuration file, while `.prettierignore` contains a list of files to be ignored during code formatting.

## Examining the Folders

Now, let's delve into the folders present in your SvelteKit project.

### `.sveltekit`

The `.sveltekit` folder is generated when you run either the development or build scripts. It serves as the source folder for your SvelteKit application. You don't need to worry about this folder during development as it's Git-ignored.

### `node_modules`

`node_modules` is where all your project dependencies are installed. It's generated when you run `npm install` and is also Git-ignored.

### `static`

The `static` folder contains static assets that should be served as-is, such as `favicon.png` or `robots.txt`. These assets are not processed by the build tools and are directly served to the client.

### `src` (The Heart of the Project)

The `src` folder is the most important part of your project and contains the following subfolders:

#### `routes`

The `routes` folder is responsible for handling the routing in your application. Each route corresponds to a URL, and the route files determine what content is displayed for a given URL. The main file that gets served when you visit `localhost` on port `5173` is `index.svelte`. This is also the file that you may have modified in your previous work.

#### `app.html`

`app.html` serves as the page template for your application. This template includes placeholders like `sveltekit.assets` for static assets, `sveltekit.head` for managing link and script elements, and `sveltekit.body`, which holds the rendered page content. When you visit `localhost:5173`, the content from `index.svelte` replaces the `sveltekit.body` placeholder, resulting in the final HTML document you see in your browser.

If you inspect the element in the HTML, you'll notice the `body` tag with a `data-svelte-kit-preload-data` attribute and a `div` tag with `style` set to `display: contents`. These are generated based on the content from `index.svelte`.

## Understanding the Routing

As you might have guessed, the `routes` folder is the heart of the routing feature in SvelteKit. However, we won't dive deep into routing in this article; that's a topic we'll explore in detail in the next section of this series.

In summary, a SvelteKit project consists of various files and folders that play essential roles in building and running your application. Understanding this structure will provide a solid foundation for your journey with SvelteKit.

In the next section, we'll dive into the details of routing and how the `routes` folder drives the navigation within your SvelteKit application. Stay tuned for more exciting insights!

---

This blog post provides an overview of the structure of a SvelteKit project, breaking down the purpose of each file and folder. It also hints at the significance of the `routes` folder, which we'll explore in detail in the next section. The information is organized in a more structured and readable format, making it suitable for a blog post.
