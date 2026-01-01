# Yapidrom Organization Settings

Bu repo, yapidrom organizasyonundaki tüm repo'lar için merkezi yapılandırmaları içerir.

## Workflows

### PR Source Branch Check

`.github/workflows/pr-source-check.yml`

Tüm repo'larda PR açıldığında kaynak branch kontrolü yapar:

| Hedef | İzin Verilen Kaynaklar |
|-------|------------------------|
| `master` / `main` | `dev`, `hotfix/*` |
| `dev` | `feature/*`, `bugfix/*`, `refactor/*`, `chore/*`, `test/*` |

Bu workflow, organization ruleset tarafından zorunlu tutulur.

## Ruleset

Organization seviyesinde `protected-branches` ruleset'i aktiftir.

**Koşullar:**
- `branch-protection` custom property = `true`
- Branch: `master`, `main`, `dev`

**Kurallar:**
- PR zorunlu
- 1 approval gerekli
- Code owner review zorunlu
- Status check zorunlu
- Delete ve force push engelli

## Daha Fazla Bilgi

Detaylı dokümantasyon için: [BRANCH-PROTECTION.md](https://github.com/yapidrom/test-repo/blob/master/BRANCH-PROTECTION.md)
