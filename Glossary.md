Useful terms to know.

Add terms specific to the hardware, reverse engineering, and Apple ecosystems that are relevant. Don't add things that everyone is expected to know (CPU, GPU, HDD, SSD, OSX, USB, HDMI, RAM, etc.) or which are not likely to be relevant to the project. Think of the target audience as "random Linux developer".

If you want to collect a large set of terms specific to a sub-field (such as GPUs), feel free to create a separate page.

### 1
* **1TR**: One True Recovery. The recovery partition in M1 Macs, running with full codesigning. Boot with the power button held down. You get root access, but you can only run software signed by Apple. From here you can change the Mac's security settings.

### A
* **AGX**: The internal name for Apple's GPU series.
* **AIC**: Apple Interrupt Controller. Apple's custom ARM interrupt controller, because the standard GIC was too standard for Apple.
* **ANS**: NVME / storage coprocessor?
* **AP**: Application Processor. The main CPU running most of the OS. Contrast to SEP.
* **APFS**: Apple File System. Apple's new container and volume oriented "modern" filesystem, think ZFS and btrfs.
* **APFS Container**: a physical partition on a disk that can itself contain multiple filesystems (volumes), all dynamically sharing space.
* **APFS Snapshot**: a read-only copy-on-write snapshot of an APFS volume.
* **APFS Volume**: a logical filesystem within an APFS container, that can be mounted on a directory.
* **ASC**: Possible generic name for Coprocessors? e.g. gfx-asc


### B
* **BootROM**: A read-only memory embedded in a chip such as the M1, which is the first code executed upon boot.

### C
* **Chicken Bits**: Otherwise known as "kill bits", configuration bits used for disabling/enabling specific features.

### D
* **DART**: Device Address Resolution Table. Apple's custom IOMMU.
* **DFR**: Dynamic Function Row. Apple's internal name for the Touch Bar.
* **DFU**: Device Firmware Update. A USB mode that allows flashing a device's firmware over USB. Apple devices support this in the SecureROM, to allow the user to restore devices which have otherwise been bricked.

### E
* **EEPROM**: Electrically Erasable Programmable Read Only Memory. A type of re-writable memory, commonly available in sizes of a few kilobytes at most, more robust than NOR Flash. Often used for settings and very early boot code.

### F
* **fuOS**: Custom OS, speculated to mean "fully untrusted OS".
* **Fallback Recovery OS**: 2nd copy of recovery OS accessed by double clicking and holding power button to boot. Unlike 1TR is unable to change security state(settings). Can be distinguished from Recovery OS 1TR by Utilities missing "Start Security Utility" option under Utilities

### G
* **GPT**: GUID Partition Table: A partition table format created for EFI/UEFI and now used on most modern systems.
* **GXF**: probably Guarded Execution Function. Lateral exception levels used to create a low-overhead hypervisor to protect pagetables and equally important structures from XNU itself. See e.g. [Sven's write-up](https://blog.svenpeter.dev/posts/m1_sprr_gxf/) or [[HW:-SPRR-and-GXF]]

### H
* **HFS+**: Hierarchical Filesystem+: Apple's previous filesystem, used for external storage. Not used for internal storage on M1 Macs.

### I
* **I²C**: Inter-Integrated Circuit. A 2-wire standard for communicating at low speed between chips on a board.
* **iBoot**: Apple's bootloader. Can refer to the specific second-stage loader on the OS Preboot partition, or to the LLB, iBSS or iBEC.
* **iBSS**: iBoot Single Stage. Replacement for the first-stage iBoot (LLB), loaded in the DFU boot flow when the NOR is corrupted.
* **iBEC**: iBoot Epoch Change. Replacement for the second-stage iBoot, loaded in the DFU boot flow.
* **IPI**: Inter-processor interupt. An interrupt used by one processor to interrupt another.
* **iSC**: iBoot System Container. A disk partition (usually first on the internal SSD) containing the system wide boot data. (See [[SW:Storage]])

### J
* **JTAG**: Joint Test Action Group. Actually refers to a debugging interface released by that group, a 4/5-wire interface to debug chips and CPUs at the hardware level.

### K
* **kASLR**: kernel Address Space Loacation Randomization: Linux kernel feature randomizes where the kernel code is placed in memory at boot time. Disabled by specifying `nokaslr` boot flag.
* **kcOS**: OS with a custom kernel cache.
* **Kernel cache**: A bundle of the kernel and its extensions, optionally encrypted.
* **kmutil** macOS Kernel Management utility for managing kernel extensions (kexts). Used to boot alternative kernels i.e. m1n1

### L
* **LLB**: Low Level Bootloader. The first-stage iBoot located in NOR, loaded by the SecureROM. It chainloads the second-stage iBoot on the OS Preboot partition.

### M
* **Mux**: Multiplexer, a device that can connect one of several things to a single connection, such a switching one set of pins between USB, UART, and SWD modes.
* **Mini** - Custom bootloader for internal investigation. May or may not support booting from SSD. This project uses a fork that's referred to as M1N1.

### N
* **NAND**: Not-AND. A type of logic gate, but normally refers to a type of Flash memory, which is the one used on all modern high-capacity Flash-based storage such as SD cards and SSDs, but also comes in bare chips.
* **NOR**: Not-OR. A type of logic gate, but normally refers to a type of Flash memory, which is only used for low-capacity applications (up to a few megabytes at most). More robust than NAND. Usually comes in bare 8-pin chips these days.
* **NVRAM**: Non-Volatile RAM. The name is obsolete, it just means a list of key=value parameters stored in a Mac for boot configuration. Akin to UEFI variables.

### R
* **RecoveryOS:** The recovery environment, either the 1TR located on the internal disk, or a recovery environment associated with any particular macOS install, located inside an APFS subvolume.
* **RestoreOS:** The restore environment, loaded onto the device when "reviving" it through DFU mode by Apple Configurator. [[more info]](https://www.theiphonewiki.com/wiki/Restore_Ramdisk)
* **RTKit:** Apple's proprietary real-time operating system. Most of the accelerators (AGX, ANE, AOP, DCP, AVE, PMP) run RTKit on an internal processor. The string "RTKSTACKRTKSTACK" is characteristic of a firmware containing RTKit.

### S
* **SBU**: Sideband Use. Two pins on Type C connectors free to be used for random stuff, not defined by the Type C standard itself.
* **SecureROM**: The BootROM of the M1. This is in charge of reading SFR from NOR and passing control to it, or falling back to DFU mode.
* **SEP**: Secure Enclave Processor. The M1's built-in HSM/TPM/etc device. Handles Touch ID and most crypto, as well as boot policy decisions. Harmless to Linux, but we can use its features if we want to. Contrast to AP.
* **SFR**: System Firmware, the portion of firmware stored in NOR flash. This includes the first stage of iBoot, which will boot the second stage from the OS partition.
* **SIP**: System Integrity Protection. Also called "rootless", where the macOS kernel stops even root from doing some things.
* **SOP**: Start Of Packet. Used to differentiate packet types in USB-PD. SOP for normal comms, SOP' and SOP" to talk to built-in chips in a cable, SOP'DEBUG and SOP"DEBUG for custom vendor specific things like Apple VDMs.
* **SPI**: Serial Peripheral Interface. A 4-wire standard for communicating at low speed between chips on a board.
* **SPRR**: probably Shadow Permission Remap Registers. Turns the normal page permission attributes (AP,PXN,UXN) into an index to a separate table. This new table then determines the real page permissions. Also disallows pages that writeable and executable at the same time. See e.g. [Sven's write-up](https://blog.svenpeter.dev/posts/m1_sprr_gxf/) or [[HW:-SPRR-and-GXF]]
* **SWD**: Serial Wire Debug. A 2-pin interface used for debugging ARM cores, like JTAG over fewer pins. Used on Apple devices, but inaccessible (for the main CPU/SoC) in production devices due to security restrictions.

### T

* **TBT**: Thunderbolt Technology

### U
* **UART**: Universal Asynchronous Receiver Transmitter. The hardware behind a serial port.
* **USC**: Unified shader core. A shader core supporting all shader types (vertex, fragment, compute). AGX is a unified architecture, so this just refers to a shader core.
* **USB-PD**: USB Power Delivery. A standard for side-band communications over USB Type C (we won't talk about the older standard for our own sanity). This is used for things like detecting what kind of cable is used, connector orientation, configuring the supply voltage, and switching to non-USB modes.

### V
* **VBUS**: USB pin delivering power. Defaults to 5V, can go as high as 20V with USB-PD.
* **VDM**: Vendor Defined Message. Used for both USB Alternate Mode (not actually proprietary) and vendor-proprietary commands over USB-PD. Apple uses these to configure special modes on their Type C ports.
* **VHE**: Virtual Host Extensions. Extra Registers to allow more efficient switching between OS/VMs/User-space. See [ARM VHE explanation](https://developer.arm.com/documentation/102142/0100/Virtualization-Host-Extensions)