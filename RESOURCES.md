# Apprenticeship Resource Directory

Every external resource referenced in the curriculum, organized by when you'll need it. Bookmark this file.

---

## Your Lab Environment (macOS)

The curriculum was written assuming Windows/WSL2 — you're on a Mac, so use one of these instead:

| Option | Best for | Setup |
|:---|:---|:---|
| **Multipass VM** (recommended) | All labs, including Day 5 systemd work | `brew install multipass`, then `multipass launch --name trs-lab`, then `multipass shell trs-lab` |
| **Docker container** (already installed) | Quick labs, Days 1–4 | `docker run -it --name trs-lab ubuntu:24.04 bash` — note: **no systemd**, so Day 5 service labs won't work here |
| **AWS EC2 t2.micro/t3.micro** (free tier) | Production-realistic practice, SSH workflow | [EC2 Getting Started](https://aws.amazon.com/ec2/getting-started/) — you have the AWS CLI installed |
| **GitHub Codespaces** | Zero-install fallback | [github.com/codespaces](https://github.com/codespaces) — Ubuntu terminal in the browser |

**Recommendation:** Multipass for daily labs (it's a real Ubuntu VM with systemd, one command to launch), plus one EC2 instance in Week 2+ for realistic SSH/networking practice.

Useful Multipass commands: `multipass list`, `multipass stop trs-lab`, `multipass start trs-lab`, `multipass delete trs-lab && multipass purge` (rebuild a clean lab).

---

## Phase 1: Operations Foundation (Weeks 1–4)

### Linux fundamentals
- [Linux Journey](https://linuxjourney.com/) — guided, beginner-friendly lessons; do "Command Line" and "Text-Fu" tracks during Week 1
- [Explainshell](https://explainshell.com/) — paste any command and it explains every flag; use it whenever a lab command confuses you
- [The Linux Command Line (free book, PDF)](https://linuxcommand.org/tlcl.php) — reference reading, chapters 1–10 map to Week 1
- [man7.org Linux man pages](https://man7.org/linux/man-pages/) — official manual pages online (or just run `man <command>` in your VM)
- [OverTheWire: Bandit](https://overthewire.org/wargames/bandit/) — gamified Linux practice via SSH; excellent evening reinforcement, levels 0–15 align with Week 1

### Hands-on troubleshooting practice (highly recommended)
- [SadServers](https://sadservers.com/) — real broken Linux servers you debug in-browser; this is *exactly* the Technical Resolution Specialist skill, start the "Easy" scenarios in Week 2
- [KillerCoda](https://killercoda.com/) — free interactive Linux scenarios in-browser

### Bash scripting
- [Bash Guide for Beginners (TLDP)](https://tldp.org/LDP/Bash-Beginners-Guide/html/) — the classic guide, for Day 6
- [ShellCheck](https://www.shellcheck.net/) — paste your scripts here before committing; it catches bugs and bad practices (also: `brew install shellcheck`)
- [Bash cheatsheet (devhints)](https://devhints.io/bash) — quick syntax reference

### Incident management
- [Atlassian Incident Management Handbook](https://www.atlassian.com/incident-management) — read "What is incident management?" and "Incident severity levels" in Week 1; the rest in Week 3
- [Google SRE Book — Managing Incidents](https://sre.google/sre-book/managing-incidents/) — free chapter; how the best in the industry run incidents
- [PagerDuty Incident Response Guide](https://response.pagerduty.com/) — free, practical, used by real on-call teams; severity/escalation material feeds Week 3
- [Atlassian: How to write a postmortem](https://www.atlassian.com/incident-management/postmortem) — calibrate your RCA writing against this

### Networking (Week 2)
- [How DNS Works (comic)](https://howdns.works/) — gentle, visual DNS introduction
- [Julia Evans' networking zines & posts](https://jvns.ca/#networking) — the best plain-English networking explanations anywhere
- [MDN: HTTP status codes](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status) — your 4xx/5xx reference for the entire program
- [curl cheatsheet](https://devhints.io/curl) — quick reference for the tool you'll use daily

---

## Track A: Tenura Deployment & Operations (runs all phases)

- [Render docs](https://render.com/docs) — backend deployment, env vars, logs, health checks, rollbacks
- [Vercel docs](https://vercel.com/docs) — frontend deployment, env vars, instant rollback to previous deployments
- [MongoDB Atlas docs](https://www.mongodb.com/docs/atlas/) — database hosting, network access rules, connection troubleshooting
- [UptimeRobot](https://uptimerobot.com/) — free uptime monitoring for the deployed health endpoint (Phase 2+)
- [12-Factor App: Config](https://12factor.net/config) — the principle behind environment variable management

---

## Phase 2: Application & Database Support (Weeks 5–8)

### Java / Spring Boot support
- [Spring Boot Actuator docs](https://docs.spring.io/spring-boot/reference/actuator/index.html) — health endpoints you'll use to triage apps
- [Spring PetClinic](https://github.com/spring-projects/spring-petclinic) — the real Spring Boot app we'll run, break, and troubleshoot
- [Baeldung: Spring Boot logging](https://www.baeldung.com/spring-boot-logging) — how app logs are configured, so you know where to look

### REST API troubleshooting
- [Postman (download)](https://www.postman.com/downloads/) — API client for reproducing failures
- [httpbin.org](https://httpbin.org/) — test API that echoes requests and can return any status code on demand (`/status/503`) — perfect for simulating failures
- [Reqres](https://reqres.in/) — mock user API for practice calls

### Databases
- [PostgreSQL official Docker image](https://hub.docker.com/_/postgres) — you already have Docker; this is your Week 7 database
- [PostgreSQL Tutorial](https://www.postgresqltutorial.com/) — syntax and admin reference
- [Use The Index, Luke!](https://use-the-index-luke.com/) — the definitive free guide to why queries are slow
- [pgexercises.com](https://pgexercises.com/) — interactive SQL practice in-browser

### Git & CI/CD
- [Oh Shit, Git!?!](https://ohshitgit.com/) — recovering from git mistakes, plain English
- [GitHub Actions quickstart](https://docs.github.com/en/actions/quickstart) — CI/CD basics for Week 8

---

## Phase 3: Enterprise Simulation & Interview Readiness (Weeks 9–12)

### Monitoring & alerting
- [Prometheus: Getting Started](https://prometheus.io/docs/prometheus/latest/getting_started/) — metrics collection for the dashboard project
- [Grafana: Getting Started](https://grafana.com/docs/grafana/latest/getting-started/getting-started/) — dashboard visualization
- [Node Exporter guide](https://prometheus.io/docs/guides/node-exporter/) — system metrics (CPU/memory/disk), the heart of Project 2

### Ticketing & ITSM concepts
- [Jira free tier](https://www.atlassian.com/software/jira/free) — create a real board for your incident simulator workflow
- [ITIL incident vs. problem management (Atlassian)](https://www.atlassian.com/itsm/incident-management/incident-vs-problem-management) — the vocabulary enterprise interviews expect

### Interview prep
- [Glassdoor — Kyndryl interview questions](https://www.glassdoor.com/Interview/Kyndryl-Interview-Questions-E5482086.htm) — real questions from your target company
- [STAR method guide (Indeed)](https://www.indeed.com/career-advice/interviewing/how-to-use-the-star-interview-response-technique) — structure for behavioral answers

---

## How resources fit the daily workflow

1. **Labs are self-contained.** Every daily lesson I give you includes the full commands, files, and scenarios — you never need an external site to *complete* a lab.
2. **Resources are for depth and reinforcement.** Use them when a concept doesn't click (Explainshell, Linux Journey), for evening practice (Bandit, SadServers), or as references while writing artifacts (MDN status codes, Atlassian postmortem guide).
3. **When stuck, ask me first.** Tell me "I'm stuck on X" in a session — debugging your confusion is part of the training, and I can see your actual files and environment.
