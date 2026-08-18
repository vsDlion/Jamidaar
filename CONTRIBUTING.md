# Contributing to Jamidaar

## Team workflow

1. Pull the latest `main` branch before starting work.
2. Create a branch for each change:
   - `feature/<short-name>` for features
   - `fix/<short-name>` for bug fixes
   - `ui/<short-name>` for design work
3. Keep commits focused and descriptive.
4. Test the app before pushing.
5. Open a pull request into `main` and describe what changed.
6. Do not commit credentials, `.env` files, API secrets, keystores, or production customer data.

## Common commands

```bash
npm install
npx expo install --fix
npx expo-doctor
npx expo start --clear
```

## Before a pull request

- Confirm the app starts without a red screen.
- Test the screen or flow you changed.
- Check that navigation and scrolling still work.
- Run `npx expo-doctor`.
- Make sure no secrets are present in the diff.

## Code areas

- Shared UI: `src/components/`
- Screens: `src/screens/`
- App data/demo data: `src/data.js`
- Theme/colors: `src/theme.js`
- Main app/navigation state: `App.js`
