# Skills Hub

A community-curated registry of skills. Each skill is submitted as a JSON file and automatically enriched with owner info, latest commit, and a security scan.

---

## Skill Directory

Each enriched skill lives as its own file in the [`skills/`](skills/) folder.

| Skill | Category | Owner | AgentGuard |
|-------|----------|-------|------------|
| *(No skills yet ··· [submit yours!](CONTRIBUTING.md))* | | | |

---

## How It Works

```
Contributor opens PR
  ······ adds skills/<skillname>-metadata.json
        ··�··· name
        ··�··· github_url
        ··�··· category
        ······ description
             ·�·
GitHub Actions workflow runs automatically
  ··�··· ·�· Checks GitHub URL is accessible
  ··�··· ·�· Fetches owner username, display name, avatar, profile URL
  ··�··· ·�· Fetches latest commit hash
  ··�··· ·�· Calls AgentGuard API ·�� injects security report URL
  ··�··· ·�· Stamps evaluated_at timestamp
  ······ ·�· Writes enriched data back into <skillname>-metadata.json
             ·�·
PR comment shows enrichment preview
             ·�·
Merge ·�� enriched file committed automatically
```

## Submit a Skill

See [CONTRIBUTING.md](CONTRIBUTING.md) ··· it takes about 2 minutes.
