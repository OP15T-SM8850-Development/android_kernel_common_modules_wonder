# Wonder for OnePlus 15T

## Upstream source

This repository is based on Google's official AOSP Wonder kernel module:

- Repository: [kernel/common-modules/wonder](https://android.googlesource.com/kernel/common-modules/wonder/)
- Upstream tag used for the current update: `android17-6.18_v3.6.6`
- Upstream commit: [`ae3c841469c64e69eb0739e01f8f4a356bf57c56`](https://android.googlesource.com/kernel/common-modules/wonder/+/ae3c841469c64e69eb0739e01f8f4a356bf57c56)

## OnePlus adaptation

The `android16-6.12-op15t` branch adapts the upstream module for the OnePlus 15T's Qualcomm CNSS Wi-Fi driver and Android kernel 6.12. Local changes provide platform/component registration, compatibility with kernel 6.12 mac80211 callbacks and debugfs helpers, and per-instance resource cleanup.

The matching Qualcomm provider integration is maintained in [android_kernel_oneplus_sm8850-modules](https://github.com/OP15T-SM8850-Development/android_kernel_oneplus_sm8850-modules/tree/lineage-24.0-op15t). Firmware capabilities remain reported by the driver; this port does not force channel-hopping or HBS capability flags.
