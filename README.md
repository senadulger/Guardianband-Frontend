# GuardianBand — HarmonyOS Frontend

![GuardianBand app screens](docs/images/guardianband.png)

Mobile application frontend developed during my Huawei internship using ArkTS and ArkUI.

This was a team project; my contribution was frontend development. The backend is separate and is not included in this repository.

## Features

- Login, registration, and role selection
- User profiles and medical information
- Patient and caregiver screens
- Medication and prescription screens
- QR-based linking and emergency access flows
- SOS screens with location integration
- API integration and session management

## Run locally

1. Open the project in DevEco Studio.
2. Install the configured HarmonyOS SDK `6.1.1(24)` and sync OHPM dependencies.
3. Configure your own device signing in DevEco Studio.
4. Run a compatible backend and configure its address in `entry/src/main/ets/services/ApiConfig.ets`.
5. Select a compatible device or emulator and run the `entry` module.

The default API address is `http://10.0.2.2:3000`. For a physical device, set your backend computer's reachable LAN address. Staging and production `.example` URLs are placeholders. Backend-dependent features require the separate backend service.

## Source structure

- `AppScope/`: application metadata and assets
- `entry/src/main/ets/pages/`: screens
- `entry/src/main/ets/components/`: shared UI components
- `entry/src/main/ets/services/`: API, repositories, sessions, and QR logic
- `entry/src/main/ets/utils/`: utilities
- `entry/src/main/resources/`: images, strings, and page configuration
- `BACKEND_REQUESTS.md`: backend integration notes

## Status

Internship frontend portfolio project. The build has not been verified during repository preparation. This is not an official Huawei product or a production medical service.
