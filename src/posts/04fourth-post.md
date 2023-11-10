---
title: Routing
description: Mastering Routing in SvelteKit - A File-Based Approach
date: '2023-11-09'
categories:
  - sveltekit
  - svelte
published: true
---

# Mastering Routing in SvelteKit: A File-Based Approach

Welcome back, everyone! In our previous discussions, we explored how to create a new SvelteKit project and examined the project's folder structure. Now, it's time to dive deep into one of the most essential features that SvelteKit has to offer – routing.

SvelteKit boasts a unique and efficient file system-based routing mechanism. What this means is that the URL paths accessible in the browser are defined by files and folders within your codebase. Let's explore this concept with some practical examples.

## Setting Up a SvelteKit Project

Before we delve into the routing intricacies, let's set up a SvelteKit project. Here's a quick guide to get you started:

1. Open your preferred code editor, and navigate to your desired project directory.

2. Create a new SvelteKit project using the following command:

   ```bash
   npm create svelte@latest my-svelte-kit-project
   ```

3. Once the project is generated, navigate to your project folder:

   ```bash
   cd my-svelte-kit-project
   ```

4. Install project dependencies:

   ```bash
   npm install
   ```

Great! With the project set up, we can now explore the file-based routing mechanism in SvelteKit.

## Understanding File-Based Routing

In SvelteKit, every route is defined by a specific set of conventions:

1. **Route Placement:** All routes must be placed inside a folder named `routes` within the `src` directory.

2. **File Naming:** Each file that corresponds to a route in your application must be named `page.svelte`.

3. **Folder Structure:** Each folder within the `routes` directory corresponds to a path segment in the browser's URL.

These conventions play a pivotal role in determining the routes in your application. Now, let's see these conventions in action with practical examples.

### Scenario 1: Home Route

For our first scenario, we want to create a simple route that is displayed when users visit the root of our website, which, in this case, is `localhost:5173`.

Here's how we implement this:

1. Create a folder named `routes` within the `src` directory. This is the default location for all routes.

2. Inside the `routes` folder, create a new file named `page.svelte`.

3. In `page.svelte`, add a basic HTML structure:

   ```html
   <h1>Welcome Home</h1>
   ```

By following these conventions, we have successfully created our first route in SvelteKit. To see it in action, run the following command:

```bash
npm run dev
```

You should now see the "Welcome Home" message in your browser when you visit `localhost:5173`.

### Scenario 2: Additional Routes

For the next scenario, let's create two additional routes: one for the "About" page and another for the "Profile" page.

1. Inside the `routes` folder, create a new folder named `about`.

2. Inside the `about` folder, create a `page.svelte` file and add the following content:

   ```html
   <h1>About Me</h1>
   ```

3. Create another folder named `profile` inside the `routes` directory.

4. Inside the `profile` folder, create a `page.svelte` file and add the following content:

   ```html
   <h1>My Profile</h1>
   ```

By adhering to the conventions we discussed, you've effortlessly defined the routes for the "About" and "Profile" pages. If you visit `localhost:5173/about`, you'll see the "About Me" message. Likewise, `localhost:5173/profile` will display the "My Profile" content.

Moreover, if you enter a URL that doesn't correspond to a file in the `routes` folder, SvelteKit will automatically respond with a 404 "Not Found" response. You don't need to explicitly handle non-matching routes.

In summary, SvelteKit's file-based routing approach eliminates the need for a router configuration and makes route creation straightforward and intuitive. This is just the beginning of our journey into SvelteKit's routing capabilities, and there's much more to explore.

Stay tuned for future articles where we'll dive deeper into SvelteKit's routing features and explore its full potential. Happy coding!
