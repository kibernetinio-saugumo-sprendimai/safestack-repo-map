<p align="center">
  <img src="assets/repository-map.svg" alt="SafeStack public repository architecture map" width="100%">
</p>

<p align="center">
  <a href="REPOSITORY_TREE.md"><img src="https://img.shields.io/badge/tree-20%20public%20repositories-43e6d2?style=for-the-badge&labelColor=07152d" alt="20 public repositories"></a>
  <a href="REPOSITORY_SNAPSHOT.json"><img src="https://img.shields.io/badge/snapshot-2026--11--06-6d5dfc?style=for-the-badge&labelColor=07152d" alt="2026-11-06 snapshot"></a>
  <a href="SHA256SUMS"><img src="https://img.shields.io/badge/integrity-SHA--256%20%2B%20Ed25519-9be15d?style=for-the-badge&labelColor=07152d" alt="Owner-signed SHA-256"></a>
  <a href="https://github.com/kibernetinio-saugumo-sprendimai"><img src="https://img.shields.io/badge/org-SafeStack-ffb86b?style=for-the-badge&labelColor=07152d" alt="SafeStack organisation"></a>
</p>

# SafeStack Public Repository Map

An independent visual architecture map of the public repositories across the [`kibernetinio-saugumo-sprendimai`](https://github.com/kibernetinio-saugumo-sprendimai) GitHub organisation. It organizes all public SafeStack projects into a coherent architectural topology: foundational root anchors at the bottom, user-facing surfaces at the top, and public exposure surfaces along the horizontal axis.

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
| **Trust & registry** | Keys, canons, owner-signed manifests, checksums, control boundaries | 6 |
| **Runtime & infrastructure** | Zero-trust policy engine, platform orchestration, sentinel, runtime suite | 4 |
| **Intelligence & automation** | Deterministic security audit framework and verified OSINT | 2 |
| **Web & publishing** | Freedom manifesto, technical library, OHS/DSS standard, organisation config | 4 |
| **Ecosystem & meta** | Repository map, security partners, media library, soundtrack | 4 |
| **Total Public Ecosystem** | | **20** |

---

## Detailed Tree & Machine-Readable Snapshot

- Complete readable catalogue: [REPOSITORY_TREE.md](REPOSITORY_TREE.md)
- Machine-readable JSON snapshot: [REPOSITORY_SNAPSHOT.json](REPOSITORY_SNAPSHOT.json)
- Repository SHA-256 manifest & owner signature: [SHA256SUMS](SHA256SUMS) · [SHA256SUMS.sig](SHA256SUMS.sig)

```mermaid
flowchart TD
  ORG["kibernetinio-saugumo-sprendimai (20 Public)"]
  ORG --> TRUST["Trust & Registry (6)"]
  ORG --> RUNTIME["Runtime & Infrastructure (4)"]
  ORG --> INTEL["Intelligence & Automation (2)"]
  ORG --> WEB["Web & Publishing (4)"]
  ORG --> ECO["Ecosystem & Meta (4)"]

  TRUST --> T_CANON["safestack-canon · safestack-technical-canon"]
  TRUST --> T_KEYS["safestack-project-public-keys · safestack-validation-registry"]
  TRUST --> T_VERIF["Verification-artifacts · safestack-control-architecture"]

  RUNTIME --> R_ZT["Safestack-Zero-Trust · SafeStack-Zero-Trust-Platform"]
  RUNTIME --> R_SUITE["Safestack-Sentinel · Safestack-suite"]

  INTEL --> I_AUDIT["safestack-audit_system"]
  INTEL --> I_OSINT["safestack-OSINT"]

  WEB --> W_SITES["freedom.manifesto.github.io · safestack-book"]
  WEB --> W_DOCS["safestack-darbu-sauga · .github"]

  ECO --> E_MAP["safestack-repo-map · safestack-partners"]
  ECO --> E_MEDIA["safestack-media-library · safestack-music"]
```

---

## Snapshot Governance & Cryptographic Verification

The snapshot records all **20** public repository names, architectural domains, statuses, and primary languages as verified on **2026-11-06**. It contains no confidential data, customer records, private repository references, or private keys. The map is refreshed whenever public repositories are created, archived, or change visibility.

`SHA256SUMS` is cryptographically signed (`SHA256SUMS.sig`) by the SafeStack Organization Owner (`safestack-owner`, OpenSSH Ed25519 key `SHA256:jpM7K4+8hyAJo9qg4ISDbljuENZzx2UqMHu73+S9q48`, published in [`Verification-artifacts/keys/allowed_signers`](https://github.com/kibernetinio-saugumo-sprendimai/Verification-artifacts/blob/main/keys/allowed_signers)):

```bash
shasum -a 256 -c SHA256SUMS

ssh-keygen -Y verify -f ../Verification-artifacts/keys/allowed_signers \
  -I safestack-owner -n file -s SHA256SUMS.sig < SHA256SUMS
```
