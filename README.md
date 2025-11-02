
# 🚀 Vite + Yarn + TailwindCSS (Modern Setup Guide)

A clean, working setup for Vite + Yarn + TailwindCSS, tested and simplified.
Forget the usual install headaches — this method just works.



## Create the Vite Project

Install my-project with yarn


```bash
  yarn create vite
```
### When prompted with “Install and run dependencies?”, select No. This creates the project structure without installing dependencies yet.


```bash
  cd [project_name]
```

Example  

```bash
  cd myapp
```

Install Dependencies

```bash
  yarn
```

Add TailwindCSS and Vite Plugin
```bash
  yarn add tailwindcss @tailwindcss/vite
```

### Configure -- vite.config.js --

Open the file and add this at the top:

```bash
  import tailwindcss from '@tailwindcss/vite'
```
AND 
```bash
  plugins: [
  react(),
  tailwindcss(),
]
```
Final Version:

```bash
import { defineConfig } from 'vite'
import react from '@vitejs/plugin-react'
import tailwindcss from '@tailwindcss/vite'

export default defineConfig({
  plugins: [
    react(),
    tailwindcss(),
  ],
})
```

--------
### Edit app.css

Add the following line:
```bash
@import "tailwindcss";
```

----
### Run the project on terminal used at first

```bash
yarn vite
```
