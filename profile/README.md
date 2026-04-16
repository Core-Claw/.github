<p align="center">
    <a href="https://coreclaw.com" target="_blank">
        <img src="./images/banner.svg" alt="CoreClaw — Web Scraping Platform & Ready-Made Data Workers" width="800">
    </a>
</p>

<p align="center">
    <strong>Build, deploy, and monetize web data Workers — or use 100+ ready-made ones instantly.</strong>
</p>

<p align="center">
    <a href="https://coreclaw.com">
        <img src="https://img.shields.io/badge/coreclaw.com-Visit-0A0A0A?style=flat-square&logo=googlechrome&logoColor=white" alt="Website">
    </a>
    <a href="https://docs.coreclaw.com">
        <img src="https://img.shields.io/badge/Docs-Read-4A90D9?style=flat-square&logo=readthedocs&logoColor=white" alt="Docs">
    </a>
    <a href="https://coreclaw.com/store">
        <img src="https://img.shields.io/badge/Worker_Store-Browse-FF6B35?style=flat-square&logo=shopify&logoColor=white" alt="Store">
    </a>
    <a href="mailto:support@coreclaw.com">
        <img src="https://img.shields.io/badge/Email-Contact-D14836?style=flat-square&logo=gmail&logoColor=white" alt="Email">
    </a>
</p>

---

## What is CoreClaw?

CoreClaw is a full-stack **web data extraction platform** that combines a managed cloud runtime with a marketplace of ready-made data Workers. Whether you're a non-technical user who needs data now, or a developer building the next scraper — CoreClaw has you covered.

- **For users**: Pick a Worker, enter a URL, get structured data in minutes. No code, no infrastructure, pay per success.
- **For developers**: Build Workers in Python, Node.js, or Go. Deploy on managed infrastructure with scheduling, logs, webhooks, and auto-scaling. Publish to the Store and earn revenue.

## Why CoreClaw?

| | CoreClaw | Traditional Scraping |
|---|---|---|
| **Setup** | Zero-config cloud workspace | Self-hosted proxies, browsers, schedulers |
| **Pricing** | Pay per successful result | Pay for infrastructure regardless of results |
| **No-code** | 100+ ready-made Workers | Build everything from scratch |
| **Scale** | Built-in auto-scaling | Manual capacity planning |
| **Monetization** | Publish & sell your Workers | No distribution channel |

## Quick Start

### Use a Worker (No Code)

1. Browse the [Worker Store](https://coreclaw.com/store)
2. Pick a Worker (Google Maps, TikTok, Instagram, LinkedIn, YouTube…)
3. Enter your target URL or keyword
4. Get structured data — export as CSV, JSON, or via API

### Build a Worker (Code)

Create a Worker in your preferred language and deploy it to CoreClaw:

**Python**
```python
from coreclaw import Worker

@worker.run
async def main(context):
    data = await context.request("https://example.com")
    await context.push_data({"title": data.css("h1::text").get()})
```

**Node.js**
```javascript
import { Worker } from '@coreclaw/worker';

export default async function run(context) {
    const data = await context.request('https://example.com');
    await context.pushData({ title: data.css('h1::text').get() });
}
```

**Go**
```go
func Run(ctx *coreclaw.Context) error {
    data, _ := ctx.Request("https://example.com")
    ctx.PushData(map[string]string{"title": data.Css("h1").Text()})
    return nil
}
```

👉 [Read the full Developer Docs](https://docs.coreclaw.com)

## Open Source Repositories

| Repo | Description |
|---|---|
| [PythonScirptDemo](https://github.com/Core-Claw/PythonScirptDemo) | Python Worker template — build and deploy Python scrapers on CoreClaw |
| [NodeScirptDemo](https://github.com/Core-Claw/NodeScirptDemo) | Node.js Worker template — build and deploy JS scrapers on CoreClaw |
| [GoScirptDemo](https://github.com/Core-Claw/GoScirptDemo) | Go Worker template — build and deploy Go scrapers on CoreClaw |
| [scraper-webui-docs](https://github.com/Core-Claw/scraper-webui-docs) | Official documentation portal (Starlight/Astro) |
| [cafe-scraper-skill](https://github.com/Core-Claw/cafe-scraper-skill) | Scraper skill definitions and configurations |

## Data Solutions by Industry

- **B2B Leads** — Extract company & contact data from Google Maps, LinkedIn, Apollo
- **Price Tracking** — Monitor competitor pricing on Amazon, eBay, Walmart, AliExpress
- **Influencer Discovery** — Find creators on TikTok, Instagram, YouTube with engagement metrics
- **Market Monitoring** — Track reviews, ratings, and trends across platforms
- **Custom Solutions** — Enterprise-grade data pipelines with 99.9% SLA

## Links

- 🌐 [Website](https://coreclaw.com)
- 📚 [Documentation](https://docs.coreclaw.com)
- 🛒 [Worker Store](https://coreclaw.com/store)
- 💰 [Pricing](https://coreclaw.com/pricing)
- 📧 [Contact / Enterprise](mailto:support@coreclaw.com)

---

<p align="center">
    <sub>Built with ❤️ by the CoreClaw team · <a href="https://coreclaw.com">coreclaw.com</a></sub>
</p>