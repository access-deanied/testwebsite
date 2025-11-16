---
title: "Portfolio Website Development & Deployment"
date: 2025-02-01
draft: false
description: "Design, development, and continuous deployment of a technical portfolio website using static site generation (Hugo), Git version control, and Cloudflare Pages for global hosting."
tags: ["Hugo", "Git", "GitHub Actions", "Cloudflare", "HTML", "CSS", "Deployment"]
---

**![](/images/hugo.png) ![](/images/git.png) ![](/images/cloudflare.png) ![](/images/squarespace.png)**

# 🌐 Portfolio Website: Architecture and Deployment

## Project Overview

This project showcases the end-to-end process of building and deploying a modern, fast, and secure technical portfolio website. It leverages a robust **Static Site Generator (SSG)** and **Continuous Integration/Continuous Deployment (CI/CD)** practices to maintain an always-available, zero-downtime public presence.

## 🛠️ Key Technical Skills & Software

| Category | Technology | Description |
| :--- | :--- | :--- |
| **Static Site Generator** | **Hugo** | Used to rapidly generate all HTML content from lightweight Markdown files, enabling high performance and minimal server load. |
| **Version Control** | **Git / GitHub** | Managed all code changes, tracked revisions, and utilized a GitHub repository as the source of truth for all content and deployment. |
| **Frontend Languages** | **HTML, CSS, JavaScript** | Responsible for custom theme development, creating semantic structure (HTML), styling layouts (CSS), and implementing interactivity (JavaScript). |
| **Continuous Deployment** | **Cloudflare Pages** | Integrated with GitHub to automatically build and deploy the Hugo site globally every time changes are pushed, ensuring rapid content updates. |
| **Domain Management (Future State)** | **Squarespace Domains** | **Planned:** Future use of Squarespace to register and manage the custom domain. This service simplifies linking the domain to the Cloudflare deployment via DNS records (CNAME/A records). |

---

## Deployment Pipeline (CI/CD)

The deployment pipeline is built for efficiency and reliability:

1.  **Code Commit & Push:** All content and code changes are committed and pushed to the **main branch** of the **GitHub repository**.
2.  **Cloudflare Trigger:** Cloudflare Pages is configured to listen for changes on the GitHub repository.
3.  **Automatic Build:** Upon detection, Cloudflare automatically runs the necessary Hugo commands to compile the Markdown and Go templates into static HTML, CSS, and JS files.
4.  **Global Deployment:** The generated static files are instantly deployed across Cloudflare's **global CDN**, pushing the latest version of the website live with near-zero latency.

## Domain Registration & Setup (Future)

While the site is currently hosted on a default Cloudflare Pages URL (`.pages.dev`), the planned steps for full domain registration involve:

* **Domain Acquisition (Squarespace):** Registering the custom domain name through a registrar like **Squarespace