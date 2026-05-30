# Bonusaki — front-end demo

A static, UI-only demo of **Bonusaki**, a scratch-and-win loyalty engine for
cafes: scan a QR on your cup → play a scratch-and-win → the prize lands in your
wallet → staff redeem it at the counter.

**▶ Live demo:** https://ioannisbekas.github.io/bonusaki-demo/

This repo is just the clickable demo (`index.html`, mock data, no backend). The
real application — Postgres row-level security, the atomic every-scan-wins prize
engine, async wallet-pass creation, single-use HMAC redemption, and Stripe
billing, all test-covered — lives in a separate private repo.

The demo shows three surfaces:

- **Customer** — the branded scan landing, email capture, and the real
  scratch-card interaction.
- **Merchant** — dashboard with scan/redemption stats, prize distribution, and a
  prize-tier editor with the live "weights must total 100%" meter.
- **Cashier** — the redemption screen (valid / already-used / tampered outcomes).
