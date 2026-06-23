# Hi, I'm Dane 👋

Senior **Ruby on Rails** backend engineer based in Taiwan, with 6+ years building and scaling web applications for small-to-mid-sized teams. I focus on **system architecture, database optimization, and high-concurrency design**, and I care about clean, well-tested, observable code.

- 🔭 Deep in Rails 7/8, high-throughput systems, and AI-assisted development workflows
- ⚡ Strong on caching, distributed locking, and API design under load
- 🤖 Daily driver of Claude Code for faster, higher-quality delivery
- 🌏 Open to international remote roles

---

## 🚀 Featured Projects

### [MerchantOS](https://github.com/srichsun/merchant_os) — Multi-tenant E-commerce SaaS (Shopify-style)
Row-level multi-tenancy, pessimistic locking to prevent overselling, an AASM order state machine, Stripe & ECPay webhook signature verification, `pg_search` trigram full-text search, Hotwire frontend, and Sentry + Lograge observability.
🔗 [Live overview](https://srichsun.github.io/merchant_os/)

### [Inference Cache Gateway](https://github.com/srichsun/inference-cache-gateway) — High-Concurrency AI Inference Cache
A caching gateway that absorbs a **1,000:1 supply-demand gap** — serving 1M+ daily requests against an upstream model capped at 1,000 calls/day — without sacrificing data freshness or breaking the upstream contract. A study in high-concurrency architecture and engineering quality.
🔗 [Live overview](https://srichsun.github.io/inference-cache-gateway/)

### [rails-health-audit](https://github.com/srichsun/rails-health-audit) — Severity-Ranked Rails Codebase Audit
A repeatable health audit for legacy Rails codebases. It orchestrates the canonical tools (Brakeman, bundler-audit, RubyCritic, RuboCop, license_finder, …) and adds the judgment layer on top: **ranks findings by business impact**, runs runtime data-correctness checks (`active_record_doctor`, `lol_dba`) that static bundles skip, and turns the raw output into a prioritized action plan. Packaged as a Claude Code skill, with zero footprint on the target project.

---

## ✍️ Writing

I write up engineering practice on [**dev.to/danewu**](https://dev.to/danewu):

- [Diagnosing a slow Rails page, layer by layer](https://dev.to/danewu/diagnosing-a-slow-rails-page-layer-by-layer-3abo) — locating slowness by request layer: N+1 vs. a single slow query, and how dev tooling and a production APM fit together.

---

## 🛠️ Tech Stack

**Backend** · Ruby on Rails 7/8 · RSpec (TDD) · Sidekiq · RESTful API · JWT · Hotwire · Devise · Pundit · ActionCable · acts_as_tenant · AASM

**Data** · PostgreSQL · MySQL · Redis · Memcached · query tuning & index design · N+1 detection (Bullet) · row-level tenancy

**Infra & DevOps** · AWS (EC2, RDS, S3, SES) · Docker · GitHub Actions CI/CD · Capistrano · Puma · Nginx · Brakeman · bundler-audit · strong_migrations

**Architecture** · System design · distributed locks (Redis SETNX) · cache architecture (Russian Doll / fragment) · rate limiting · observability (Sentry) · payment integration (Stripe / ECPay)

---

## 📫 Reach Me

[LinkedIn](https://www.linkedin.com/in/danewuglobal/) · srichsun@gmail.com

<!-- Replace the # links and email above before publishing -->
