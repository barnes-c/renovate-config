# renovate-config

Shared [Renovate](https://docs.renovatebot.com/) preset for my repositories.

```json
{
    "$schema": "https://docs.renovatebot.com/renovate-schema.json",
    "extends": ["github>barnes-c/renovate-config"]
}
```

A consuming repo's own `packageRules` are applied after the preset's, so they override it (e.g. a shorter `minimumReleaseAge` for patches).
