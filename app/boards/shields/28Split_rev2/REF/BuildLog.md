# BuildLog.md

202209030800

Last login: Sat Sep  3 07:03:05 on ttys000
source ~/.bashrc
➜  ~ source ~/.bashrc
➜  ~ cd zmk
➜  zmk git:(main) ✗ cd app
➜  app git:(main) ✗ export ZEPHYR_TOOLCHAIN_VARIANT=zephyr
➜  app git:(main) ✗ west build --pristine -b nrfmicro_13 -- -DSHIELD=28split_rev2_left
-- west build: making build dir /Users/stuartliu/zmk/app/build pristine
-- west build: generating a build system
Including boilerplate (Zephyr base): /Users/stuartliu/zmk/zephyr/cmake/app/boilerplate.cmake
-- Application: /Users/stuartliu/zmk/app
-- Adding /Users/stuartliu/zmk/app/boards/shields/28Split_rev2
-- Using keymap file: /Users/stuartliu/zmk/app/boards/shields/28Split_rev2/28split_rev2.keymap
-- Zephyr version: 3.0.0 (/Users/stuartliu/zmk/zephyr)
-- Found Python3: /Library/Developer/CommandLineTools/usr/bin/python3.8 (found suitable exact version "3.8.9") found components: Interpreter
-- Found west (found suitable version "0.13.1", minimum required is "0.7.1")
-- Board: nrfmicro_13, Shield(s): 28split_rev2_left
-- Cache files will be written to: /Users/stuartliu/Library/Caches/zephyr
-- Found host-tools: zephyr 0.14.2 (/Users/stuartliu/zephyr-sdk-0.14.2)
-- Found dtc: /usr/local/bin/dtc (found suitable version "1.6.1", minimum required is "1.4.6")
-- Found toolchain: zephyr 0.14.2 (/Users/stuartliu/zephyr-sdk-0.14.2)
-- Found BOARD.dts: /Users/stuartliu/zmk/app/boards/arm/nrfmicro/nrfmicro_13.dts
-- Found devicetree overlay: /Users/stuartliu/zmk/app/boards/shields/28Split_rev2/28split_rev2_left.overlay
-- Found devicetree overlay: /Users/stuartliu/zmk/app/boards/shields/28Split_rev2/28split_rev2.keymap
-- Generated zephyr.dts: /Users/stuartliu/zmk/app/build/zephyr/zephyr.dts
-- Generated devicetree_unfixed.h: /Users/stuartliu/zmk/app/build/zephyr/include/generated/devicetree_unfixed.h
-- Generated device_extern.h: /Users/stuartliu/zmk/app/build/zephyr/include/generated/device_extern.h
-- Including generated dts.cmake file: /Users/stuartliu/zmk/app/build/zephyr/dts.cmake
Parsing /Users/stuartliu/zmk/app/Kconfig
Loaded configuration '/Users/stuartliu/zmk/app/boards/arm/nrfmicro/nrfmicro_13_defconfig'
Merged configuration '/Users/stuartliu/zmk/app/prj.conf'
Configuration saved to '/Users/stuartliu/zmk/app/build/zephyr/.config'
Kconfig header saved to '/Users/stuartliu/zmk/app/build/zephyr/include/generated/autoconf.h'
-- The C compiler identification is GNU 10.3.0
-- The CXX compiler identification is GNU 10.3.0
-- The ASM compiler identification is GNU
-- Found assembler: /Users/stuartliu/zephyr-sdk-0.14.2/arm-zephyr-eabi/bin/arm-zephyr-eabi-gcc
-- Configuring done
CMake Warning (dev) at /Users/stuartliu/zmk/zephyr/cmake/linker/ld/target.cmake:69 (add_custom_command):
  Policy CMP0116 is not set: Ninja generators transform DEPFILEs from
  add_custom_command().  Run "cmake --help-policy CMP0116" for policy
  details.  Use the cmake_policy command to set the policy and suppress this
  warning.
Call Stack (most recent call first):
  /Users/stuartliu/zmk/zephyr/CMakeLists.txt:1053 (configure_linker_script)
This warning is for project developers.  Use -Wno-dev to suppress it.

CMake Warning (dev) at /Users/stuartliu/zmk/zephyr/cmake/linker/ld/target.cmake:69 (add_custom_command):
  Policy CMP0116 is not set: Ninja generators transform DEPFILEs from
  add_custom_command().  Run "cmake --help-policy CMP0116" for policy
  details.  Use the cmake_policy command to set the policy and suppress this
  warning.
Call Stack (most recent call first):
  /Users/stuartliu/zmk/zephyr/CMakeLists.txt:1265 (configure_linker_script)
This warning is for project developers.  Use -Wno-dev to suppress it.

CMake Warning (dev) at /Users/stuartliu/zmk/zephyr/cmake/linker/ld/target.cmake:69 (add_custom_command):
  Policy CMP0116 is not set: Ninja generators transform DEPFILEs from
  add_custom_command().  Run "cmake --help-policy CMP0116" for policy
  details.  Use the cmake_policy command to set the policy and suppress this
  warning.
Call Stack (most recent call first):
  /Users/stuartliu/zmk/zephyr/CMakeLists.txt:1322 (configure_linker_script)
This warning is for project developers.  Use -Wno-dev to suppress it.

-- Generating done
-- Build files have been written to: /Users/stuartliu/zmk/app/build
-- west build: building application
[1/316] Preparing syscall dependency handling

[2/316] Generating include/generated/version.h
-- Zephyr version: 3.0.0 (/Users/stuartliu/zmk/zephyr), build: 8adeab429a24
[306/316] Linking C executable zephyr/zephyr_pre0.elf

[310/316] Linking C executable zephyr/zephyr_pre1.elf

[316/316] Linking C executable zephyr/zmk.elf
Memory region         Used Size  Region Size  %age Used
           FLASH:      196032 B       792 KB     24.17%
            SRAM:       54290 B       256 KB     20.71%
        IDT_LIST:          0 GB         2 KB      0.00%
Converting to uf2, output size: 392192, start address: 0x26000
Wrote 392192 bytes to zmk.uf2
➜  app git:(main) ✗ west build --pristine -b nrfmicro_13 -- -DSHIELD=28split_rev2_right
-- west build: making build dir /Users/stuartliu/zmk/app/build pristine
-- west build: generating a build system
Including boilerplate (Zephyr base): /Users/stuartliu/zmk/zephyr/cmake/app/boilerplate.cmake
-- Application: /Users/stuartliu/zmk/app
-- Adding /Users/stuartliu/zmk/app/boards/shields/28Split_rev2
-- Using keymap file: /Users/stuartliu/zmk/app/boards/shields/28Split_rev2/28split_rev2.keymap
-- Zephyr version: 3.0.0 (/Users/stuartliu/zmk/zephyr)
-- Found Python3: /Library/Developer/CommandLineTools/usr/bin/python3.8 (found suitable exact version "3.8.9") found components: Interpreter
-- Found west (found suitable version "0.13.1", minimum required is "0.7.1")
-- Board: nrfmicro_13, Shield(s): 28split_rev2_right
-- Cache files will be written to: /Users/stuartliu/Library/Caches/zephyr
-- Found host-tools: zephyr 0.14.2 (/Users/stuartliu/zephyr-sdk-0.14.2)
-- Found dtc: /usr/local/bin/dtc (found suitable version "1.6.1", minimum required is "1.4.6")
-- Found toolchain: zephyr 0.14.2 (/Users/stuartliu/zephyr-sdk-0.14.2)
-- Found BOARD.dts: /Users/stuartliu/zmk/app/boards/arm/nrfmicro/nrfmicro_13.dts
-- Found devicetree overlay: /Users/stuartliu/zmk/app/boards/shields/28Split_rev2/28split_rev2_right.overlay
-- Found devicetree overlay: /Users/stuartliu/zmk/app/boards/shields/28Split_rev2/28split_rev2.keymap
-- Generated zephyr.dts: /Users/stuartliu/zmk/app/build/zephyr/zephyr.dts
-- Generated devicetree_unfixed.h: /Users/stuartliu/zmk/app/build/zephyr/include/generated/devicetree_unfixed.h
-- Generated device_extern.h: /Users/stuartliu/zmk/app/build/zephyr/include/generated/device_extern.h
-- Including generated dts.cmake file: /Users/stuartliu/zmk/app/build/zephyr/dts.cmake
Parsing /Users/stuartliu/zmk/app/Kconfig
Loaded configuration '/Users/stuartliu/zmk/app/boards/arm/nrfmicro/nrfmicro_13_defconfig'
Merged configuration '/Users/stuartliu/zmk/app/prj.conf'
Configuration saved to '/Users/stuartliu/zmk/app/build/zephyr/.config'
Kconfig header saved to '/Users/stuartliu/zmk/app/build/zephyr/include/generated/autoconf.h'
-- The C compiler identification is GNU 10.3.0
-- The CXX compiler identification is GNU 10.3.0
-- The ASM compiler identification is GNU
-- Found assembler: /Users/stuartliu/zephyr-sdk-0.14.2/arm-zephyr-eabi/bin/arm-zephyr-eabi-gcc
-- Configuring done
CMake Warning (dev) at /Users/stuartliu/zmk/zephyr/cmake/linker/ld/target.cmake:69 (add_custom_command):
  Policy CMP0116 is not set: Ninja generators transform DEPFILEs from
  add_custom_command().  Run "cmake --help-policy CMP0116" for policy
  details.  Use the cmake_policy command to set the policy and suppress this
  warning.
Call Stack (most recent call first):
  /Users/stuartliu/zmk/zephyr/CMakeLists.txt:1053 (configure_linker_script)
This warning is for project developers.  Use -Wno-dev to suppress it.

CMake Warning (dev) at /Users/stuartliu/zmk/zephyr/cmake/linker/ld/target.cmake:69 (add_custom_command):
  Policy CMP0116 is not set: Ninja generators transform DEPFILEs from
  add_custom_command().  Run "cmake --help-policy CMP0116" for policy
  details.  Use the cmake_policy command to set the policy and suppress this
  warning.
Call Stack (most recent call first):
  /Users/stuartliu/zmk/zephyr/CMakeLists.txt:1265 (configure_linker_script)
This warning is for project developers.  Use -Wno-dev to suppress it.

CMake Warning (dev) at /Users/stuartliu/zmk/zephyr/cmake/linker/ld/target.cmake:69 (add_custom_command):
  Policy CMP0116 is not set: Ninja generators transform DEPFILEs from
  add_custom_command().  Run "cmake --help-policy CMP0116" for policy
  details.  Use the cmake_policy command to set the policy and suppress this
  warning.
Call Stack (most recent call first):
  /Users/stuartliu/zmk/zephyr/CMakeLists.txt:1322 (configure_linker_script)
This warning is for project developers.  Use -Wno-dev to suppress it.

-- Generating done
-- Build files have been written to: /Users/stuartliu/zmk/app/build
-- west build: building application
[1/279] Preparing syscall dependency handling

[2/279] Generating include/generated/version.h
-- Zephyr version: 3.0.0 (/Users/stuartliu/zmk/zephyr), build: 8adeab429a24
[269/279] Linking C executable zephyr/zephyr_pre0.elf

[273/279] Linking C executable zephyr/zephyr_pre1.elf

[279/279] Linking C executable zephyr/zmk.elf
Memory region         Used Size  Region Size  %age Used
           FLASH:      157725 B       792 KB     19.45%
            SRAM:       37658 B       256 KB     14.37%
        IDT_LIST:          0 GB         2 KB      0.00%
Converting to uf2, output size: 315904, start address: 0x26000
Wrote 315904 bytes to zmk.uf2
➜  app git:(main) ✗
