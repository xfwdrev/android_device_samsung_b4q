# TWRP Device Tree for Samsung Galaxy Z Flip4

The Galaxy Z Flip4 (codenamed _"b4q"_) is a flagship foldable smartphone from Samsung.

It was announced in August 2022 and released in August 2022.

## Device specifications

| Feature                        | Specification                                                                             |
| -----------------------------: | :---------------------------------------------------------------------------------------- |
| Chipset                        | Qualcomm SM8475 Snapdragon 8+ Gen 1                                                       |
| CPU                            | Octa-core (1x3.19 GHz Cortex-X2 & 3x2.75 GHz Cortex-A710 & 4x1.80 GHz Cortex-A510)        |
| GPU                            | Qualcomm Adreno 730                                                                       |
| Memory                         | 8GB RAM (LPDDR5X)                                                                         |
| Shipped OS                     | Android 12 (One UI 4.1)                                                                   |
| Storage                        | 128GB / 256GB (UFS 3.1)                                                                   |
| SIM                            | Nano-SIM + eSIM                                                                           |
| MicroSD                        | No                                                                                        |
| Battery                        | 3700mAh Li-Po (non-removable), 25W fast charge                                            |
| Dimensions                     | Unfolded: 165.2 x 71.9 x 6.9 mm, Folded: 84.9 x 71.9 x 15.9-17.1 mm                       |
| Display                        | 6.7", 1080 x 2640 pixels, 20:9 ratio, Foldable Dynamic AMOLED, 120Hz (~426 ppi density)   |
| Rear Camera 1 (S5K2LD)         | 12 MP, f/1.8, 24mm (wide), 1/1.76", 1.8µm, dual pixel PDAF, OIS                           |
| Rear Camera 2 (IMX258)         | 12 MP, f/2.2, 13mm, 123˚ (ultrawide), 1/3.06", 1.12µm                                     |
| Front Camera (S5K3J1)          | 10 MP, f/2.4, 26mm (wide), 1/3.0", 1.22µm                                                 |
| Fingerprint                    | Goodix GW36T1 (side-mounted)                                                              |
| Sensors                        | Accelerometer, Gyro, Proximity, Compass, Barometer, Hall IC, Grip                         |
| Extras                         | Dual speakers, NFC, MST                                                                   |

## Kernel source 

Available at [https://github.com/xfwdrev/android_kernel_samsung_sm8475](https://github.com/xfwdrev/android_kernel_samsung_sm8475)

## How to build

This device tree was tested and is fully compatible with [Orangefox](https://wiki.orangefox.tech).

1. Set up the build environment following the instructions [here](https://wiki.orangefox.tech/en/dev/building)

2. In the root folder of the fetched repo, clone the device tree:

```bash
git clone https://github.com/xfwdrev/android_device_samsung_b4q.git -b android-12.1 device/samsung/b4q
```

3. To build:

```bash
export ALLOW_MISSING_DEPENDENCIES=true
. build/envsetup.sh
lunch twrp_b4q-eng
mka recoveryimage
```

## Copyright

```
#
# Copyright (C) 2022 The TWRP Open Source Project
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#      http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
#
```