# 203 Entrance firmware

Signed OTA release assets for the ESP32-C3 Super Mini with 4 MB flash.

Source, setup, CLI and documentation: [Achxy/203-entrance](https://github.com/Achxy/203-entrance). Hardware evidence: [validation record](https://github.com/Achxy/203-entrance/blob/main/docs/validation.md).

Install only after USB provisioning using your device's local HTTPS console or the certificate-pinned CLI. The device verifies native RSA-3072 application signatures and signed manifests. Downloads require an optional 2.4 GHz Internet uplink; local management remains available on the device hotspot. Installation and reboot are administrator initiated.

Each release contains `firmware.bin`, `manifest.json`, `manifest.sig`, `signing-public.pem`, `source.json` and `SHA256SUMS`. GitHub prereleases are qualification candidates. Consult the validation record before treating a release as hardware qualified.

Public signing PEM SHA-256: `9f68e10ee55995cf51babeb6aa6567457275a0fa15c9f9971fcbac24d5bd54a6`.

This repository contains no production private keys, device passwords, full-flash backups or device-specific certificates. Bootloader and partition-table replacement require USB recovery.
