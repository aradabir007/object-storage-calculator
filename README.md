# Object Storage Pricing Calculator

A simple, fast, and comprehensive calculator to compare object storage pricing across 21+ cloud providers. Built as a single HTML file with no backend required.

![Object Storage Calculator](https://img.shields.io/badge/Providers-21+-blue) ![License](https://img.shields.io/badge/License-MIT-green) ![Built with AI](https://img.shields.io/badge/Built%20with-AI-purple)

> 🤖 **Built entirely by AI** — This project was created using AI. The only human contribution was providing and verifying the pricing data for each provider.

## Features

- **21+ Cloud Providers** - Compare pricing from major providers including AWS S3, Cloudflare R2, Backblaze B2, and more
- **Real-time Calculation** - Instant price updates as you type
- **Smart Pricing Logic** - Handles tiered pricing, minimum charges, free tiers, and traffic allowances
- **Currency Conversion** - Automatic EUR to USD conversion with live exchange rates
- **Dark Mode** - Easy on the eyes with automatic system preference detection
- **Mobile Friendly** - Responsive design that works on all devices
- **Quick Presets** - One-click presets for common usage scenarios
- **Sort by Cost** - Easily find the cheapest option for your needs
- **No Dependencies** - Single HTML file, works offline after initial load

## Providers Included

| Provider             | Currency | Free Traffic | Notes             |
| -------------------- | -------- | ------------ | ----------------- |
| AWS S3               | $        | ❌           | Tiered pricing    |
| Azure Blob Storage   | $        | ❌           |                   |
| Backblaze B2         | $        | 3x stored    |                   |
| Bunny Storage        | $        | ❌           | Tiered traffic    |
| Cloudflare R2        | $        | ✅ Unlimited |                   |
| Contabo              | €        | ✅ Unlimited |                   |
| DigitalOcean Spaces  | $        | 1TB included | Min $5/mo         |
| Exoscale             | €        | ❌           | Tiered storage    |
| Google Cloud Storage | $        | ❌           |                   |
| Hetzner              | €        | 1TB included | Min €4.99/mo      |
| IDrive e2            | $        | ✅ Unlimited |                   |
| IONOS                | $        | 2TB free     | Tiered traffic    |
| Linode               | $        | 1TB included | Min $5/mo         |
| OVH                  | €        | ❌           |                   |
| Railway              | $        | ✅ Unlimited |                   |
| Scaleway             | €        | ❌           | 75GB free storage |
| Storadera            | €        | Up to stored | Fair usage policy |
| Storj                | $        | ❌           |                   |
| Tigris               | $        | ✅ Unlimited | 5GB free storage  |
| Vultr                | $        | 1TB free     |                   |
| Wasabi               | $        | Up to stored | 90-day retention  |

## Usage

### Online

Simply open `index.html` in your browser or host it on any static file server.

### Quick Presets

- **Hobby** - 50GB storage / 100GB traffic
- **Small** - 100GB storage / 500GB traffic
- **Startup** - 500GB storage / 1TB traffic
- **Medium** - 1TB storage / 2TB traffic
- **Business** - 5TB storage / 10TB traffic
- **Large** - 10TB storage / 20TB traffic
- **Enterprise** - 50TB storage / 100TB traffic

## Technical Details

- **Frontend**: Vue.js 3 (CDN)
- **Styling**: Tailwind CSS (CDN)
- **Exchange Rate API**: [fawazahmed0/currency-api](https://github.com/fawazahmed0/currency-api)
- **No Backend Required**: Everything runs client-side

## Important Notes

- All prices are calculated based on the provider's billing model (per GB or per TB)
- Providers with per TB pricing round up storage and traffic to the nearest TB
- Some providers include free traffic allowances based on storage or fixed amounts
- Uses EU location (mostly Germany) for all providers
- 1TB = 1024GB
- Exchange rates are fetched dynamically but may fluctuate
- **Always confirm pricing with providers** as prices may vary by region

## Contributing

Found incorrect pricing or want to add a provider? Contributions are welcome!

1. Fork the repository
2. Update the `providers` array in `index.html`
3. Submit a pull request with source links for the pricing

## License

MIT License - feel free to use, modify, and distribute.

## Changelog

### 2025-12-28

- Added Railway with free egress/ingress
- Added Exoscale with tiered storage pricing
- Added Storadera with fair usage traffic policy
- Major UI overhaul with mobile-friendly card layout
- Added quick preset buttons for common usage scenarios
- Improved dark mode with better color scheme
- Added collapsible notes and changelog sections
- Added custom +/- buttons for inputs
- Added favicon

---

**Disclaimer**: This calculator is for estimation purposes only. Prices were manually verified but may change. Always check the official pricing pages before making decisions.
