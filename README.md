The Xiaomi Redmi Note 7 (codenamed _"lavender"_) is a mid-range smartphone from Xiaomi announced in January 2019.

## Device specifications

| Device                  | Xiaomi Redmi Note 7                                         |
| ----------------------- | :---------------------------------------------------------- |
| SoC                     | Qualcomm SDM660 Snapdragon 660                              |
| CPU                     | 8x Qualcomm® Kryo™ 260 CPU up to 1.8GHz                     |
| GPU                     | Adreno 512                                                  |
| Memory                  | 3GB / 4GB / 6GB RAM (LPDDR4X)                               |
| Shipped Android version | 9                                                           |
| Storage                 | 32 / 64 / 128GB eMMC 5.1 flash storage                      |
| MicroSD                 | Up to 256 GB                                                |
| Battery                 | Non-removable Li-Po 4000 mAh                                |
| Dimensions              | 159.21 x 75.21 x 8.1 mm                                     |
| Display                 | 2340 x 1080 (19:5:9), 6.3 inch                              |
| Rear camera 1           | 48 MP, f/1.8, (wide), 1/2", 0.8µm, PDAF (Indian/Global)     |
| Rear camera 2           | 2 MP, f/2.4, depth sensor or 5 MP, f/2.2, depth sensor      |
| Front camera            | 13 MP, f/2.0, 1.12µm                                        |


## Device picture

![Xiaomi Redmi Note 7](https://i01.appmifile.com/webfile/globalimg/products/pc/redmi-note7/gallery1-2.jpg)

***

## For building LineageOS 20
Create '.repo/local_manifests/roomservice.xml' with the following content:
```
<?xml version="1.0" encoding="UTF-8"?>
<manifest>

  <project name="LineageOS/android_hardware_xiaomi" path="hardware/xiaomi" remote="github" revision="lineage-21" />

  <project name="MossyTC/android_kernel_xiaomi_sdm660" path="kernel/xiaomi/sdm660" remote="github" revision="lineage-21" />
  <project name="MossyTC/android_device_xiaomi_sdm660-common" path="device/xiaomi/sdm660-common" remote="github" revision="lineage-21" />
  <project name="MossyTC/android_device_xiaomi_lavender" path="device/xiaomi/lavender" remote="github" revision="lineage-21" />
  <project name="MossyTC/android_vendor_xiaomi_sdm660-common" path="vendor/xiaomi/sdm660-common" remote="github" revision="lineage-21" />
  <project name="MossyTC/android_vendor_xiaomi_lavender" path="vendor/xiaomi/lavender" remote="github" revision="lineage-21" />

</manifest>
```
