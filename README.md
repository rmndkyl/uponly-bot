# UpOnly Bot

**Versi:** 1.0.0 · **Harga:** Rp 150.000 (~$9) · **Kontak pembelian:** [@rmndkyl](https://t.me/rmndkyl)

Bot automation untuk UpOnly Testnet (Solana Devnet). Pump Mode volume farming untuk kompetisi $1,000,000 UPR.

## Kebutuhan

| Item | Detail |
|---|---|
| Runtime | Node.js 18+ |
| Wallet | EVM / sesuai chain proyek (kamu sendiri) |
| Proxy | opsional (1 proxy per akun) |
| Captcha | tidak perlu |
| Akses | akun proyek yang kamu kelola sendiri |

## Pembayaran

E-Wallet: DANA / GoPay / ShopeePay · Bank: BCA / Seabank · Crypto: contact for wallet address.
Pembeli menghubungi [@rmndkyl](https://t.me/rmndkyl), kirim bukti transfer, lalu terima license key.

---

🌐 **Website:** https://uponly.space
🔗 **Referral:** Referral wallet `7tJpQhBoHC2eATEyk44n9gGEG4nsBnie1JweDmtJYgXd`

## Fitur

- Menu interaktif (1-8) + `--daily` flag
- Auto faucet claim (10,000 USDC per wallet)
- Auto set referral
- Buy & Lock UPR tokens (on-chain Anchor program)
- Early Unlock tokens (sell back → USDC)
- Farm Volume: Buy+Unlock × N rounds per wallet
- Submit signature ke backend untuk volume tracking
- Anti-detection: random delay, realistic User-Agent
- Error handling: retry, skip wallet on error

## Requirements

- Node.js v18+
- Solana wallet dengan SOL Devnet (untuk gas)
- Private key Solana (base58 format)

## Setup

1. `npm install`
4. Edit `config.json` jika perlu

## Menu

```
1. Claim Faucet (all wallets)     — Claim 10,000 USDC testnet
2. Set Referral (all wallets)     — Set referral address
3. Show User Info & Points        — Cek volume, points, stats
4. Buy UPR Tokens (all wallets)   — Buy & lock UPR
5. Unlock Tokens (all wallets)    — Unlock tokens → USDC back
6. Farm Volume (Buy+Unlock × N)   — N rounds buy+unlock per wallet
7. Run Full Daily                  — Faucet + Referral + Farm Volume
8. Exit
```

## Usage

```bash
# Interactive menu
node index.js

# Daily auto-run (cron)
node index.js --daily
```

## Chain Info

- Chain: Solana Devnet
- Program ID: `7Y5XSaB37BQMyK81F9UgLaVzETywwdKrzg1qygn9e3b3`
- Token: $UPR (UpOnly)
- Faucet: 10,000 USDC testnet per wallet
- Competition ends: 30 June 2026

## Config

Edit `config.json`:

```json
{
    "program_id": "7Y5XSaB37BQMyK81F9UgLaVzETywwdKrzg1qygn9e3b3",
    "rpc_url": "https://api.devnet.solana.com",
    "api_base": "https://dev-api.uponly.space",
    "referral_address": "7tJpQhBoHC2eATEyk44n9gGEG4nsBnie1JweDmtJYgXd",
    "trade_rounds": 50,
    "trade_amount_usdc": 10000,
    "delay_min": 2000,
    "delay_max": 5000
}
```

## API Endpoints

Lihat `docs/endpoints.md` untuk dokumentasi lengkap API.

---

© Layer Airdrop ID (LYID) — Premium Automation Script

## 💰 Harga

| Lisensi | Harga | Fitur |
|---------|-------|-------|
| **Single** | Rp 150.000 / ~$10 | 1 device, lifetime |
| **Bundle (3 bot)** | Rp 150.000 / ~$16 | Pilih 3 bot, hemat 20% |
| **Pro (semua bot)** | Rp 150.000 / ~$70 | Semua bot + update, hemat 30% |

**Cara beli:** Chat [@OG_LYID_bot](https://t.me/OG_LYID_bot) di Telegram → /buy

**Bayar pakai:**
- 🇮🇩 DANA / GoPay / ShopeePay / BCA / Seabank
- 🌐 Crypto (USDT/SOL/ETH)

## 🔧 Troubleshooting

| Masalah | Solusi |
|---------|--------|
| `Cannot find module` | Jalankan `npm install` di folder bot |
| `insufficient balance` | Pastikan wallet punya cukup token untuk gas |
| `429 Too Many Requests` | Tunggu 30-60 detik, bot auto-retry |
| Bot diam/tidak jalan | Cek `config.json` — pastikan API key valid |
| License invalid | Chat [@OG_LYID_bot](https://t.me/OG_LYID_bot) → /verify |

**Butuh bantuan?** Join [Discord](https://discord.gg/ZK2NVkfSNn) atau chat [@layerairdrop](https://t.me/layerairdrop)
