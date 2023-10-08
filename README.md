# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

<!-- Install Redux Toolkit -->

npm install @reduxjs/toolkit
npm install react-redux

Then create a folder in src name like app and in this folder create your store store.js
In store.js file import configure store

<!-- store.js -->

import { configureStore } from "@reduxjs/toolkit";

make another folder in src features
in this folder we add features like login feature todo feature etc.

make folder in features for example todo and add file in todo name like todoSlice.js we used slice for naming convetion like to know that you use redux toolkit it not neccessary to add slice file name can be todo.js

<!-- todoSlice.js -->

import { createSlice, nanoid } from "@reduxjs/toolkit";

nanoid method generate unique id's

then declare initial state

const initialState = {
todos: [{id: 1, text: "Hello World"}]
}
