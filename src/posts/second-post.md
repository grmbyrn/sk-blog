---
title: Create Your First SvelteKit Application
description: Create Your First SvelteKit Application
date: '2023-11-09'
categories:
  - sveltekit
  - svelte
published: true
---

In this blog post, we will create our first SvelteKit application. To get started, you will need to have Node.js and a text editor of your choice installed.

### Set up your development environment

1. Install the latest stable release of Node.js from node.js.org.
2. Install a text editor of your choice. I recommend Visual Studio Code, which you can download from code.visualstudio.com.

### Create a new SvelteKit project

1. Create a new folder for your project.
2. Open Visual Studio Code inside the folder you created.
3. Run the following command in the terminal:

```
npm create svelte@latest hello-world
```

This will create a new SvelteKit project with the name `hello-world`. You can name your project whatever you like.

4. I recommend answering the prompts in the interactive CLI as follows, at least while learning:

   - **Template:** Skeleton project
   - **Types:** No
   - **Linting:** Yes
   - **Code formatting:** Yes
   - **Browser testing:** No
   - **Unit testing:** No

5. Install the dependencies using the following command:

```
npm install
```

6. Set up Git for version control (optional):

```
git init
```

7. Start the development server:

```
npm run dev --open
```

This will open your app in the browser at `http://localhost:5173`.

### Edit your app

By default, the app displays a heading that says "Welcome to SvelteKit" and a link to the documentation. To change this, edit the `src/routes/+page.svelte` file.

Replace the text Welcome to SvelteKit with the text Hello world.

When you save the file, the page content will be automatically refreshed and you should see the text "Hello world" displayed in the browser.

### Conclusion

Congratulations! You have created your first SvelteKit application.

In the next blog post, we will learn about the generated project folder structure.
