# Hi, I'm Dane 👋

Senior **Ruby on Rails** backend engineer based in Taiwan, with 6+ years building and scaling web applications for small-to-mid-sized teams. I focus on **system architecture, database optimization, and high-concurrency design**, and I care about clean, well-tested, observable code.

- 🔭 Deep in Rails 7/8, high-throughput systems, and AI-assisted development workflows
- ⚡ Strong on caching, distributed locking, and API design under load
- ✍️ Writing a deep-dive series on Rails performance — *Lessons from Production*
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

**Rails Performance: Lessons from Production** — a deep-dive series that diagnoses real performance incidents one layer at a time (SQL → caching → background work → infrastructure), all on a single running example.

📍 Read it on [**dev.to/danewu**](https://dev.to/danewu) and [**Medium**](https://medium.com/@danewu_).

**Start here**
- [Diagnosing a slow Rails page, layer by layer](https://dev.to/danewu/diagnosing-a-slow-rails-page-layer-by-layer-3abo) — locating slowness by request layer: N+1 vs. a single slow query, and how dev tooling and a production APM fit together.

**Database layer**
- [From 8s to 1s: Truly Understanding Rails N+1 by Opening Up ActiveRecord](https://dev.to/danewu/from-8s-to-1s-truly-understanding-rails-n1-by-opening-up-activerecord-1oj) — a four-layer mental model of ActiveRecord (Ruby → SQL → DB → memory) that explains N+1, broken preloads, and row explosion.
- [A 1000x Speedup From One Index — and Why It Sometimes Does Nothing](https://dev.to/danewu/a-1000x-speedup-from-one-index-and-why-it-sometimes-does-nothing-6if) — how indexes actually work (B-tree, leftmost prefix) and the real reasons one you added still won't kick in.
- [You Wanted a Number, but Loaded 500,000 Rows Into Memory](https://dev.to/danewu/you-wanted-a-number-but-loaded-500000-rows-into-memory-5087) — count vs size, exists? vs present?, SQL aggregation, and find_each: let the database do the work.

**Caching**
- [The Fastest Query Is the One You Never Run: The Four Layers of Rails Caching](https://dev.to/danewu/the-fastest-query-is-the-one-you-never-run-the-four-layers-of-rails-caching-fif) — compute, invalidate, render, transfer — and the one idea that ties them together.
- [We Added a Cache; Three Days Later It Took the Database Down at Peak](https://dev.to/danewu/we-added-a-cache-three-days-later-it-took-the-database-down-at-peak-p46) — four production caching traps: stampede, treating cache as source of truth, unbounded keys, and caching failures.

**Background work & the application layer**
- [One Notification Email Made Our Checkout API 3 Seconds Slower](https://dev.to/danewu/one-notification-email-made-our-checkout-api-3-seconds-slower-34oj) — moving slow work to background jobs: idempotency, passing ids vs. objects (GlobalID), queue priorities, retries.
- [Your SQL Is Fast but the API Is Slow: It's the Ruby Layer](https://dev.to/danewu/your-sql-is-fast-but-the-api-is-slow-its-the-ruby-layer-2fno) — serialization, object allocation / GC pressure, and the memoization gotchas.

**Infrastructure**
- [The Code Is Fine, but Requests Queue Until They Time Out: Puma, Pools, CDN](https://dev.to/danewu/the-code-is-fine-but-requests-queue-until-they-time-out-puma-pools-cdn-15lj) — Puma workers × threads, aligning the connection pool, the GVL and IO, and offloading static assets to a CDN.


## 🛠️ Tech Stack

**Backend** · Ruby on Rails 7/8 · RSpec (TDD) · Sidekiq · RESTful API · JWT · Hotwire · Devise · Pundit · ActionCable · acts_as_tenant · AASM

**Data** · PostgreSQL · MySQL · Redis · Memcached · query tuning & index design · N+1 detection (Bullet) · row-level tenancy

**Infra & DevOps** · AWS (EC2, RDS, S3, SES) · Docker · GitHub Actions CI/CD · Capistrano · Puma · Nginx · Brakeman · bundler-audit · strong_migrations

**Architecture** · System design · distributed locks (Redis SETNX) · cache architecture (Russian Doll / fragment) · rate limiting · observability (Sentry) · payment integration (Stripe / ECPay)

---

## 📫 Reach Me

[LinkedIn](https://www.linkedin.com/in/danewuglobal/) · srichsun@gmail.com
