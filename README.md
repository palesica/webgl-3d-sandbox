# Sandbox 3D Experiments 🧪

A collection of my graphics experiments built with `WebGL` and `React`.
The main idea is to recreate core `Three.js` concepts in a custom mini-engine: with its own entities, camera system, materials, renderers, and scene management.

## What This Project Is

- 🎯 A personal sandbox for 2D/3D graphics experiments
- 🧠 Practice building rendering engine architecture from scratch
- 🧩 Learning rendering math and pipeline details through real code
- 🛠 UI and demo scenes built with `React`

## Demo Scenes / Experiments

This project includes several standalone visual demos:

- `snow-2d`
- `snow-3d`
- `bezier-particles`
- `perlin-flow-field`
- `terrain`
- `cube-wave`
- `water-2d`

Routes are defined in `src/common/Routes.tsx`.

## Technical Highlights ⚙️

- **Custom engine layer** in `src/engine`
  - `core`: math, buffers, shader system, utilities
  - `package`: scene, camera, materials, geometries, renderers, events
- **Decorators and metadata** (`reflect-metadata`) for parts of the internal architecture
- **Custom GLSL shaders** (`.vert`, `.frag`, `.glsl`)
- **Modular reusable architecture** (geometry / materials / renderers / scene)
- **CRACO + Babel setup** for an older CRA stack and experimental features

## Quick Start 🚀

> This is a legacy project, so `Node 14` is required for a stable setup.

### 1) Prepare the environment

```bash
nvm use 14
```

If Node 14 is not installed:

```bash
nvm install 14
nvm use 14
```

### 2) Install dependencies

```bash
yarn install
```

### 3) Run in development mode

```bash
yarn start
```

The app will be available at `http://localhost:3000`.

## Useful Commands

- `yarn start` - start the dev server
- `yarn test` - run tests in watch mode
- `yarn build` - create a production build

## Project Structure

- `src/engine` - core and modules of the mini-engine
- `src/components` - demo scenes/experiments
- `src/common` - shared application infrastructure
- `src/layout` - UI layout components

## Why This Exists

This project is about learning by building:
not just using a ready-made 3D framework, but understanding how it works internally and recreating a similar architecture from scratch. 💙
