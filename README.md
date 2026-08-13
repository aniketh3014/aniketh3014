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
               `+oooooo:                   Shell      zsh + tmux        Editor  nvim
               -+oooooo+:                  Uptime     3 yrs of shipping backends
             `/:-:++oooo+:
            `/++++/+++++++:                Role       Backend Engineer · Go
           `/++++++++++++++:               Focus      distributed systems · cloud infra
          `/+++ooooooooooooo/`             Runtime    goroutines · channels · contexts
         ./ooosssso++osssssso+`            Languages  Go · TypeScript · SQL · Bash
        .oossssso-````/ossssss+`           Data       PostgreSQL · Redis
       -osssssso.      :ssssssso.          Infra      Docker · Kubernetes · Nginx · AWS
      :osssssss/        osssso+++.         Network    Tailscale · gRPC · TCP transports
     /ossssssss/        +ssssooo/-         Learning   K8s operators · gRPC · AWS SAA-C03
   `/ossssso+/:-        -:/+osssso+-       Audio      PipeWire → EasyEffects → USB DAC
  `+sso+:-`                 `.-/+oso:
 `++:.                           `-/+/     Location   West Bengal, IN  (UTC+05:30)
 .`                                 `/     Status     focusing · open to opportunities
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

Backend engineer. I build distributed systems in Go — the kind where the interesting
problems are coordination, failure, and throughput rather than screens. Peer-to-peer file
storage with content-addressable replication, custom TCP transports with their own
handshake and framing, services that run identically under Compose, Swarm and Kubernetes.

Most of my work lives in the unglamorous middle of the stack — the part that still has to
be correct at 3AM when nobody is watching. Goroutine lifecycles that don't leak, contexts
that actually cancel, caches that fail open, and queries that stay in the database instead
of dragging half a table into application memory to count it.

I care about three things, in this order: **correctness**, **observability**, **speed**.
Anything that can't be measured will eventually just be believed.

```console
$ pacman -Qe --explicit
```

```
go            1.24   # first language, still favourite
                     # goroutines, channels, sync, pprof
grpc          ─      # protobuf contracts over http/2
postgresql    17     # cte-heavy raw sql, explain analyze, no orm heroics
redis         7      # caches, distributed locks, rate limits, pub/sub
docker        27     # everything ships in a box
kubernetes    1.32   # deployments, services, the yaml tax
nginx         1.27   # tls termination, reverse proxy, load balancing
linux         ─      # arch on the desktop, ubuntu on the metal
tailscale     ─      # wireguard mesh — my entire security model
aws           ─      # ec2, s3, vpc, iam · studying for SAA-C03
typescript    5      # when the browser insists
```

<div align="center">
<img src="https://skillicons.dev/icons?i=go,grpc,postgres,redis,docker,kubernetes,nginx,linux,aws,ts,nodejs,neovim&theme=dark" />
</div>

---

```console
$ ls -la ~/interests/
```

```
drwxr-xr-x  distributed-systems/   p2p topologies, replication, consistency, gossip
drwxr-xr-x  go-performance/        pprof, escape analysis, allocation budgets
drwxr-xr-x  concurrency/           worker pools, backpressure, graceful shutdown
drwxr-xr-x  orchestration/         k8s, swarm, and what actually differs in practice
drwxr-xr-x  caching/               redis patterns, invalidation, distributed locks
drwxr-xr-x  observability/         metrics that matter, logs that don't lie
drwxr-xr-x  self-hosting/          the topology below, and its many scars
drwxr-xr-x  audio/                 iem tuning, parametric eq, pipewire graphs
-rw-------  .cert_grind            aws solutions architect associate · in progress
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
ERR  net: container network unreachable after firewall reload
     diagnosis: two firewalls rewriting the same iptables chains, with a
     wireguard mesh caught in the crossfire. each layer was individually
     correct and collectively fatal.
     resolution: stop fighting the platform. ufw + fail2ban, let docker
     own its chains, drop the container onto host networking.

ERR  db: p99 latency climbing under load, cpu idle
     diagnosis: aggregation happening in application memory. thousands of
     rows crossing the wire so the process could count them.
     resolution: push the work down. cte pipeline, one round trip, the
     planner does what it was built to do.

ERR  auth: redirect loop, infinite
     diagnosis: a refresh timer scheduled past the 32-bit signed cap.
     overflowed, fired immediately, forever. the code looked fine.
     the clock was the liar.
     resolution: clamp the delay, chain the timers.

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

<!--
  SETUP NOTES
  1. Repo must be named `aniketh3014` (identical to your username) for this to
     render on your profile page.
  2. The ASCII blocks are inside fenced code blocks so GitHub preserves exact
     spacing. Do NOT let prettier reformat this file — it will destroy the
     neofetch alignment. Add `README.md` to .prettierignore if you autoformat.
  3. Banner font is figlet `ansi_shadow`; logo is the standard neofetch Arch art.
     Regenerate with: pyfiglet -f ansi_shadow "ANIKET"
  4. Third-party services: shields.io, skillicons.dev, komarev, github-readme-stats,
     github-readme-activity-graph. None are load-bearing — delete on failure.
  5. Widest code block is 87 columns; blocks scroll horizontally on mobile.
-->
