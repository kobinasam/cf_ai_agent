# 🚀 Nexus AI — Full Stack Cloudflare Agent

A **serverless, full-stack AI application** running entirely on **Cloudflare’s edge network**.  
This project combines a **React frontend**, a **Worker backend**, **Durable Objects** for persistent memory, and **Llama 3.3** for intelligence — all deployed as a single unit.

---

## 🏗 Architecture

This project uses the **Worker + Assets + Durable Objects** pattern (Full-Stack):

- **Frontend:** React + Vite + Tailwind CSS (Glassmorphism UI)  
- **Backend:** Cloudflare Worker acts as both the API Gateway and Static Asset Server  
- **Intelligence:** Workers AI running `@cf/meta/llama-3.3-70b-instruct-fp8-fast`  
- **Memory:** Cloudflare Durable Objects (SQLite backend) store chat history per session  
- **Deployment:** Single command deploy via `wrangler`

---

## 🚀 Prerequisites

- **Node.js** (v18 or later)  
- **Cloudflare Account**  
- **Wrangler CLI:**  
  ```bash
  npm install -g wrangler
