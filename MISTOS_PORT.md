# MistOS Android 17 — coral

Source: its-hecker/evox-coral-dt main, reworked for MistOS.

Product is intentionally lineage_coral: upstream mistify creates lineage_<device>.
The native 3D IR Face HAL is selected (TARGET_SUPPORTS_GFU=true prevents
MistOS generic camera-based FaceUnlock from being packaged).

Preserved: Soli Motion Sense / Oslo overlay and plugin allowlist,
Google Camera 8.7 signed splits, Google Face HAL and framework compatibility
patches, Citadel/Keymaster/camera compatibility blobs, vendor Lunaris Dolby,
A/B Virtual A/B retrofit, and KernelSU Next kernel integration.

Framework face patch must be applied from the local manifest's build.sh,
then verified against the current MistOS frameworks/base source.
Neither compilation nor boot/hardware support is yet verified on MistOS.
