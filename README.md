# Getting started

To get started the quick and easy way, simply clone this repo. This options has the added value of additional file configs, vscode settings, etc. 

...or do it on your own via the steps below.

## Manually getting started

1. Create Vite + Vue 3 project as described [here](https://vitejs.dev/guide/)

   ```bash
   yarn create vite
   ```

1. Add Eslint + Prettier support

   - Install packages

     ```bash
     yarn add -D prettier eslint @typescript-eslint/eslint-plugin @typescript-eslint/parser @vue/eslint-config-typescript eslint-config-prettier eslint-plugin-prettier eslint-plugin-vue vue-eslint-parser
     ```

   - Create files and configs

     ```bash
     touch .eslintrc
     touch .prettierrc
     ```

   - Update packages scripts

     ```json
     "lint": "eslint . --ext .ts,.js,.vue --experimental-specifier-resolution=node"
     ```

1.

# Fire things up 🔥

Run `yarn dev`

# Vue 3 + TypeScript + Vite

This template should help get you started developing with Vue 3 and TypeScript in Vite. The template uses Vue 3 `<script setup>` SFCs, check out the [script setup docs](https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup) to learn more.

## Recommended IDE Setup

- [VS Code](https://code.visualstudio.com/) + [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (and disable Vetur) + [TypeScript Vue Plugin (Volar)](https://marketplace.visualstudio.com/items?itemName=Vue.vscode-typescript-vue-plugin).

## Type Support For `.vue` Imports in TS

TypeScript cannot handle type information for `.vue` imports by default, so we replace the `tsc` CLI with `vue-tsc` for type checking. In editors, we need [TypeScript Vue Plugin (Volar)](https://marketplace.visualstudio.com/items?itemName=Vue.vscode-typescript-vue-plugin) to make the TypeScript language service aware of `.vue` types.

If the standalone TypeScript plugin doesn't feel fast enough to you, Volar has also implemented a [Take Over Mode](https://github.com/johnsoncodehk/volar/discussions/471#discussioncomment-1361669) that is more performant. You can enable it by the following steps:

1. Disable the built-in TypeScript Extension
   1. Run `Extensions: Show Built-in Extensions` from VSCode's command palette
   2. Find `TypeScript and JavaScript Language Features`, right click and select `Disable (Workspace)`
2. Reload the VSCode window by running `Developer: Reload Window` from the command palette.
