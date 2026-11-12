RSC-HUB V1 — PROTOTYPE / DEMO

1. Unzip all files and upload the folder contents to a HTTPS static web host (GitHub Pages, Netlify, etc.).
2. Open index.html via the hosted HTTPS URL. First login creates an Admin username/password (min 8 chars).
3. Admin can create Product, Development, Planning, QA, Customer and Admin users.
4. Product, Development, Planning have basic local CRUD and CSV export.
5. QA module is adapted from RSC-QA TEAM V4. Import Excel/CSV, upload multiple photos, generate report preview and quick links. The Excel .xlsx reader loads from a CDN and needs Internet; CSV works without it.
6. Customer role opens only QA portal, searches published reports by PO and uses quick links.
7. Install from browser when PWA installation becomes available.

IMPORTANT LIMITATIONS:
- DEMO ONLY. Password hashes, roles and records live in browser storage. No secure server authentication, shared database, customer isolation, or real multi-device sync.
- QA and HUB data are not synchronized; each is stored separately in browser storage. Admin users created in HUB are bridged into the embedded QA UI for demo sessions only.
- Photo uploads are limited by browser storage quota.
- Export HUB JSON and QA JSON backups separately.
- For production: backend auth + row-level permissions + database + object storage + migrations + audit logs are required.
