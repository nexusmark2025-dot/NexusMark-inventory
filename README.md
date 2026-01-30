# Nexus Inventory Pro - Deployment Guide

## Step 1: Firebase Setup (5 minutes)

1. Go to [console.firebase.google.com](https://console.firebase.google.com)
2. Create new project (e.g., "NexusInventory")
3. Enable **Authentication** → Email/Password provider
4. Create **Realtime Database** → Start in test mode
5. Copy your config from Project Settings → Your Apps → Web
6. Replace the placeholder config in `index.html`

## Step 2: Security Rules

In Firebase Database → Rules, paste the content from `security-rules.json`

## Step 3: GitHub Pages Deployment

1. Create new repository on GitHub
2. Upload all 4 files (index.html, manifest.json, service-worker.js, README.md)
3. Settings → Pages → Source: Deploy from branch → Main → Root
4. Wait 2 minutes for URL

## Step 4: Admin Setup

1. Open your deployed URL
2. Click "Admin Access" at bottom
3. Enter PIN: `NEXUS2024` (change this in code for production!)
4. Create your first client account

## Features

- ✅ Multi-tenant architecture (separate data per business)
- ✅ Real-time sync across devices
- ✅ QR code device pairing
- ✅ Offline support
- ✅ Indian Rupee formatting (₹)
- ✅ Excel export
- ✅ Category management
- ✅ Low stock alerts
- ✅ Admin dashboard for client management

## Pricing Ready

Code supports your two plans:
- Plan A: ₹10,000 one-time + ₹50/month
- Plan B: ₹200/month

Track plan type in client metadata.