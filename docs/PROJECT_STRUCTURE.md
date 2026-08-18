# Project Structure

```text
Jamidaar/
├── App.js                    # App state and lightweight navigation
├── app.json                  # Expo app configuration
├── package.json              # Dependencies and scripts
├── eas.json                  # EAS build profiles
├── assets/                   # Jamidaar logo and property/onboarding imagery
├── src/
│   ├── components/
│   │   ├── BottomNav.js      # Bottom navigation
│   │   └── UI.js             # Shared buttons, fields, cards, headers
│   ├── screens/              # App screens
│   ├── data.js               # Prototype property/service/notification data
│   └── theme.js              # Brand colors and shared styling values
└── docs/                     # Team documentation
```

## Current architecture

The current build is a functional frontend prototype. Navigation/state is intentionally simple so the team can iterate quickly. AsyncStorage is used for local prototype persistence.

Recommended production evolution:

1. Add `src/api/` for a dedicated API client.
2. Move authentication into an auth context/store.
3. Replace demo data with backend responses.
4. Introduce React Navigation when route complexity grows.
5. Add typed data models and automated tests.
