# 🚀 mPanel Web Application Deployment Guide

[![mPanel Documentation](https://img.shields.io/badge/mPanel-Hosting%20Guide-blue.svg?style=flat-square)](https://github.com/sweetyagarwal3113-hub/deployment_guide)
[![Node Version](https://img.shields.io/badge/Node.js-v20.20.2%2B-green.svg?style=flat-square)](https://nodejs.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](LICENSE)

A comprehensive, step-by-step guide for deploying a full-stack web application (**Next.js / Node.js Backend** & **Static Frontend**) on the **mPanel** hosting control panel architecture.

---

## 📋 Quick Specs & Configuration Summary

| Setting Parameter | Required Configuration / Value |
| :--- | :--- |
| **Application Mode** | `Automatic (Production)` |
| **Node Version** | `20.20.2` *(or latest recommended LTS)* |
| **Startup Command** | `npm start` |
| **Working Directory** | `backend` |
| **Proxy Enabled** | **`ON`** *(Ensure the Blue Toggle switch is active)* |
| **Path** | `/` *(Leave default / blank)* |
| **Port** | `3000` |

---

## 🛠️ Step-by-Step Deployment Walkthrough

### Step 1: Website Setup & Domain Addition
1. Log into your **mPanel** control panel dashboard.
2. Navigate to the **My Website** section.
3. Click **Add Website** and input your target domain name (e.g., `example.com` or `subdomain.example.com`).
4. > 💡 **Tip:** Ensure your domain's DNS `A-Record` points to your mPanel server IP before proceeding.

---

### Step 2: Node.js Application Configuration
Configure your Node.js runtime settings in the mPanel dashboard with the parameters shown below:

```text
Application Mode  : Automatic
Node Version      : 20.20.2
Startup Command   : npm start
Working Directory : backend
Proxy Enabled     : ON (Blue Toggle)
Path              : /
Port              : 3000
```

---

### Step 3: Frontend Deployment (`public_html`)
1. In your local frontend project directory, run:
   ```bash
   npm run build
   ```
2. Compress (zip) the **contents inside the `dist/` directory** (do **not** zip the `dist` folder itself).
3. Upload and extract the zip file directly inside `public_html/`.

```text
📂 public_html/ Directory Structure
├── 📄 index.html        (Main compiled HTML entrypoint)
├── 📁 assets/            (Compiled CSS, JS, fonts & images)
└── 📄 ...               (Other compiled static files)
```

> ⚠️ **Important Zipping Rule:** Select the contents *inside* `dist/` before zipping so `index.html` resides directly at the root of `public_html/`.

---

### Step 4: Backend Deployment (`backend/` directory)
1. Create a directory named `backend` in your root host folder (**outside** `public_html`).
2. Build your local backend project:
   ```bash
   npm run build
   ```
3. Upload the compiled build files, node modules, server entry point, and environment files to `backend/`.

```text
📁 backend/ Directory Structure
├── 📁 node_modules/     (REQUIRED: production dependencies for npm start)
├── 📁 .next/            (REQUIRED: compiled Next.js build output)
├── 📄 server.js         (REQUIRED: main server entrypoint)
├── 📄 package.json      (REQUIRED: manifest with "npm start" script)
├── 📄 .env              (REQUIRED: environment configuration variables)
└── ❌ src/              (NOT NEEDED: source code is compiled inside .next/)
```

> 💡 **`node_modules/` vs `src/` Rule:**
> - **Include `node_modules/`:** **YES.** Needed so Node.js can run dependencies on application startup.
> - **Exclude `src/`:** **NO.** Do not upload `src/`. All TypeScript/React code is compiled into `.next/`. Skipping `src/` saves bandwidth and protects your source code.

> ⚠️ **Important Environment & Zip Note:** mPanel does **not** feature a separate Environment Variables UI section in the control panel. You **must upload your `.env` file directly inside the `backend/` folder**. Ensure hidden folders/files such as `.next/` and `.env` are explicitly included in your zip file before uploading.

---

### Step 5: Server Restart & Verification
1. Navigate back to the **Node.js** tab in mPanel.
2. Click **Restart Server** to apply all configuration changes and spawn your Node.js app instance.
3. Visit your website URL in the browser to verify full functionality.

---

## 🌐 How to Run & Preview the Guide Locally

You can preview the interactive `index.html` deployment guide locally using any of the following commands:

### Option 1: Direct Browser Launch (Quickest)

* **Windows (PowerShell):**
  ```powershell
  Start-Process "index.html"
  ```
* **macOS:**
  ```bash
  open index.html
  ```
* **Linux:**
  ```bash
  xdg-open index.html
  ```

---

### Option 2: Run Local Web Server

* **Using Node.js (`http-server`):**
  ```bash
  npx -y http-server -p 8080
  ```
  *Then open: [http://localhost:8080](http://localhost:8080)*

* **Using Python:**
  ```bash
  python -m http.server 8080
  ```
  *Then open: [http://localhost:8080](http://localhost:8080)*

* **Using PowerShell (No external dependencies):**
  ```powershell
  powershell -ExecutionPolicy Bypass -File tcp_server.ps1
  ```
  *Then open: [http://localhost:8080](http://localhost:8080)*

---

## 📄 License
This deployment guide is released under the [MIT License](LICENSE).
