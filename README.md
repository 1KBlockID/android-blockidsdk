## BlockID SDK

- Overview - https://developer.1kosmos.com/devportal/docs/mobile-sdk/overview
- Integration Guide - https://developer.1kosmos.com/devportal/docs/mobile-sdk/android/integration-guide
- API Reference - https://developer.1kosmos.com/devportal/docs/mobile-sdk/android/api-reference

## Installation

- BlockID SDK is available through Gradle dependency.
- To install it, simply add the following line to your build.gradle\
  implementation 'com.onekosmos.blockid.sdk:blockidsdk:1.20.55.68CBE323'

> **Notes**:
> - This repository does not carry the binary

## Change Logs

### v1.20.55
- Added support for Passkey registration and verification

### v1.20.54
- Fixed an issue on removing account

### v1.20.53
- Added updateAccounts function

### v1.20.51
- Added nonce signing during authentication

### v1.20.50
-  Just a version bump-up to aligned releases

### v1.20.40
- Added Android 15 support.
- Removed FIDO functionality
- Bug fixes

### v1.20.30
- Upgraded AGP version to 8.8.0 
- Upgraded Java version to 17
- Remove support for Android 7.1 hence minSdkVersion set to 26 
- Bug fixes

### v1.20.20
- Updated caching duration for fetch configuration api
- Bug fixes and other improvements

### v1.20.10
- Updated default trusted sources

### v1.20.00
- Introduced a new method that enables face liveness and face compare to run in parallel, enhancing the Live ID authentication process.

### v1.10.92
- Bug fixes

### v1.10.91
- Bug fixes

### v1.10.90 
- Added functionality to get removed accounts

### v1.10.80
- Code clean up (Removed addNativeAccount function which was used to add account using UWL1 QR code)

### v1.10.71
- Bug fixed related to camera start while scanning QR or LiveID 

### v1.10.70
- Introduced live id identifiers
- Bug fixes

### v1.10.60
- Remove use of jcenter() 
- Updated network library so that it will fetch from jitpack.io and not from jcenter()
- Bug fixes 

### v1.10.50
- Enhanced passive LiveID messaging by adding an error code and message
- Always show the capture button during LiveID scanning.
- Changed QR code scanning to work on non-gms devices
  
### v1.10.40 
- Bug fixes

### v1.10.32
- Removed WalletConnect

### v1.10.30
- Added FacePresenceLevel for LiveID scan.
- Updated authenticate user function to record auth factor.
- Bug fixes

### v1.10.21
- Added events for app reset and account removal.
- Changed the prototype for resetSDK() for recording the reason.

### v1.10.20
- Removed expressions prompts during LiveID scanning.
- Added Android 14 support.

### v1.10.10
- Updated tenant registration to derive root tenant if the application supplies client tenant
- Added restoration of wallet and documents through LiveID Selfie

### v1.10.00
-  Just a version bump-up to aligned releases

### v1.9.90
-  The legacy scanners have been substituted with a new web based ID proofing experience 
-  Introduced FIDO2 Pin Management functionality

### v1.9.83
-  Fixed error handling for ACR code redemption

### v1.9.80
- Added a new function to issue a scep certificate for non scep users
- Fixed a bug where a wrong error was being returned during FIDO2 security key authentication
- Updated IP Address provider to efficiently fetch and cache IP addresses

### v1.9.70
- Enhanced device details now include device name, make and model for improved reporting capabilities.

### v1.9.60
- Used user define device name instead of device make and model
- Removed unused gradle dependencies
- Fixed functions typo errors

### v1.9.51
- Fixed unintended NFC prompts and crashes caused by the Fido2Authenticator SDK's intent-filter configuration.

### v1.9.50
- Handled auth requests for linked accounts when tenant has two DNS mappings.
- Improved the FIDO2 security key registration and authentication process.
- Updated the FIDO2 security function to require pin verification before registering or authenticating the FIDO2 security key.

### v1.9.40
- Added a new function to fetch user documents which are registered against application DID
- Added a new function to update linked account Device Info and Push ID

### v1.9.30

- Added a new function to consume Verifiable Credentials
- Added a new function to generate Verifiable Presentations which allows for the sharing of VCs with verifiers
- Fixed FIDO2 authentication failure caused by multiple registrations of the same security key for a user. Now, one security key can only be registered once for a user, ensuring unique and secure authentication
