Device configuration for Sony Xperia 5 II
=========================================

The Sony Xperia 5 II (codenamed _"pdx206"_) is a high-end smartphone from Sony.

It was announced in September 2020. Release date was October 2020.

## Device specifications

Basic        | Spec Sheet
------------:|:-------------------------
SoC          | Qualcomm SM8250 Snapdragon 865
CPU          | Octa-core (1x2.84 GHz Cortex-A77 & 3x2.42 GHz Cortex-A77 & 4x1.80 GHz Cortex-A55)
GPU          | Adreno 650
Memory       | 8 GB RAM
Shipped Android Version | Android 10
Storage      | 128/256 GB
Battery      | Non-removable Li-Ion 4000 mAh battery
Display      | 1080 x 2520 pixels, 21:9 ratio, 6.1 inches, OLED (~449 ppi density)
Rear Camera  | 12 MP (wide) + 12 MP (telephoto) + 12 MP (ultrawide), PDAF, LED flash

## Device picture

![Sony Xperia 5 II](https://wiki.lineageos.org/images/devices/pdx206.png "Sony Xperia 5 II")

***

## For building LineageOS 20
Create '.repo/local_manifests/roomservice.xml' with the following content:
```
<?xml version="1.0" encoding="UTF-8"?>
<manifest>

  <project name="LineageOS/android_hardware_sony" path="hardware/sony" remote="github" revision="lineage-20" />

  <project name="LineageOS/android_device_sony_sm8250-common" path="device/sony/sm8250-common" remote="github" revision="lineage-20" />
  <project name="LineageOS/android_device_sony_pdx206" path="device/sony/pdx206" remote="github" revision="lineage-20" />
  <project name="LineageOS/android_kernel_sony_sm8250" path="kernel/sony/sm8250" remote="github" revision="lineage-20" />
  <project name="LineageOS/proprietary_vendor_sony_sm8250-common" path="vendor/sony/sm8250-common" remote="github" revision="lineage-20" />
  <project name="LineageOS/proprietary_vendor_sony_pdx206" path="vendor/sony/pdx206" remote="github" revision="lineage-20" />

</manifest>
```
