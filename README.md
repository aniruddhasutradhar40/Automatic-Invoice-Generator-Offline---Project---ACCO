# Rudrix Invoice Generator

A free, offline, single-file invoice generator that runs entirely in your browser — no backend, no sign-up, no internet required after loading. Built for freelancers and small businesses in the USA, UAE, Bangladesh, and India (with a custom option for any other country).

Just open the HTML file and start creating professional invoices.

---

## Features

- **Multi-country presets** — Switch between US, UAE, Bangladesh, India, or Custom, and the currency, tax label (Sales Tax / VAT / GST), default tax rate, and Tax ID label auto-fill.
- **Auto-calculation** — Subtotal, discount, tax, and grand total update live as you type.
- **Amount in words** — Automatically converts the total into words, using the correct numbering system (International for US/UAE, Indian Lakh/Crore system for India/Bangladesh).
- **Logo upload** — Add your company logo directly from your device (stored locally, nothing uploaded anywhere).
- **Line items** — Add/remove unlimited invoice line items with description, quantity, and unit price.
- **Save and history** — Save invoices locally (via `localStorage`) and reload any past invoice from the "My invoices" panel.
- **Export / Import backup** — Export all saved invoices as a JSON file, and import them back anytime (useful for backups or moving to a new device).
- **Print / Download as PDF** — One click to print or save the invoice as a clean, print-optimized PDF (A4 layout).
- **Responsive design** — Works smoothly on desktop, tablet, and mobile.
- **Offline and private** — No server, no tracking, no data ever leaves your browser.

---

## Supported Countries

| Country | Currency | Tax Type | Default Rate | Tax ID Label |
|---|---|---|---|---|
| United States | USD ($) | Sales Tax | 0% | EIN |
| UAE | AED | VAT | 5% | TRN |
| Bangladesh | BDT (৳) | VAT | 15% | BIN |
| India | INR (₹) | GST | 18% | GSTIN |
| Other | Custom | Custom | Custom | Custom |

---

## Getting Started

No installation, no dependencies, no build steps.

1. Download the `Automatic_Invoice_Generator_Offline.html` file from this repository.
2. Open it in any modern web browser (Chrome, Firefox, Edge, Safari).
3. Fill in your company details, customer info, and line items.
4. Click Save to store the invoice locally, or Print / Download PDF to export it.

That's it — the whole app is a single `.html` file.

### Optional: Run via a local server

You can also serve it locally if you prefer:

```bash
# Python 3
python -m http.server 8000

# then open http://localhost:8000 in your browser
```

---

## Tech Stack

- **HTML5** — structure
- **CSS3** — styling, responsive layout, print media queries
- **Vanilla JavaScript** — all logic (no frameworks, no libraries)
- **Browser localStorage** — for saving invoice history offline

No build tools, no npm packages, no external dependencies.

---

## Project Structure

```
.
└── Automatic_Invoice_Generator_Offline.html   # The entire app (HTML + CSS + JS)
```

---

## How Data is Stored

All invoice data is stored locally in your browser using `localStorage` under the key `invoiceGeneratorInvoices_v1`. Nothing is sent to any server. Use the Export JSON button regularly to back up your data, especially before clearing browser storage or switching devices.

---

## Contributing

Contributions, issues, and feature requests are welcome.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## License

This project is open source and available under the [MIT License](LICENSE).

---

## Support

If this project helped you, consider giving it a star on GitHub.
