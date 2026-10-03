# Drape

**Offline billing, inventory and customer management for apparel showrooms.**

Drape brings the sales counter, size-and-colour stock, customer history and supplier accounts into a Windows desktop application. Business data is stored locally in SQLite.

## Technology
React · TypeScript · Electron · Node.js · SQLite · Vite

## Implemented workflows
- Billing, held bills, returns and exchanges, store credit and configurable GST calculations.
- Size-and-colour inventory, stock receipts, barcode tags and supplier ledgers.
- Customer profiles, loyalty rewards, requested-item tracking and alterations.
- Thermal and full-page printing, PDF bills and CSV reports.
- Owner/cashier permissions, backup and restore, and offline licence activation.

## Architecture
React screens call a restricted Electron IPC interface. Node.js application logic handles SQLite persistence, transactions, printing and backups. A shared tax module is used across billing and reporting.

## Engineering work
The local project includes automated tests for tax calculations, backend workflows, permissions, exchanges, rewards and the WhatsApp integration using a mock API.

## Project status
A Windows distribution package exists locally. WhatsApp Cloud API support has not been validated against Meta's live service. Installation on additional computers and real printer testing remain part of release validation.

## About this repository
This is a public project showcase. Application source, licence-signing material and business data are not distributed here. It does not contain a downloadable app or an App Store / Google Play release.
