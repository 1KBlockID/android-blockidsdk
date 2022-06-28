# Change Logs
- v1.7.40
1. Bugs fixed
   - SDK throws error K_SOMETHING_WENT_WRONG during authentication (when scope = windows)

- v1.7.30
1. Returns date in yyyyMMdd format after document scan 
2. Error handling for various APIs

- v1.7.20 
1. Bug Fixed

- v1.7.00
1. Introduced new method to set dvcId (document verifier connector identifier)
2. Modify verifyDocument() method signature for verifications type parameter
3. Enhance face compare

- v1.6.20
1. Introduce capability to register and authenticate FIDO2 security keys
2. Bug Fixed

- v1.6.10
1. Added additional events for analytics

- v1.6.00
1. Bugs fixed

- v1.4.100
1. Bugs fixed
   - SDK throws error code 436 during document registration
   - LiveID scan should reset when user's face is out of focus
    
- v1.4.99
1. Bug fix - SDK throws error 'invalid driver license' when the user scans the back side of any driver license

- v1.4.98
1. Provides one step NationalID back scan feature

- v1.4.97
1. Bug fix- Scan liveID with liveness check is not working on LG device

- v1.4.96
1. Provides Document Verification Service for face liveness check

- v1.4.95
1. Provides an option to bypass PoI (Proof of Identity) based on License module configuration
2. Provides one step passport scan feature

- v1.4.94
1. Fixed PDF417 scan issue on LG device
2. Improved PDF417 scan time
