# This is an outdated fork! Please see [the upstream repository](https://github.com/minidisc-wiki/md-firmware) instead.

# md-firmware
Firmware dumps for MiniDisc recorders!

## About
In this repository, you can find the firmware for various portable MiniDisc players. It is part of an ongoing effort to reverse engineer said devices.

## Hardware revisions
The major difference between firmware versions is related to the SoC used. 


### Recorders
| **SoC** | **Description**  | **Flash size** | **SRAM size**   | **DRAM size**    | **CPU Core**  |
|---------|------------------|----------------|-----------------|------------------|---------------|
| CXD2671 | Type-R           | 0x60000 (384k) | 0x4000 (16k)    |                  | ARM7TDMI      |
| CXD2674 | Type-R           |                |                 |                  |               |
| CXD2677 | Type-R NetMD     | 0x70000 (448k) | 0x4800 (18k)    | 2MiB             | ARM7TDMI      |
| CXD2678 | Type-S NetMD     | 0xA0000 (640k) | 0x9000 (36k)    | 16MiB            | ARM7TDMI      |
| CXD2680 | Type-S NetMD     | 0xA0000 (640k) | 0x9000 (36k)    | 2MiB             | ARM7TDMI      |
| CXD2681 | NetMD, HiMD      | 1MiB           | 64k             | 16MiB            | ARM7TDMI+     |
| CXD2683 | NetMD, HiMD, Camera  | -          | -               | -                |               |
| CXD2687 | NetMD, HiMD, Latest? | 1MiB       | 32k             | 16MiB            | ARM7TDMI+     |            

### Players

| **SoC** | **Flash size** | **Ram size** |  **DRAM size** | **CPU Core** | **Description** |
|---------|----------------|--------------|----------------|--------------|-----------------|
| CXD2679 | 0x40000 (256k) | 0x3000 (12k) |                | ARM7TDMI     | No USB          |

## Available dumps
Generally, the firmware for devices that share the same SoC is the same (per version), regardless of the exact model. Minor patches may have been applied to the firmware (from the factory), so dumps can vary slightly (a couple of bytes) between devices.

| **CXD2671** | **Dumped devices**                                             |
|-------------|----------------------------------------------------------------|
| v1.3        | MZ-R700                                                        |

| **CXD2677** | **Dumped devices**                                             |
|-------------|----------------------------------------------------------------|
| v1.0        | MZ-N1                                                          |
| v1.1        | MZ-S1                                                          |
| v1.2        | MZ-N1                                                          |
| v1.3        | MZ-N505, MZ-N707                                               |
| v1.4        | MZ-N505, MZ-N1                                                 |

| **CXD2679**           | **Dumped devices**                                             |
|-----------------------|----------------------------------------------------------------|
| v1.0                  | MZ-E520                                                        |

| **CXD2678 - CXD2680** | **Dumped devices**                                             |
|-----------------------|----------------------------------------------------------------|
| v1.1                  | MZ-N10                                                         |
| v1.2                  | MZ-N510                                                        |
| v1.3                  | MZ-N10, MZ-NE410                                               |
| v1.4                  | MZ-N910                                                        |
| v1.5                  | MZ-N510                                                        |
| v1.6                  | MZ-N10, MZ-NE410, MZ-N510, MZ-NF520D, MZ-NF610, MZ-N710, MZ-N910, AIWA AM-NX9 |
| v1.0                  | MZ-N920 (v1.0 for the N920 seems to be newer than v1.6)        |
| _Note_                | _CXD2678 and CXD2680 devices share the same firmware_          |

| **CXD2681**           | **Dumped devices**                                             |
|-----------------------|----------------------------------------------------------------|
| v1.000                | MZ-RH10, MZ-RH910                                              |
| v1.100                | MZ-NH700, MZ-NH900                                             |
| v1.10A                | MZ-NH600                                                       |

| **CXD2687**           | **Dumped devices**                                             |
|-----------------------|----------------------------------------------------------------|
| v1.0A0                | MZ-RH1                                                         |
