# PLCT Monthly Report

April 2025

## Suport matrix

- PR: [https://github.com/ruyisdk/support-matrix/pull/216](https://github.com/ruyisdk/support-matrix/pull/216)
  - Add Fedora test reports for Mars.
  - Update Debian test reports for Mars.
  - Fix some typos.
- PR: [https://github.com/ruyisdk/support-matrix/pull/260](https://github.com/ruyisdk/support-matrix/pull/260)
  - Add Guix test reports for Mars
  - Update Ubuntu test reports for Mars.
  - Add Guix to metadata.
- PR: [https://github.com/ruyisdk/support-matrix/pull/253](https://github.com/ruyisdk/support-matrix/pull/253)
  - Add a new board HiFive Premier P550.
  - Add Ubuntu, Yocto and Debian (RockOS) test reports for P550 (CFT version).
- PR: [https://github.com/ruyisdk/support-matrix/pull/276](https://github.com/ruyisdk/support-matrix/pull/276)
  - Add NixOS test reports for Mars.
- PR: [https://github.com/ruyisdk/support-matrix/pull/279](https://github.com/ruyisdk/support-matrix/pull/279)
  - Update Ubuntu test reports to 25.04 for Mars.
- PR: [https://github.com/ruyisdk/support-matrix/pull/281](https://github.com/ruyisdk/support-matrix/pull/281)
  - Add OpenWRT and test reports for Mars.
  - Add NuttX test reports for Mars.
  - Fix some typos.

## GNU toolchain test

- commit: [https://github.com/QA-Team-lo/ruyisdk-gnu-tests/commit/9e87128d587a38412b7aca41651d050a3050e34d](https://github.com/QA-Team-lo/ruyisdk-gnu-tests/commit/9e87128d587a38412b7aca41651d050a3050e34d)
  - JH7110 (Milk-V Mars): Native, Cross both w/ B, w/o B.
  - CV1800B (Milk-V Duo): Cross.

## External testing requirements

- Test FreeRTOS on Milk-V Duo 64MB based on Buildroot SDK v2 <https://github.com/ruyisdk/support-matrix/issues/280> (Completed)
  - MailBox demo doesn't work, it seems that there is no relevant Linux driver in the SDK V2.
  - After the Linux kernel starts up, both the IO control and serial port output of the small-core fail to work properly.
  - During the U-Boot stage, the RTOS can still work properly.

- Test OpenGauss v7.0.0-RC1 on LicheePi 4A based on oERV 24.04 LTS (WIP) <https://github.com/QA-Team-lo/Team-Planning/issues/100>
