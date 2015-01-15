# android-quickeditor
A text editor to open and modify text files based on Querying samples for Google Drive Android API.

## News
* Added the missing code for opening files.
* Corrected incorrect consumption of PendingResults.
* Added guard for attempt to access GoogleApiClient without being connected.
* Changed get to MODE_READ_ONLY to work correctly with DriveContents.getInputStream.
* Ported to Android-Studio.
* Added keys to gradle file.

## How to launch
Open build.gradle and change the following:
```
    signingConfigs {
        config {
            keyAlias 'YOUR_KEY_NAME'
            keyPassword 'YOUR_KEY_PWD'
            storeFile file('YOUR_KEYSTORE_PATH')
            storePassword 'YOUR_KEYSTORE_PWD'
        }
    }
```
Remember to get the SHA1 fingerprint and register it in your Google APIs Console.
