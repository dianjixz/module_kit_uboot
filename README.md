# MODULE_LLM_UBOOT
Patch for the uboot adapted for the module_llm development board.  
Compilation will automatically download and apply the relevant patches to compile into a uboot project.  


auto compile:
```bash
source /opt/gcc-linaro-7.5.0-2019.12-x86_64_aarch64-linux-gnu/bash.bashrc
make ARCH=arm CROSS_COMPILE=aarch64-linux-gnu- AX630C_m5stack_LITE_defconfig
make ARCH=arm CROSS_COMPILE=aarch64-linux-gnu- -j `nproc`
axp_pack_bin ./u-boot-dtb.bin u-boot_signed.bin
```

just Extract:
```bash
make Extracting
```

just Patch:
```bash
make Patching
```

just Configur:
```bash
make Configuring
```