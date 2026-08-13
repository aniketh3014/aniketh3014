```
 █████╗ ███╗   ██╗██╗██╗  ██╗███████╗████████╗
██╔══██╗████╗  ██║██║██║ ██╔╝██╔════╝╚══██╔══╝
███████║██╔██╗ ██║██║█████╔╝ █████╗     ██║   
██╔══██║██║╚██╗██║██║██╔═██╗ ██╔══╝     ██║   
██║  ██║██║ ╚████║██║██║  ██╗███████╗   ██║   
╚═╝  ╚═╝╚═╝  ╚═══╝╚═╝╚═╝  ╚═╝╚══════╝   ╚═╝   
                                              
 ██████╗ ██╗  ██╗ ██████╗ ███████╗██╗  ██╗
██╔════╝ ██║  ██║██╔═══██╗██╔════╝██║  ██║
██║  ███╗███████║██║   ██║███████╗███████║
██║   ██║██╔══██║██║   ██║╚════██║██╔══██║
╚██████╔╝██║  ██║╚██████╔╝███████║██║  ██║
 ╚═════╝ ╚═╝  ╚═╝ ╚═════╝ ╚══════╝╚═╝  ╚═╝
                                          
```

```console
$ ssh aniket@lily
Last login: today · from everywhere · via Tailscale
```

```
                   -`                      aniket@lily
                  .o+`                     ───────────────────────────────────────────
                 `ooo/                     OS         Arch Linux x86_64  (btw)
                `+oooo:                    Host       lily · hardened self-hosted VPS
               `+oooooo:                   Uptime     4 yrs of shipping backends
               -+oooooo+:                  Shell      zsh + tmux
             `/:-:++oooo+:                 Editor     nvim
            `/++++/+++++++:
           `/++++++++++++++:               Role       Backend Engineer · Go
          `/+++ooooooooooooo/`             Domain     APIs, auth, data pipelines, infra
         ./ooosssso++osssssso+`            Languages  Go · TypeScript · SQL · Bash
        .oossssso-````/ossssss+`           Databases  PostgreSQL · Redis
       -osssssso.      :ssssssso.          Infra      Docker · Nginx · Tailscale · AWS
      :osssssss/        osssso+++.         Learning   Kubernetes · gRPC · AWS SAA-C03
     /ossssssss/        +ssssooo/-         Audio      PipeWire → EasyEffects → USB DAC
   `/ossssso+/:-        -:/+osssso+-
  `+sso+:-`                 `.-/+oso:      Location   West Bengal, IN  (UTC+05:30)
 `++:.                           `-/+/     Contact    ghoshaniket050@gmail.com
 .`                                 `/     Colors     ██ ██ ██ ██ ██ ██ ██ ██
```

<div align="center">

<a href="https://www.linkedin.com/in/aniket-ghosh-8b0b53281/"><img src="https://img.shields.io/badge/linkedin-0891b2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
<a href="https://www.x.com/aniketh3014"><img src="https://img.shields.io/badge/x-1c1917?style=for-the-badge&logo=x&logoColor=white" /></a>
<a href="https://discord.com/users/cypherv1.0"><img src="https://img.shields.io/badge/discord-1c1917?style=for-the-badge&logo=discord&logoColor=white" /></a>
<a href="mailto:ghoshaniket050@gmail.com"><img src="https://img.shields.io/badge/mail-0891b2?style=for-the-badge&logo=maildotru&logoColor=white" /></a>
<img src="https://komarev.com/ghpvc/?username=aniketh3014&style=for-the-badge&color=0891b2&label=VISITORS" />

</div>

---

```console
$ whoami --verbose
```

Backend engineer. I write Go for a living and Go for fun, which my friends tell me is a
personality flaw. Most of my work lives in the unglamorous middle of the stack — the part
that has to still be correct at 3AM when nobody is watching: request lifecycles, auth
flows, schema contracts, and queries that stay in the database instead of dragging half a
table into application memory to count it.

I care about three things, in this order: **correctness**, **observability**, **speed**.
Anything that can't be measured will eventually just be believed.

```console
$ pacman -Qe --explicit
```

```
go            1.24   # first language, still favourite
gin bun       ─      # http + orm, small surface area
postgresql    17     # cte-heavy raw sql, no orm heroics
redis         7      # caches, locks, rate limits
typescript    5      # when the browser insists
nextjs        15     # app router, server actions
docker        27     # everything ships in a box
nginx         1.27   # tls termination, reverse proxy
tailscale     ─      # my entire security model
aws           ─      # studying for SAA-C03
```

<div align="center">
<img src="https://skillicons.dev/icons?i=go,ts,nodejs,nextjs,postgres,redis,docker,nginx,linux,aws,git,neovim&theme=dark" />
</div>

---

```console
$ ls -la ~/interests/
```

```
drwxr-xr-x  api-infrastructure/    openapi, contract testing, schema validation
drwxr-xr-x  auth/                  oauth2 flows, token rotation, revocation
drwxr-xr-x  data/                  postgres internals, query plans, cte pipelines
drwxr-xr-x  self-hosting/          the homelab below, and its many scars
drwxr-xr-x  audio/                 iem tuning, parametric eq, pipewire graphs
-rw-------  .cert_grind            aws saa-c03 · in progress
```

<details>
<summary><code>$ tailscale status --topology</code></summary>

<br/>

```
        laptop ──┐                          ┌── phone
                 │                          │
                 └──────┐          ┌────────┘
                        ▼          ▼
                  ╔═══════════════════════════════════════╗
                  ║  lily · ubuntu vps                    ║
                  ║  ufw + fail2ban + adguard home        ║
                  ╠═══════════════════════════════════════╣
                  ║   nginx ── wildcard tls (dns-01)      ║
                  ║     │                                 ║
                  ║     ├──▶ vaultwarden      secrets     ║
                  ║     ├──▶ paperless-ngx    documents   ║
                  ║     ├──▶ joplin server    notes       ║
                  ║     └──▶ netdata          telemetry   ║
                  ║              │                        ║
                  ║              ▼                        ║
                  ║        postgresql + redis             ║
                  ╚═══════════════════════════════════════╝

  public surface area: 0 ports
  everything terminates inside the mesh. http-01 challenges don't work
  when nothing is reachable from the internet — which is exactly the point.
```

</details>

<details>
<summary><code>$ journalctl -u aniket.service --priority=err</code></summary>

<br/>

```log
ERR  auth: redirect loop, infinite
     diagnosis: setTimeout scheduled a token refresh past the 32-bit signed
     cap. Overflowed, fired immediately, forever. The auth context looked
     fine. The clock was the liar.
     resolution: clamp the delay, chain the timers.

ERR  net: container network unreachable after firewall reload
     diagnosis: two firewalls rewriting the same iptables chains, with a
     wireguard mesh caught in the crossfire.
     resolution: stop fighting the platform. ufw + fail2ban, let docker
     keep its own chains.

WARN diff: phantom changes reported on every run
     diagnosis: non-deterministic placeholder generation upstream of a
     comparison step.
     resolution: seed it. determinism isn't a nice-to-have in a diffing
     system — it IS the system.

INFO service restarted. lessons retained.
```

</details>

---

```console
$ git log --stat --author="Aniket Ghosh"
```

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=aniketh3014&show_icons=true&count_private=true&title_color=0891b2&text_color=c7d5d8&icon_color=0891b2&bg_color=0d1117&hide_border=true&border_radius=8" />
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=aniketh3014&layout=compact&langs_count=8&title_color=0891b2&text_color=c7d5d8&bg_color=0d1117&hide_border=true&border_radius=8" />

<img width="98%" src="https://github-readme-activity-graph.vercel.app/graph?username=aniketh3014&bg_color=0d1117&color=c7d5d8&line=0891b2&point=ffffff&area=true&area_color=0891b2&hide_border=true&radius=8" />

</div>

---

```console
$ cat /etc/motd

  open to backend contract work — go services, api + oauth integrations,
  postgres modelling, and getting things deployed properly.

  reachable at ghoshaniket050@gmail.com

$ exit
Connection to lily closed.
```

<!--
  SETUP NOTES
  1. Repo must be named `aniketh3014` (identical to your username) for this to
     render on your profile page.
  2. The ASCII blocks are inside fenced code blocks so GitHub preserves the exact
     spacing. Do NOT reformat them with prettier — it will destroy the alignment.
     Add a .prettierignore with `README.md` if your editor autoformats on save.
  3. The banner is figlet font `ansi_shadow`; the logo is standard neofetch Arch.
     Regenerate with: pyfiglet -f ansi_shadow "ANIKET"
  4. Third-party image services used: shields.io, skillicons.dev, komarev (visitor
     counter), github-readme-stats, github-readme-activity-graph. If any 404s in
     future, delete that line — none of them are load-bearing.
  5. Code blocks scroll horizontally on mobile. The widest block is 87 columns.
-->
