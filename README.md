# protocol-wars

**Interactive visualization for "The Guild, the Road, and the Ghost"**
Week 6 — Protocols That Refused to Die, Part 1
Goblin Eaters Cyber Cavern · ubritsa.com

---

## What it does

A seven-step animated visualization of the proprietary protocol ecosystem — from the Age of Abundance through the rise of IP to the holdouts and strays that never fully migrated.

Each node represents a company, department, or installation running a protocol. Nodes are fixed in their sector territory. They appear and disappear in place — growth means new installations coming online, retreat means sites migrating away. IP permeates each sector as the proprietary protocols vacate it, rather than pooling in the center.

---

## The seven steps

| Step | Phase | What it shows |
|------|-------|---------------|
| 1 | The Guilds Emerge | IPX/SPX, DECnet, AppleTalk appear in their home sectors |
| 2 | The Age of Abundance | All three grow — Industrial and Healthcare join |
| 3 | Islands That Cannot Speak | Friction indicators at sector boundaries — the incompatibility problem |
| 4 | The Interpreter Arrives | Multi-protocol routers appear at boundaries |
| 5 | The Common Road | IP begins appearing in every sector alongside the proprietary protocols |
| 6 | Not By Conquest. By Inevitability. | IP fills vacated territory — holdouts dim and retreat to provinces |
| 7 | Holdouts and Strays | IP dominates every sector — isolated dim remnants mark the defensive blind spots |

---

## Sectors

| Sector | Primary protocols shown |
|--------|------------------------|
| Enterprise | IPX/SPX → IP |
| Government & Eng. | DECnet → IP |
| Creative & Academic | AppleTalk → IP |
| Industrial | IPX/SPX holdout (never fully migrates) |
| Home & Small Biz | IP (early adopter) |
| Healthcare & Spec. | AppleTalk (admin) → IP; Clinical devices holdout |

---

## Navigation

- **Next / Back** — step through phases manually
- **Auto Play** — runs through all seven steps at 3.5s intervals, stops at the end

---

## Technical

- Single HTML file, no dependencies beyond Google Fonts
- Canvas-based rendering with per-node opacity animation
- Nodes seeded deterministically — layout is stable across resize
- Fonts: JetBrains Mono, Syne (consistent with GECC toolset)
- Palette: GECC dark theme (`#0b0e14` background)

---

## Deployment

```bash
# Copy to tool repo
cp protocol-wars.html ~/git-projects/protocol-wars/index.html

# Version control
cd ~/git-projects/protocol-wars
git add . && git commit -m "initial release — protocol-wars visualizer"
git push

# Copy to Hugo static
cp index.html ~/ubritsa/static/tools/protocol-wars.html

# Publish
gecc-publish "add protocol-wars tool for Week 6"
```

---

## Related

- Post: "The Guild, the Road, and the Ghost" — Week 6, Protocols That Refused to Die Part 1
- Series: How Protocols Work, and How They Break
- Tool repo: `~/git-projects/protocol-wars/`
- Live: `ubritsa.com/tools/protocol-wars`
