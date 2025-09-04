#  Beginner’s Guide to NestJS

*A Simple Starter Toolkit for New Learners*

---

##  Introduction

NestJS is a progressive **Node.js framework** for building server-side applications.
It uses **TypeScript** (a typed version of JavaScript) and takes inspiration from **Angular**, making it structured, testable, and maintainable.

Think of it as **Express.js on steroids** — it has all the flexibility of Express but adds structure and powerful features for building scalable apps.

In this guide, you’ll:

* Install and set up NestJS
* Build a simple **Hello World API**
* Run and test your project
* Learn enough to explore further on your own

---

##  Prerequisites

Before starting, make sure you have:

* **Node.js (>=16)** → [Download here](https://nodejs.org/)

  ```bash
  node -v
  ```

* **npm** (comes with Node.js)

  ```bash
  npm -v
  ```

* A code editor (**VS Code recommended**)

---

##  Step 1: Install NestJS CLI

The CLI helps you create and manage NestJS projects:

```bash
npm install -g @nestjs/cli
```

---

##  Step 2: Create a New Project

Run the following:

```bash
nest new hello-world
```
 Choose **npm** when asked for a package manager.
This creates a folder `hello-world` with everything set up.

---

##  Step 3: Run Your App

Navigate into the project folder and start the server:

```bash
cd hello-world
npm run start:dev
```

Open your browser at: **[http://localhost:3000](http://localhost:3000)**

You should see:

```
Hello World!
```

---

##  Step 4: Customize the Hello World

Open the file: `src/app.controller.ts`

Find the method:

```ts
@Get()
getHello(): string {
  return 'Hello World!';
}
```

Change it to:

```ts
@Get()
getHello(): string {
  return 'Hello from NestJS!';
}
```

\ Save the file → The server reloads automatically → Refresh the browser →

You should now see:

```
Hello from NestJS!
```

Congratulations — you’ve built your first NestJS API!

---

##  Step 5: Test Your API

Instead of a browser, you can test with **curl**:

```bash
curl http://localhost:3000
```

Output:

```
Hello from NestJS!
```

---

