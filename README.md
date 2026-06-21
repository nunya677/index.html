# Secure Remote Access Architecture — Independent Lab

An interactive, self-paced lab for interns covering bastion hosts, jump servers, VPN design, and the redundancy-vs-security tradeoff.

## What's in here

This repo hosts a single self-contained HTML page (`index.html`) — an interactive mini-course that walks through:

- **Part 0** — Standing up a 4-zone Docker network (attacker, bastion/DMZ, jump server, app server)
- **Part 1** — Hardening a bastion host from scratch (key-only auth, no root login, fail2ban)
- **Part 2** — Simulating a brute-force attack, before and after hardening
- **Part 3** — Pivoting through a jump server with SSH ProxyJump
- **Part 4** — Reading and analyzing real auth logs
- **Part 5** — Adding a redundant bastion behind a load balancer, then testing failover
- **Part 6** — Cleanup and submission

Each part includes copyable terminal commands, a checkpoint to confirm before moving on, and progress tracking (saved locally in the browser). At the end, interns can submit their write-up directly via a pre-filled email.

## Live site

Deployed on Render as a static site: **https://internlab-s05z.onrender.com**

## Prerequisites for interns

- Docker and Docker Compose installed locally
- A terminal (macOS/Linux, or WSL2/Git Bash on Windows)
- ~2.5–3.5 hours

No cloud account or production system is touched — everything runs in local containers.

## Updating this site

1. Edit `index.html` directly on GitHub (or upload a replacement) and commit to `main`.
2. Render auto-redeploys within a minute or two of any commit to this branch.
3. Refresh the live URL above to confirm the change.

## Related materials

This lab is the independent/take-home companion to a live facilitator-led session, which also includes a slide deck, a no-terminal paper activity for groups, and a knowledge-check quiz.
