## BlockID SDK

- Overview - https://developer.1kosmos.com/devportal/docs/mobile-sdk/overview
- Integration Guide - https://developer.1kosmos.com/devportal/docs/mobile-sdk/android/integration-guide
- API Reference - https://developer.1kosmos.com/devportal/docs/mobile-sdk/android/api-reference

## Installation

- BlockID SDK is available through Gradle dependency.
- To install it, simply add the following line to your build.gradle\
  implementation 'com.onekosmos.blockid.sdk:blockidsdk:1.9.50.64BE5DD8'

> **Notes**:
> - This repository does not carry the binary

## Change Logs

### v1.9.51
- Bug Fixes related to custom FIDO2 NFC fetaures.

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
