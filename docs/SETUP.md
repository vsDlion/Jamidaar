# Jamidaar Development Setup

## Requirements

- Git
- Node.js compatible with Expo SDK 57
- npm
- Android Studio + emulator, or a compatible Expo Go/development build on a phone
- Optional: VS Code

## First-time setup

```bash
git clone https://github.com/vsDlion/Jamidaar.git
cd Jamidaar
npm install
npx expo install --fix
npx expo-doctor
npx expo start --clear
```

On Windows, the included `REPAIR_AND_START.bat` can install/align packages and start Expo once the project source is present.

## Prototype login

- Enter a legal name.
- Enter a valid-looking mobile number.
- Tap **Verify Mobile**.
- OTP `123456` is filled automatically.
- Accept Terms & Conditions.
- Tap **Create Profile**.

## Common fixes

### Metro or Expo cache issue

```bash
npx expo start --clear
```

### Dependency mismatch

```bash
npx expo install --fix
npx expo-doctor
```

### Important

Use the local Expo CLI:

```bash
npx expo start
```

Do not rely on the deprecated globally installed `expo-cli` package.
