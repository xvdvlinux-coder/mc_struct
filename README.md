# Project Setup & Initialization

Follow these steps to initialize and run the project:

## 1. Install Oriented_Direct via node.js & npm

```
npm install -g @xvdxlinux/oriented-direct
```

## 2. Build Frontend Bundle

Compile the application to generate the `public/` directory:

```bash
ospc build --public
```

## 3. Dynamic `main.block` Link (This will only work on Windows, not supported for Linux)

Run this command to create a live dynamic link from `main.block` to `public/main.block`:

```bash
cmd /c "mklink public\main.block ..\main.block 2>nul || mklink /H public\main.block main.block"
```

## 4. Start the Development Server

Start the development server:

```bash
ospc dev
```

Open your browser at `http://localhost:3000`.

