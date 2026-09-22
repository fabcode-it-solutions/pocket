# Pocket App — Save & Read Articles Offline

A cross-platform **"read it later"** mobile app (iOS, Android & Web) built with React Native and Expo. Users can save articles from around the web, organize them with tags and favorites, and read them later — even without an internet connection.

This project was built as a production-quality showcase of a modern, offline-first React Native application: clean architecture, a reusable design system, robust state management, and full offline data sync.

---

## Key Features

- **Save Articles for Later** — add any article by URL and read it in a distraction-free, formatted in-app reader
- **Offline-First** — articles, tags, and favorites are stored locally with [WatermelonDB](https://watermelondb.dev/) and remain fully accessible without an internet connection
- **Search & Filter** — instantly search saved articles and filter by tags, favorites, or read status
- **Tagging & Organization** — categorize articles with custom tags for quick retrieval
- **Favorites** — bookmark important articles for one-tap access
- **Authentication** — secure sign-in/sign-up flow with persisted sessions
- **Light & Dark Mode** — full theming support that adapts to system appearance
- **Responsive UI** — a custom, reusable component and theming library shared across every screen

---

## Tech Stack

| Layer | Technology |
|---|---|
| Framework | [Expo](https://expo.dev) (React Native) + [Expo Router](https://docs.expo.dev/router/introduction/) (file-based navigation) |
| Language | TypeScript |
| State Management | Redux Toolkit + RTK Query (data fetching, caching, token refresh) |
| Offline Storage | WatermelonDB (local database with reactive sync) |
| Persistence | Redux Persist + AsyncStorage |
| UI System | Custom theme engine + reusable component library (buttons, cards, inputs, tags, etc.) |
| Forms | React Hook Form |
| Testing | Jest + jest-expo |
| Build & Deploy | EAS Build / EAS Submit |

---

## App Structure

```
app/            Screens & navigation (Expo Router)
├── (auth)/     Sign in / sign up flow
├── (tabs)/     Main tab navigation (home, search, etc.)
├── article/    Article detail views
└── reader/     In-app article reader

components/     Reusable UI & core themed components
redux/          Store, slices, and RTK Query API services
database/       WatermelonDB models, schema & sync logic
theme/          Design tokens, theme provider & hooks
provider/       App-level context providers
screens/        Screen-level feature components
utils/          Shared helper functions
```

---

## Getting Started (for developers)

1. **Install dependencies**
   ```bash
   yarn install
   ```

2. **Run the app**
   ```bash
   npx expo start
   ```

   From the Expo CLI output you can launch the app in a:
   - [Development build](https://docs.expo.dev/develop/development-builds/introduction/)
   - [Android emulator](https://docs.expo.dev/workflow/android-studio-emulator/)
   - [iOS simulator](https://docs.expo.dev/workflow/ios-simulator/)
   - [Expo Go](https://expo.dev/go) sandbox

3. **Run tests**
   ```bash
   yarn test
   ```

---

## About This Project

This repository demonstrates end-to-end mobile app development capability, including:

- Designing and building a scalable, themeable UI component library from scratch
- Implementing offline-first data architecture with local persistence and sync
- Structuring a production-grade Redux + RTK Query data layer
- Delivering a polished, native-feeling experience across iOS, Android, and Web from a single codebase

---

## Let's Work Together

Interested in a similar mobile or cross-platform app for your business? Feel free to reach out — I'd be glad to discuss your project and how this same approach can be applied to it.
