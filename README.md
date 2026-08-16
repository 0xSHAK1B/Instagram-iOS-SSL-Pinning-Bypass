<div align="center">

# 🔓 Instagram iOS SSL Pinning Bypass

**Intercept, capture & analyze Instagram HTTPS traffic on iPhone & iPad — 2026 working build**

[![Download IPA](https://img.shields.io/badge/⬇_Download_IPA_(v442.0.0)-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](../../releases/latest) &nbsp; [![Telegram](https://img.shields.io/badge/Telegram-26A5E4?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/MUH4MM4DSH4KIB)

![iOS](https://img.shields.io/badge/iOS_14.0+-000000?style=flat-square&logo=apple&logoColor=white)
![ARM64](https://img.shields.io/badge/arm64-blue?style=flat-square)
![Version](https://img.shields.io/badge/Instagram-v442.0.0.22.64-E4405F?style=flat-square&logo=instagram&logoColor=white)

<img width="590" height="1280" alt="Instagram iOS SSL Pinning Bypass PoC – Traffic Captured" src="https://github.com/user-attachments/assets/46e71e11-e609-45e9-a559-a1cce80af639" />

*Live capture — Instagram iOS `i.instagram.com` traffic intercepted in cleartext, v442.0.0.22.64.*

</div>

> **Bypass SSL/TLS certificate pinning** in Instagram for iOS and pipe the full HTTPS stream — login, API, and Direct flows — into **Burp Suite · mitmproxy · Reqable · Proxypin.** Tap a section below to expand.

---

<details open>
<summary><b>📦 Supported version</b></summary>

<br>

| App | Bundle ID | Version | Arch | Status |
|-----|-----------|:-------:|:----:|:------:|
| Instagram for iOS | `com.burbn.instagram` | **442.0.0.22.64** | `arm64` | ✅ [**Download**](../../releases/latest) |

The patched IPA lives in the [**Releases**](../../releases/latest) section. Need the newest build or another version? [Message me on Telegram](https://t.me/MUH4MM4DSH4KIB).

</details>

<details>
<summary><b>🎯 What you can capture</b></summary>

<br>

- **Login & authentication** — `i.instagram.com/api/v1/accounts/login/`, 2FA, session tokens
- **REST & GraphQL API** — feed, explore, reels, stories, and profile endpoints
- **Direct (DMs)** — realtime/MQTT channels and thread endpoints
- **Media & CDN** — image/video delivery and the upload pipeline
- **Search & discovery** — search queries, hashtag and location lookups
- **Analytics & telemetry** — device telemetry and A/B assignments

</details>

<details>
<summary><b>⚙️ Requirements</b></summary>

<br>

**iOS device — iOS 14.0+.** Install with one of:

- **TrollStore** — permanent, no re-sign, no expiration (iOS 14.0 – 16.6.1 / 17.0). Recommended where supported.
- **KravaSign** or a **paid Apple Developer certificate** — for newer iOS (17.1+, 18, 26); stable, longer-lived signing.
- **Sideloadly / AltStore** — works, but a free Apple ID signature expires after 7 days and must be re-signed.

**Proxy tool** — [Burp Suite](https://portswigger.net/burp) · [mitmproxy](https://mitmproxy.org/) · [Reqable](https://reqable.com) · [Proxypin](https://proxypin.com)

</details>

<details>
<summary><b>🚀 How to bypass — step by step</b></summary>

<br>

1. Download the patched IPA from [**Releases**](../../releases/latest).
2. Install it (TrollStore, or sign with Sideloadly/AltStore and trust the profile under **Settings → General → VPN & Device Management**). Uninstall the official Instagram app first — signatures conflict.
3. Export your proxy's CA certificate, then **install and fully trust** it: open the `.crt`/`.pem` → **Settings → General → VPN & Device Management → Install Profile**, then **Settings → General → About → Certificate Trust Settings → enable full trust**.
4. Set the Wi-Fi proxy: **Settings → Wi-Fi → (network) → Configure Proxy → Manual**.
5. Launch Instagram — decrypted HTTPS streams into your proxy in real time.

> Both the CA install **and** full-trust toggle are required; skip either and decryption fails silently.

</details>

<details>
<summary><b>💼 Need a custom bypass?</b></summary>

<br>

Custom SSL pinning bypass · automated patching scripts · full reverse-engineering projects — for any iOS or Android app. [**Message me on Telegram →**](https://t.me/MUH4MM4DSH4KIB)

</details>

<details>
<summary><b>⚠️ Disclaimer</b></summary>

<br>

For **educational and security-research purposes only**. Not affiliated with, endorsed by, or connected to Meta, Instagram, or their subsidiaries. All trademarks belong to their respective owners. You are responsible for complying with your local laws and the app's Terms of Service, and should only analyze traffic on accounts and devices you own or are authorized to test. Provided "as is", without warranty of any kind.

</details>

<details>
<summary><b>🔗 Related projects</b></summary>

<br>

| App | Platform | Repository |
|-----|----------|------------|
| Instagram | Android | [Instagram SSL Pinning Bypass](https://github.com/0xSHAK1B/Instagram-SSL-Pinning-Bypass) |
| Threads | iOS | [Threads iOS SSL Pinning Bypass](https://github.com/0xSHAK1B/Threads-iOS-SSL-Pinning-Bypass) |
| Facebook | iOS | [Facebook iOS SSL Pinning Bypass](https://github.com/0xSHAK1B/Facebook-iOS-SSL-Pinning-Bypass) |
| Edits | iOS | [Edits iOS SSL Pinning Bypass](https://github.com/0xSHAK1B/Edits-iOS-SSL-Pinning-Bypass) |
| Instants | iOS | [Instants iOS SSL Pinning Bypass](https://github.com/0xSHAK1B/Instants-iOS-SSL-Pinning-Bypass) |
| TikTok | iOS | [TikTok iOS SSL Pinning Bypass](https://github.com/0xSHAK1B/TikTok-iOS-SSL-Pinning-Bypass) |

</details>

---

<div align="center">

### 💖 Support This Project

Please **⭐ star the repo** — it helps others find it and keeps the builds coming.

| Currency | Address |
|:---------|:--------|
| **BTC** | `131NaAJooX2XYq5QUFmKsTuLQXcGNayYPJ` |
| **ETH** | `0xea9a566a5123c3a1b8d60f8bdd845835716668f0` |
| **USDT (TRC-20)** | `THssAZhUQEEsw15211rAaRLGRjSWXMX4PW` |

[![Telegram](https://img.shields.io/badge/@MUH4MM4DSH4KIB-26A5E4?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/MUH4MM4DSH4KIB)

</div>
