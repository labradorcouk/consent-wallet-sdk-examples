# Perse Consent Wallet Integration Examples

This repository provides minimal code examples showing how to integrate the Perse Consent Wallet with third‑party applications.

- Developer Guide: https://opendata.energy/dev-guide

## Examples

- Web: `web-integration.html` — minimal browser example

## Web integration

Use `web-integration.html` as the reference. It demonstrates how to:
- Load the Consent SDK from the CDN (`https://opendata.energy/consent-sdk.min.js`).
- Obtain an access token via the OAuth client credentials flow.
- Initialize the SDK and request consent using customer email and meter details.

Quick start:
1. Open `web-integration.html` and replace `<YOUR_CLIENT_ID>` and `<YOUR_CLIENT_SECRET>` with your credentials.
2. Serve the file locally (e.g., using a simple static server) and open it in a browser.
3. Enter an email, meter number, and fuel type, then click “Request Consent”.

Security note: Do not expose client secrets in frontend code in production. Fetch tokens on your backend and pass short‑lived tokens to the browser.
