# Release Notes

## v0.2.0
- Adds support for YubiKeys that use AES management keys
- Adds support for larger RSA key sizes on YubiKeys that support larger RSA key sizes. For devices that support larger RSA key sizes, a 3072-bit RSA key is generated during pre-enrollment (instead of the default 2048-bit key). During enrollment and user key management, key sizes are dictated by the payloads supplied by the Purebred portal. If a device does not support a requested key size, a 2048-bit key is generated instead. Recovery operations that attempt it installed an RSA key larger than the target YubiKey supports will fail.
- Copy and paste functionality now works in GUI mode on macOS
- YubiKey reset capability is now available on macOS on x86_64 hardware
