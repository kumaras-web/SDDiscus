AQUARIUM FISH E-COMMERCE DEMO
=============================

Files
-----
- index.html: responsive storefront, cart, checkout, QR payment instructions, admin tools.
- README.txt: this file.

Run
---
1. Extract the ZIP.
2. Open index.html in a current browser (Chrome, Edge, Firefox).
3. Click Admin.
4. Open Store & QR settings, set your store name and optional UPI ID, upload your fixed UPI QR image, and save.
5. In Products, edit sample fish/prices/stock or add your own items.
6. Test checkout. Orders will be marked "Payment Pending Verification".
7. In Admin > Orders, verify a payment only after checking your bank/UPI app.
8. Export orders CSV (opens in Excel) and download a JSON backup regularly.

IMPORTANT LIMITATIONS
---------------------
- This is a front-end prototype. Products, orders, cart, settings and QR image are stored in the browser's localStorage.
- Data stays in that browser profile on that device. It does NOT automatically sync between customers, admin devices, or browsers.
- Clearing browser data, changing devices/profiles, or storage corruption can remove data. Export CSV and JSON backups regularly.
- A customer's browser stores the order only on their own device. The shop owner's browser will NOT receive it. Therefore this is NOT ready for real public sales until a backend/database or hosted order-submission service is added.
- Admin has no login and is not secure. Anyone opening the file can access admin controls. Do not publish as-is with private data.
- The QR code is fixed. The page displays the order subtotal and accepts a UPI reference typed by the customer, but cannot confirm payment automatically. Check your bank/UPI account before changing the order to Payment Verified.
- Delivery/packing charges are not calculated. Confirm them separately before taking payment or add them to the workflow.
- Sample product names, prices, quantities and icons are demo content; replace them before launch.
- Live-fish delivery, species restrictions and animal-welfare/transport rules should be checked for your operating area.

Recommended next step before public launch
------------------------------------------
Add a small server-side API and database so customer orders reach the admin, stock is reserved/updated consistently, admin access is protected, and backups are reliable. This can still use the same HTML/CSS/JavaScript front end.

PHOTO NOTE
----------
The initial product cards reference fish photos from the S.D. Discus Aqua Magicpin photo gallery supplied by the user. They are linked as remote images, not downloaded into this package, because this runtime could not fetch the image files directly. An internet connection is required to display them. Remote links can change or stop working. Before using these third-party photos for a commercial store, obtain permission from the photo/store owner or replace them with your own licensed product photos.

The fish names, prices and stock counts in the demo are placeholders and do not represent verified stock or pricing from S.D. Discus Aqua.
