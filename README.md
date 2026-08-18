# Jamidaar Mobile App

Jamidaar is a React Native / Expo mobile application for verified land discovery, land-related services, due diligence, reports, requests, and user account management.

This repository is intended to be easy for the whole Jamidaar development team to clone, run, test, and extend.

## Current app features

- Swipeable onboarding
- Create Profile / prototype OTP flow
- Home dashboard
- Property marketplace and filters
- Property detail pages
- Wishlist
- Land verification services
- Court Case Search request flow
- Request cart and GST calculation
- Profile editing
- Notifications
- Order history
- Local prototype persistence using AsyncStorage
- Expo/EAS Android build configuration

## Quick start

```bash
git clone https://github.com/vsDlion/Jamidaar.git
cd Jamidaar
npm install
npx expo install --fix
npx expo-doctor
npx expo start --clear
```

Then press `a` for Android, or scan the Expo QR code with a compatible Expo client/development build.

On Windows, use `REPAIR_AND_START.bat` once the project files are present.

## Prototype login

The current frontend prototype does not call a production OTP provider yet.

1. Enter a legal name.
2. Enter a mobile number.
3. Tap **Verify Mobile**.
4. Demo OTP `123456` is filled automatically.
5. Accept the Terms checkbox.
6. Tap **Create Profile**.

## Project structure

```text
Jamidaar/
├── App.js
├── assets/
├── src/
│   ├── components/
│   ├── screens/
│   ├── data.js
│   └── theme.js
├── docs/
├── app.json
├── eas.json
├── package.json
├── CONTRIBUTING.md
└── .env.example
```

## Useful commands

```bash
npm install
npx expo install --fix
npx expo-doctor
npx expo start --clear
npm run android
npm run web
npm run build:apk
```

## Android APK

```bash
npx eas-cli@latest login
npx eas-cli@latest build -p android --profile preview
```

## Backend integrations still required

The current repository is primarily the mobile frontend. Production integrations still need to be connected for OTP/authentication, user accounts, property data, land/revenue records, court search, AI Land Reports, blockchain status, uploads, maps, payments, order history, and report downloads.

See `docs/BACKEND_INTEGRATION.md`.

## Team development

Recommended workflow:

```bash
git checkout main
git pull
git checkout -b feature/my-feature
# work + test
git add .
git commit -m "Add my feature"
git push -u origin feature/my-feature
```

Then open a Pull Request into `main`.

Read `CONTRIBUTING.md`, `docs/SETUP.md`, and `docs/TEAM_WORKFLOW.md` before making larger changes.

## Security

This repository is public. Never commit `.env`, private API credentials, Razorpay secrets, OTP credentials, service-account files, keystores, private keys, Aadhaar credentials, database credentials, or customer data.

`EXPO_PUBLIC_*` values are visible to the client and must contain only publishable configuration.

## Technology

- React Native
- Expo SDK 57
- React 19
- AsyncStorage
- Expo Vector Icons
- EAS Build

## Brand

**Jamidaar** — institutional deep green with premium land and heritage styling.
