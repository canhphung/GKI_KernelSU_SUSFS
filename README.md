# Droidspaces GKI 5.15.178

This fork builds one Android 13 GKI kernel artifact:

`android13-5.15.178-2025-03-AnyKernel3.zip`

It includes SukiSU Ultra, SUSFS, and the Droidspaces GKI support required by
the upstream [Kernel Configuration Guide](https://github.com/ravindu644/Droidspaces-OSS/blob/main/Documentation/Kernel-Configuration.md):

- the mandatory SYSVIPC kABI patch for kernels below 6.12;
- the recommended Droidspaces GKI configuration options;
- no 5.10 POSIX mqueue patch, because this target is kernel 5.15.

Run **Build Droidspaces GKI 5.15.178** from the Actions tab. A successful run
publishes a release containing only the AnyKernel3 ZIP above.

> Flashing a custom kernel can prevent the device from booting. Keep a known-good
> stock boot image available for recovery.
