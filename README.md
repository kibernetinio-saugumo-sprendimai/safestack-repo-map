<p align="center">
  <img src="assets/repository-map.svg" alt="SafeStack public repository architecture map" width="100%">
</p>

<p align="center">
  <a href="REPOSITORY_TREE.md"><img src="https://img.shields.io/badge/tree-22%20public%20repositories-43e6d2?style=for-the-badge&labelColor=07152d" alt="22 public repositories"></a>
  <a href="REPOSITORY_SNAPSHOT.json"><img src="https://img.shields.io/badge/snapshot-2026--09--24-6d5dfc?style=for-the-badge&labelColor=07152d" alt="2026-09-24 snapshot"></a>
  <a href="https://github.com/kibernetinio-saugumo-sprendimai"><img src="https://img.shields.io/badge/org-SafeStack-ffb86b?style=for-the-badge&labelColor=07152d" alt="SafeStack organisation"></a>
</p>

# SafeStack Public Repository Map

An independent visual architecture map of the public repositories across the `kibernetinio-saugumo-sprendimai` GitHub organisation. It organizes all public SafeStack projects into a coherent architectural topology: foundational root anchors at the bottom, user-facing surfaces at the top, and public exposure surfaces along the horizontal axis.

> **Scope Notice:** All private and internal operational repositories are strictly excluded from this map.

---

## How to read the map

- **X axis (Horizontal):** Architectural exposure surface, from foundation core to public edge.
- **Y axis (Vertical):** System layer, from root anchors to user interfaces.
- **Node Colour:** Functional domain (Trust, Runtime, Intelligence, Web, Ecosystem).
- **Grey node:** Archived canonical foundation (`safestack-canon`).

---

## Repository groups

| Group | Role | Public Repositories |
| :--- | :--- | :---: |
| **Trust & registry** | Keys, canons, manifests, checksums, control boundaries | 6 |
| **Runtime & infrastructure** | Autonomous node OS, zero trust policy engine, sentinel, suite | 5 |
| **Intelligence & automation** | Deterministic audit engine, verified OSINT, AI team tooling | 3 |
| **Web & publishing** | Freedom manifesto, portfolio, documentation library, organisation config | 4 |
| **Ecosystem & meta** | Repository map, security partners, media library, soundtrack | 4 |
| **Total Public Ecosystem** | | **22** |

---

## Detailed Tree & Machine-Readable Snapshot

- Complete readable catalogue: [REPOSITORY_TREE.md](REPOSITORY_TREE.md)
- Machine-readable JSON snapshot: [REPOSITORY_SNAPSHOT.json](REPOSITORY_SNAPSHOT.json)

```mermaid
flowchart TD
  ORG["kibernetinio-saugumo-sprendimai"]
  ORG --> TRUST["Trust & Registry (6)"]
  ORG --> RUNTIME["Runtime & Infrastructure (5)"]
  ORG --> INTEL["Intelligence & Automation (3)"]
  ORG --> WEB["Web & Publishing (4)"]
  ORG --> ECO["Ecosystem & Meta (4)"]

  TRUST --> T_CANON["canon · technical-canon"]
  TRUST --> T_KEYS["public-keys · validation-registry"]
  TRUST --> T_VERIF["verification-artifacts · control-architecture"]

  RUNTIME --> R_NODE["node-os (Pi 5 Autonomous Node)"]
  RUNTIME --> R_ZT["Safestack-Zero-Trust · ZT-Platform"]
  RUNTIME --> R_SUITE["Safestack-Sentinel · Safestack-suite"]

  INTEL --> I_AUDIT["safestack-audit_system"]
  INTEL --> I_OSINT["safestack-OSINT · AI-Tyreju-Komanda"]

  WEB --> W_SITES["freedom.manifesto · portfolio"]
  WEB --> W_DOCS["safestack-book · .github"]

  ECO --> E_MAP["safestack-repo-map"]
  ECO --> E_MEDIA["partners · media-library · music"]
```

---

## Snapshot Governance

The snapshot records all public repository names, architectural domains, statuses, and primary languages as verified on **2026-09-24**. It contains no confidential data, customer records, or private keys. The map is refreshed whenever public repositories are created, archived, or restructured.
