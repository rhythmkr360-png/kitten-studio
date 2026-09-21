# Kitten Studio privacy policy

Effective date: 2026-07-19  
App package: `com.kitten.studio`

Kitten Studio is designed to run speech generation on the user’s Android device.

## Data collection

Kitten Studio does not create an account and does not include advertising, analytics, crash-reporting, tracking, or cloud speech SDKs. The app developer does not receive scripts, recordings, generated audio, model files, or usage history through the app.

## Data stored on the device

Kitten Studio can store the following in app-private storage:

- downloaded speech-model packages;
- a validated copy of the public model catalog;
- voice-preview MP3 files held in Android's temporary cache for up to six hours;
- scripts currently being edited;
- generated WAV files and their local metadata;
- an optional authorized reference-voice WAV, transcript, display name, and consent timestamp;
- preferences such as appearance and Wi-Fi-only downloading.

Users can remove generated audio, model packages, and the voice reference from Settings. Uninstalling the app removes its app-private data.

## Network use

Kitten Studio checks a public GitHub catalog when the app starts and when the Voices screen is reopened after 15 minutes. This lets newly listed compatible models and corrected preview links appear without an app update.

When the user taps a voice preview, the app downloads that short MP3 from the public Kitten Studio GitHub Release. Android stores it in temporary cache for no more than six hours, subject to a 32 MiB cache limit. Android may clear cached files sooner. The preview isn't added to the user's audio library.

When the user requests a model download, the app connects directly to the official host listed for that verified package. GitHub and model hosts may process ordinary connection data such as the user's IP address, request time, device network information, and requested URL under their own privacy policies.

Scripts, reference recordings, and generated speech are not uploaded by Kitten Studio.

## Permissions

- **Notifications:** requested when starting a model download so Android can show foreground progress. A denied permission does not give Kitten Studio access to other data.
- **Microphone:** requested only after the user enters the authorized voice-sample flow and taps Record. Users can choose a WAV file instead.
- **Network access:** used for catalog checks, user-initiated voice previews, and model downloads.

## Sharing and export

Kitten Studio shares or exports a generated WAV only after the user explicitly chooses that action and selects a destination or receiving app.

## Children

Kitten Studio is not directed to children and should not be used to clone a person’s voice without clear authorization.

## Changes and contact

Material policy changes should be reflected in the app and on the public policy URL before a new Play Store release.

Questions about this policy can be filed through the public Kitten Studio GitHub repository: <https://github.com/rhythmkr360-png/kitten-studio/issues>.
