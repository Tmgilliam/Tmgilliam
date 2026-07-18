# Profile bio, socials, and pins — UI / auth steps

Automated bio update requires the GitHub CLI `user` scope:

```powershell
gh auth refresh -h github.com -s user
gh api user -X PATCH `
  -f bio='Enterprise AI & Cloud Architect | ERP transformation, governed agents | Azure AZ-305 | Founder @Brilliant-Brainstorm-Intelligence-LLC' `
  -f blog='https://bbiedge.com' `
  -f location='California' `
  -f company='Brilliant Brainstorm Intelligence, LLC'
```

Or set the same fields in GitHub Settings → Public profile.

## Social accounts

Keep LinkedIn. Website field = `https://bbiedge.com` (up to four social links supported). Prefer “California” over a precise city unless needed.

## Pins (UI only — no API)

https://github.com/Tmgilliam → Customize your pins

**Replace current pins** (`erp-ai-delay-risk`, `aws-sagemaker-mlops`) with:

1. `tmgilliam.github.io`
2. `bbi-ai-readiness-diagnostic-kit`
3. Optional: one audited cloud/infra repo
4. Hold `erp-ai-delay-risk` until public-proof audit passes

Org pins: https://github.com/Brilliant-Brainstorm-Intelligence-LLC → pin the diagnostic kit only for now.
