# `n` – unified command to launch a Node package manager

**TL;DR: Forget about package manager names — just always use `n`:**
```shell
n i && n build && n start; n add my-package
```

## Installation

```shell
curl -fsSL https://raw.githubusercontent.com/MurzNN/n/refs/heads/main/bin/n -o ~/.local/bin/n && chmod +x ~/.local/bin/n
```

## Problem: Node.js has too many package managers!

Yeah, we have not only [NPM](https://www.npmjs.com/), but also [Yarn](https://yarnpkg.com/), [PNPM](https://pnpm.io/), [Bun](https://bun.sh/), and even [Volta](https://volta.sh/), [Rush](https://rushjs.io/), [Lerna](https://lerna.js.org/), [Bit](https://bit.dev/), [Tnpm](https://tnpm.js.org/), and many others.

And when you download a new Node.js project and want to run it, learning a single command like `npm i && npm run start` is no longer enough!

Instead, you have to check which package manager this specific project uses and type the correct command to install dependencies, like this:

```
[npm|pnpm|yarn] i
```

## Solution: Let's use a single short command `n` to launch any package manager!

Why should we always have to manually check or remember which package manager is used in the current directory?

Let's just remember a single short command `n` to interact with the current package manager! It autodetects the right package manager and runs the correct one. So, just learn these commands:

- Install dependencies
  ```shell
  n i
  ```

- Build the project
  ```shell
  n build
  ```

- Start the project
  ```shell
  n start
  ```

And forget about always typing `npm/yarn/pnpm/whateverelse`!
