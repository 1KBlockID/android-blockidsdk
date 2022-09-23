## BlockID SDK
- Overview - https://developer.1kosmos.com/devportal/docs/mobile-sdk/overview
- Integration Guide - https://developer.1kosmos.com/devportal/docs/mobile-sdk/android/integration-guide
- API Reference - https://developer.1kosmos.com/devportal/docs/mobile-sdk/android/api-reference

## Change Logs

### v1.8.03
- Change isSdkLocked() method to isSDKUnLocked()

### v1.8.02
- Crash fixed during account recovery process using recovery phrases

### v1.8.00
- Upgraded gradle dependency and wrapper
- Register FIDO2 key
- Renew smart card certificates

### v1.7.52
- Returns error during user linking flow w.r.t Sim Binding capability

### v1.7.50
- Updated error code for license check

### v1.7.40
- Bugs fixed - SDK throws error K_SOMETHING_WENT_WRONG during authentication (when scope = windows)

### v1.7.30
- Returns date in yyyyMMdd format after document scan 
- Error handling for various APIs

### v1.7.20 
- Bug Fixed

### v1.7.00
- Introduced new method to set dvcId (document verifier connector identifier)
- Modify verifyDocument() method signature for verifications type parameter 
- Enhance face compare

### v1.6.20
- Introduce capability to register and authenticate FIDO2 security keys 
- Bug Fixed

### v1.6.10
- Added additional events for analytics

### v1.6.00
- Bugs fixed

### v1.4.100
- Bugs fixed
   - SDK throws error code 436 during document registration
   - LiveID scan should reset when user's face is out of focus

### v1.4.99
- Bug fix - SDK throws error 'invalid driver license' when the user scans the back side of any driver license

### v1.4.98
- Provides one step NationalID back scan feature

### v1.4.97
- Bug fix- Scan liveID with liveness check is not working on LG device

### v1.4.96
- Provides Document Verification Service for face liveness check

### v1.4.95
- Provides an option to bypass PoI (Proof of Identity) based on License module configuration
- Provides one step passport scan feature

### v1.4.94
- Fixed PDF417 scan issue on LG device
- Improved PDF417 scan time
