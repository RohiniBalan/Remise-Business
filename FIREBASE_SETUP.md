# Firebase Setup Instructions for Remise Business App

The Remise Business App is configured with Android package name `com.remiseapp.business`.

## Setup Steps

1. Open the [Firebase Console](https://console.firebase.google.com/).
2. Select the existing Remise project: **`remise-4b221`** (Project Number: `147544305027`).
3. Navigate to **Project Settings** (gear icon) → **General** tab.
4. Scroll down to the **Your apps** section and click **Add app** (select **Android** icon).
5. Enter the following details:
   - **Android package name**: `com.remiseapp.business`
   - **App nickname**: `Remise Business`
   - *(Optional)* Debug signing certificate SHA-1: can be added for debug authentication if needed.
6. Click **Register app**.
7. Download the updated **`google-services.json`** file.
8. Replace this file at:
   `C:\Porulon-Project\Remise\Remise-Business-App\android\app\google-services.json`
9. Rebuild the Android project.

> **Note:** The current `google-services.json` contains a placeholder client block for `com.remiseapp.business` so that native Gradle checks recognize the package name. Replace it with the official downloaded file for live push notifications.
