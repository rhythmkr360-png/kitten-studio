# Kitten Studio privacy policy

Effective date: 2026-09-23  
App package: `com.kitten.studio`

Kitten Studio is designed to run speech generation on the user’s Android device.

## Data collection

Kitten Studio does not create an app account and does not include advertising, analytics, crash-reporting, tracking, or cloud speech SDKs. The app developer does not receive scripts, recordings, generated audio, or voice samples through the app. If you use the optional one-time Pro purchase, the app and our Cloudflare service process a Google Play purchase token and Play Integrity proof to verify access to private model downloads. We do not offer a subscription.

## Data stored on the device

Kitten Studio can store the following in app-private storage:

- downloaded speech-model packages;
- a validated copy of the public model catalog;
- voice-preview MP3 files held in Android's temporary cache; files older than six hours are removed when the preview cache is next used;
- scripts currently being edited;
- generated WAV files and their local metadata;
- an optional authorized reference-voice WAV, transcript, display name, and consent timestamp;
- preferences such as appearance, selected voice, and model installation state;
- if Pro is purchased, an encrypted Google Play purchase token protected by Android Keystore. It is used to restore access and request private Pro model files. The app does not store the Play Integrity proof after each request.

Users can remove generated audio, model packages, and the voice reference from Settings. Uninstalling the app removes its app-private data.

## Network use

Kitten Studio checks a public GitHub catalog when the app starts and when the Voices screen is reopened after 15 minutes. This lets newly listed compatible models and corrected preview links appear without an app update.

When the user taps a voice preview, the app downloads that short MP3 from the public Kitten Studio GitHub Release. Android stores it in temporary cache, subject to a 32 MiB cache limit. Files older than six hours are removed on the next preview-cache cleanup; Android may clear them sooner. The preview isn't added to the user's audio library.

When the user requests a free model download, the app connects to the approved HTTPS source in the verified catalog, normally a Kitten Studio GitHub Release. The app checks the downloaded file's expected size and SHA-256 hash. GitHub and any approved model host may process ordinary connection data such as the user's IP address, request time, device network information, and requested URL under their own privacy policies.

If Pro becomes available in this build, the one-time in-app purchase is handled by Google Play Billing, not by a subscription or an external checkout. Google Play handles payment-method details; the developer does not receive card numbers through the app. A new Play Integrity proof is requested when verifying the purchase and when starting or resuming a private model download. The app sends the purchase token and proof over HTTPS to our Cloudflare Worker, which asks Google to verify the purchase and integrity verdict before streaming the requested file from a private GitHub repository. The token and proof are sent in request bodies or headers, not URLs. The Worker does not write them to a database or application log, though Google Play and Cloudflare may process request data under their own policies. Cloudflare handles network metadata such as IP address, request time, and file path. GitHub receives the Worker's download request. A Pro catalog metadata check may occur on app launch; repeat checks during the same running session are throttled to at most once every six hours. Pro purchasing is disabled in builds where the verification service is not configured.

Scripts, reference recordings, and generated speech are not uploaded by Kitten Studio.

## Permissions

- **Notifications:** requested when starting a model download so Android can show foreground progress. A denied permission does not give Kitten Studio access to other data.
- **Microphone:** requested only after the user enters the authorized voice-sample flow and taps Record. Users can choose a WAV file instead.
- **Network access:** used for catalog checks, user-initiated voice previews, model downloads, and optional Play Billing/Integrity purchase checks.

## Sharing and export

Kitten Studio shares or exports a generated WAV only after the user explicitly chooses that action and selects a destination or receiving app.

## Children

Kitten Studio is not directed to children and should not be used to clone a person’s voice without clear authorization.

## Changes and contact

Material policy changes should be reflected in the app and on the public policy URL before a new Play Store release.

Questions about this policy can be sent to the developer, Hysoft, at <Sponsorme360@gmail.com>, or filed through the public Kitten Studio GitHub repository: <https://github.com/rhythmkr360-png/kitten-studio/issues>.
