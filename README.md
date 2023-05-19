## BlockID SDK
- Overview - https://developer.1kosmos.com/devportal/docs/mobile-sdk/overview
- Integration Guide - https://developer.1kosmos.com/devportal/docs/mobile-sdk/android/integration-guide
- API Reference - https://developer.1kosmos.com/devportal/docs/mobile-sdk/android/api-reference

## Installation
- BlockID SDK is available through Gradle dependency. To install it, simply add the following line to your build.gradle:
  implementation 'com.onekosmos.blockid.sdk:blockidsdk:1.9.30.6465D938'

> **Notes**:
> -  This repository does not carry the binary

## Change Logs

### v1.9.30
- Introduced new APIs to get VC and VP
- Fixed FIDO2 authentication failed issue
  - One SECURITY KEY must be registered only once for a userid

### v1.9.21
- To reduce number of API calls, added API caching
- Added keep-alive in some API
- Fixed get IAL API calling even though IAL is not asked in scopes

### v.1.9.20
- Introduced enhance document scanner for National ID scanning
- Revamped IAL calculation logic

### v.1.9.10
- Fixed FIDO2 registration and authentication issue for client tenant

### v.1.9.00
- Consume SDK using gradle dependency
- Introduced enhance selfie scanner for LiveID scanning
- Added liveness check before registering LiveID
- Introduced enhance document scanner for Drivers License scanning
- - Minor bug fixes related to FIDO2 functionality