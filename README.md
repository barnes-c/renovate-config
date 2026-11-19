# renovate-config

Shared [Renovate](https://docs.renovatebot.com/) preset for my repositories.

```json
{
    "$schema": "https://docs.renovatebot.com/renovate-schema.json",
    "extends": ["github>barnes-c/renovate-config"]
}
```

Go modules also extend `github>barnes-c/renovate-config:go` (`go.json`).

A consuming repo's own `packageRules` are applied after the preset's, so they override it (e.g. a longer `minimumReleaseAge` for a risky package).
