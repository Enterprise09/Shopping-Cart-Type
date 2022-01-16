# Simple Fake Shopping mall

<div>
    <img src="https://img.shields.io/badge/Node.js-14.15.1-brightgreen?logo=node.js">
    <img src="https://img.shields.io/badge/npm-6.14.8-CB3837?logo=npm">
    <img src="https://img.shields.io/badge/React-17.0.2-61DAFB?logo=react">
    <img src="https://img.shields.io/badge/TS-4.5.4-3178C6?logo=typescript">
    <img src="https://img.shields.io/badge/Lincense-MIT-blue">
</div>

> Getting Started with Create React App<br />
> with `--template typescript`<br />
> study with <a href="https://www.youtube.com/channel/UC8butISFwT-Wl7EV0hUK0BQ">freeCodeCamp.org</a>

## Start project

- Download

  1. .zip file => click `download to .zip` button
  2. Using Git
     ```shell
         git clone https://github.com/Enterprise09/Shopping-Cart-Type.git
         cd [clone directory path]   # move to clone directory
         npm install
         npm start
     ```

## Dependency

- package.json

  ```json
  "dependencies": {
      "@material-ui/core": "^4.12.3",
      "@material-ui/icons": "^4.11.2",
      "@testing-library/jest-dom": "^5.16.1",
      "@testing-library/react": "^12.1.2",
      "@testing-library/user-event": "^13.5.0",
      "@types/jest": "^27.4.0",
      "@types/node": "^16.11.19",
      "@types/react": "^17.0.38",
      "@types/react-dom": "^17.0.11",
      "@types/styled-components": "^5.1.20",
      "react": "^17.0.2",
      "react-dom": "^17.0.2",
      "react-query": "^3.34.8",
      "react-scripts": "5.0.0",
      "styled-components": "^5.3.3",
      "typescript": "^4.5.4",
      "web-vitals": "^2.1.3"
  },
  ```

## Features

- Show shopping items - get fake data from fakestore api

  ```js
  // App.tsx
  const getProducts = async (): Promise<CartItemType[]> => {
    return await (await fetch("https://fakestoreapi.com/products")).json();
  };
  ```

- Add & remove items to shopping cart

- Show shopping cart use by Drawer

    <img src="https://user-images.githubusercontent.com/73864148/149665835-be6deacc-22da-4a5e-b2d5-563c2aeda01f.png" width="500">
