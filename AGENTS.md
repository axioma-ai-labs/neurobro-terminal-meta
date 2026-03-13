# Neurobro Terminal - Meta

## Overview

Public-facing meta resources for the [Neurodex](https://neurodex.ai) platform (Neurobro Terminal). This repository hosts static assets and configuration manifests that are referenced by external services and integrations.

## Repository Structure

```
.
├── assets/                    # Static assets (images, icons)
│   └── unkonwn.png           # Default/placeholder image
├── manifests/
│   └── tonconnect-manifest.json  # TON Connect wallet integration manifest
└── README.md
```

## Contents

### TON Connect Manifest

`manifests/tonconnect-manifest.json` - Configuration for TON blockchain wallet connection integration. Referenced by the Neurobro mobile app for TON wallet pairing.

```json
{
  "url": "https://neurodex.ai",
  "name": "Neurodex",
  "iconUrl": "https://neurodex.ai/icons/logo.svg"
}
```

### Assets

Static assets served publicly. Used as fallback images and branding resources across the platform.

## Development

This is a static resource repository. Changes are deployed by pushing to the main branch. No build step required.

When modifying the TON Connect manifest, ensure the mobile app's TON integration still works correctly.

## Keeping This File in Sync

Update this file when:
- New static assets or manifests are added
- External integration configurations change (TON Connect, etc.)
- New platform integrations require public meta resources
