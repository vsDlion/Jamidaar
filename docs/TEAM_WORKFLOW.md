# Team Workflow

## Recommended branches

- `main` — stable shared branch
- `feature/...` — new features
- `fix/...` — bug fixes
- `ui/...` — visual/UX changes

## Daily flow

```bash
git checkout main
git pull
git checkout -b feature/my-change
```

Work and test, then:

```bash
git add .
git commit -m "Add <feature>"
git push -u origin feature/my-change
```

Open a Pull Request into `main`.

## Avoid direct main edits

Once multiple people are contributing, use Pull Requests instead of everyone pushing directly to `main`. This reduces accidental overwrites and gives the team a review point.

## Useful commit examples

- `Fix onboarding swipe behavior`
- `Add property detail API integration`
- `Improve mobile OTP validation`
- `Connect wishlist to backend`
- `Update Jamidaar service cards`

Use GitHub Issues or Projects to assign work by screen or feature and keep one person responsible for merging into `main` until maintainership is formalized.
