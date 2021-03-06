## Glossary

Some of these are guesses

* ACC: Apple Core Cluster
* HID: Hardware Implementation Defined Register
* EHID: Hardware Implementation Defined Register (e-core)
* IPI: Inter-processor Interrupt

## Register definitions

Using Linux format:
```c

/* These make sense... */
#define SYS_HID0            sys_reg(3, 0, 15, 0, 0)
#define SYS_HID1            sys_reg(3, 0, 15, 1, 0)
#define SYS_EHID1           sys_reg(3, 0, 15, 1, 1)
#define SYS_HID2            sys_reg(3, 0, 15, 2, 0)
#define SYS_EHID2           sys_reg(3, 0, 15, 2, 1)
#define SYS_HID3            sys_reg(3, 0, 15, 3, 0)
#define SYS_EHID3           sys_reg(3, 0, 15, 3, 1)
#define SYS_HID4            sys_reg(3, 0, 15, 4, 0)
#define SYS_EHID4           sys_reg(3, 0, 15, 4, 1)
#define SYS_HID5            sys_reg(3, 0, 15, 5, 0)
#define SYS_EHID5           sys_reg(3, 0, 15, 5, 1)
#define SYS_HID6            sys_reg(3, 0, 15, 6, 0)
#define SYS_HID7            sys_reg(3, 0, 15, 7, 0)
#define SYS_HID8            sys_reg(3, 0, 15, 8, 0)
#define SYS_HID9            sys_reg(3, 0, 15, 9, 0)
#define SYS_EHID9           sys_reg(3, 0, 15, 9, 1)
#define SYS_HID10           sys_reg(3, 0, 15, 10, 0)
#define SYS_EHID10          sys_reg(3, 0, 15, 10, 1)
#define SYS_HID11           sys_reg(3, 0, 15, 11, 0)
#define SYS_EHID11          sys_reg(3, 0, 15, 11, 1)

/* Uh oh */
#define SYS_HID13           sys_reg(3, 0, 15, 14, 0)
#define SYS_HID14           sys_reg(3, 0, 15, 15, 0)

/* All sanity went out the window here */
#define SYS_HID16           sys_reg(3, 0, 15, 15, 2)
#define SYS_HID17           sys_reg(3, 0, 15, 15, 5)
#define SYS_HID18           sys_reg(3, 0, 15, 11, 2)
#define SYS_EHID20          sys_reg(3, 0, 15, 1, 2)
#define SYS_HID21           sys_reg(3, 0, 15, 1, 3)

#define SYS_LSU_ERR_STS     sys_reg(3, 3, 15, 0, 0)
#define SYS_E_LSU_ERR_STS   sys_reg(3, 3, 15, 2, 0)
#define SYS_LSU_ERR_CTL     sys_reg(3, 3, 15, 1, 0)

#define SYS_L2C_ERR_STS     sys_reg(3, 3, 15, 8, 0)
#define SYS_L2C_ERR_ADR     sys_reg(3, 3, 15, 9, 0)
#define SYS_L2C_ERR_INF     sys_reg(3, 3, 15, 10, 0)

#define SYS_FED_ERR_STS     sys_reg(3, 4, 15, 0, 0)
#define SYS_E_FED_ERR_STS   sys_reg(3, 4, 15, 0, 2)

#define SYS_APCTL_EL1       sys_reg(3, 4, 15, 0, 4)
#define SYS_KERNELKEYLO_EL1 sys_reg(3, 4, 15, 1, 0)
#define SYS_KERNELKEYHI_EL1 sys_reg(3, 4, 15, 1, 1)

#define SYS_VMSA_LOCK       sys_reg(3, 4, 15, 1, 2)

#define SYS_APRR_EL0        sys_reg(3, 4, 15, 2, 0)
#define SYS_APRR_EL1        sys_reg(3, 4, 15, 2, 1)

#define SYS_CTRR_LOCK_EL1   sys_reg(3, 4, 15, 2, 2)
#define SYS_CTRR_A_LWR_EL1  sys_reg(3, 4, 15, 2, 3)
#define SYS_CTRR_A_UPR_EL1  sys_reg(3, 4, 15, 2, 4)
#define SYS_CTRR_CTL_EL1    sys_reg(3, 4, 15, 2, 5)

#define SYS_APRR_JIT_ENABLE sys_reg(3, 4, 15, 2, 6)
#define SYS_APRR_JIT_MASK   sys_reg(3, 4, 15, 2, 7)

#define SYS_s3_4_c15_c5_0   sys_reg(3, 4, 15, 5, 0)

#define SYS_CTRR_LOCK_EL2   sys_reg(3, 4, 15, 11, 5)
#define SYS_CTRR_A_LWR_EL2  sys_reg(3, 4, 15, 11, 0)
#define SYS_CTRR_A_UPR_EL2  sys_reg(3, 4, 15, 11, 1)
#define SYS_CTRR_CTL_EL2    sys_reg(3, 4, 15, 11, 4)

#define SYS_IPI_RR_LOCAL    sys_reg(3, 5, 15, 0, 0)
#define SYS_IPI_RR_GLOBAL   sys_reg(3, 5, 15, 0, 1)

#define SYS_DPC_ERR_STS     sys_reg(3, 5, 15, 0, 5)

#define SYS_IPI_SR          sys_reg(3, 5, 15, 1, 1)
#define SYS_IPI_CR          sys_reg(3, 5, 15, 3, 1)

#define SYS_ACC_CFG         sys_reg(3, 5, 15, 4, 0)
#define SYS_CYC_OVRD        sys_reg(3, 5, 15, 5, 0)
#define SYS_ACC_OVRD        sys_reg(3, 5, 15, 6, 0)
#define SYS_ACC_EBLK_OVRD   sys_reg(3, 5, 15, 6, 1)

#define SYS_MMU_ERR_STS     sys_reg(3, 6, 15, 0, 0)

#define SYS_E_MMU_ERR_STS   sys_reg(3, 6, 15, 2, 0)

#define SYS_APSTS_EL1       sys_reg(3, 6, 15, 12, 4)

```

### HID registers

This naming convention most likely comes from PowerPC. A lot of chicken bits
seem to be located here.

These are mostly chicken bits to disable CPU features, and likely many only apply only to certain CPU generations. However, their definitions are global.

#### SYS_HID0

* [20] Loop Buffer Disable
* [21] AMX Cache Fusion Disable
* [25] IC Prefetch Limit One "Brn"
* [28] Fetch Width Disable
* [33] PMULL Fuse Disable
* [36] Cache Fusion Disable
* [45] Same Pg (page?) Power Optimization
* [62:60] Instruction Cache Prefetch Depth

#### SYS_EHID0

* [45] nfpRetFwdDisb

#### SYS_HID1

* [14] Disable CMP-Branch Fusion
* [15] ForceMextL3ClkOn
* [23] rccForceAllIexL3ClksOn
* [24] rccDisStallInactiveIexCtl
* [25] disLspFlushWithContextSwitch
* [44] Disable AES Fusion across groups
* [49] Disable MSR Speculation DAIF
* [54] Trap SMC
* [58] enMDSBStallPipeLineECO
* [60] Enable Branch Kill Limit / SpareBit6

#### SYS_EHID1

* [30] Disable MSR Speculation DAIF


#### SYS_HID2

* [13] Disable MMU MTLB Prefetch
* [17] Force Purge MTB

#### SYS_EHID2

* [17] Force Purge MTB

#### SYS_HID3

* [2] Disable Color Optimization
* [25] Disable DC ZVA Command Only
* [44] Disable Arbiter Fix BIF CRD
* [54] Disable Xmon Snp Evict Trigger L2 Starvation Mode
* [63] Dev Pcie Throttle Enable

#### SYS_EHID3

* [2] Disable Color Optimization
* [25] Disable DC ZVA Command Only

#### SYS_HID4

* [1] Disable STNT Widget
* [9] Disable Speculative LS Redirect
* [11] Disable DC MVA Ops
* [33] Disable Speculative Lnch Read
* [39] Force Ns Ord Ld Req No Older Ld (Non-speculative Ordered Load Requires No Older Load?)
* [41:40] Cnf Counter Threshold
* [44] Disable DC SW L2 Ops
* [49] Enable Lfsr Stall Load Pipe 2 Issue
* [53] Enable Lfsr Stall Stq Replay

#### SYS_HID5

* [15:14] Crd Edb Snp Rsvd
* [44] Disable HWP Load
* [45] Disable HWP Store
* [54] Enable Dn FIFO Read Stall
* [57] Disable Full Line Write
* [61] Disable Fill 2C Merge

#### SYS_EHID5

* [35] Disable Fill Bypass

#### SYS_HID6

* [9:5] Up Crd Tkn Init C2
* [55] Disable ClkDiv Gating

#### SYS_HID7

* [7] Disable Cross Pick 2
* [10] Disable Nex Fast FMUL
* [16] Force Non Speculative If Spec Flush Ptr Invalid And MP Valid
* [20] Force Non Speculative If Stepping
* [25:24] Force Non Speculative Target Timer Sel

#### SYS_HID8

* [7:4] DataSetID0
* [11:8] DataSetID1
* [35] Wke Force Strict Order
* [59:56] DataSetID2
* [63:60] DataSetID3

#### SYS_HID9

* [16] TSO Enable
* [26] TSO Allow DC ZVA WC
* [29] TSO Serialize VLD Microops
* [48] EnableFixBug51667805
* [49] EnableFixBug51667717
* [50] EnableFixBug57817908
* [52] Disable STNT (Store Non-Temporal?) Widget For Unaligned
* [53] EnableFixBug58566122
* [54] EnableFixBug47221499
* [55] HidEnFix55719865

#### SYS_EHID9

* [5] Dev Throttle 2 Enable

#### SYS_HID10

* [0] Disable Hwp Gups

#### SYS_EHID10

* [19] RCC Disable Power Save Prf (performance?) Clock Off
* [32] Force Wait State Drain UC
* [49] Disable ZVA Temporal TSO

#### SYS_HID11

* [1] Disable X64 NT Lnch Optimization
* [7] Disable Fill C1 Bub(ble?) Optimization
* [15] HID Enable Fix UC 55719865
* [23] Disable Fast Drain Optimization
* [59] Disable LDNT (Load Non-Temporal?) Widget

#### SYS_EHID11

* [41:40] SMB Drain Threshold

#### SYS_HID13

* [17:14] PreCyc
* [63:60] Reset Cycle count

#### SYS_HID14

* [?:0] Nex Sleep Timeout Cyclone
* [32] Nex Power Gating Enable

#### SYS_HID16

* [18] LEQ Throttle Aggr
* [56] SpareBit0
* [57] Enable RS4 Sec
* [59] SpareBit3
* [60] Disable xPick RS 45
* [61] Enable MPx Pick 45
* [62] Enable MP Cyclone 7
* [63] SpareBit7

#### SYS_HID17

* [2:0] Crd Edb Snp Rsvd

#### SYS_HID18

* [14] HVC Speculation Disable
* [49] SpareBit17

#### SYS_EHID20

* [8] Trap SMC
* [15] Force Nonspeculation If Oldest Redir Valid And Older
* [16] Force Nonspeculation If Spec Flush Pointer != Blk Rtr Pointer
* [22:21] Force Nonspeculation Targeted Timer

#### SYS_HID21

* [19] Enable LDREX Fill Reply
* [33] LDQ RTR Wait For Old ST Rel Cmpl
* [34] Disable Cdp Reply Purged Trans

### ACC/CYC Registers

These seem to relate to the core complex and power management configuration

#### SYS_ACC_OVRD

* [14:13] OK To Power Down SRM (3=deepsleep)
* [16:15] Disable L2 Flush For ACC Sleep (2=deepsleep)
* [18:17] OK To Train Down Link (3=deepsleep)
* [26:25] OK To Power Down CPM (2=deny 3=deepsleep)
* [28:27] CPM Wakeup (3=force)
* [29] Disable Clock Dtr
* [32] Disable PIO On WFI CPU
* [34] Enable Deep Sleep

#### SYS_ACC_CFG

Branch predictor state retention across ACC sleep

* [3:2] BP Sleep (2=BDP, 3=BTP)

#### SYS_CYC_OVRD

* [0] Disable WFI Return
* [25:24] OK To Power Down (2=force up, 3=force down)
* [21:20] FIQ mode (2=disable)
* [23:22] IRQ mode (2=disable)

### Memory subsystem registers

Mainly error control?

#### SYS_LSU_ERR_STS

* [54] L1 DTLB Multi Hit Enable

#### SYS_LSU_ERR_CTL

* [3] L1 DTLB Multi Hit Enable

#### SYS_L2C_ERR_STS

L2 subsystem fault control and info. This register is cluster-level and shared among all cores within a cluster.

* [1] Recursive fault (fault occurred while another fault was pending)
* [7] Access fault (unmapped physical address, etc)
* [38..34] Enable flags? (all 1 on entry from iBoot)
* [39] Enable SError interrupts (asynchronous errors)
* [43..40] Enable flags? (all 1 on entry from iBoot)
* [56] Enable write-1-to-clear behavior for fault flags
* [60] Some enable? (1 on entry)

#### SYS_L2C_ERR_ADR

Fault address for L2 subsystem fault.

* [?:0] Physical address of the fault
* [57:56] Set to '11'? Perhaps EL mode or other state info?
* [62..61] Core within cluster that caused fault

#### SYS_L2C_ERR_INF

L2 subsystem error information.

### CTRR Registers

Configurable Text Read-only Region

#### SYS_CTRR_CTL_EL1

* [0] A MMU off write protect
* [1] A MMU on write protect
* [2] B MMU off write protect
* [3] B MMU on write protect
* [4] A PXN
* [5] B PXN
* [6] A UXN
* [7] B UXN

### APRR Registers

#### SYS_APRR_EL0 / SYS_APRR_EL1

This is a table. The value is a 4-bit field:

* [0] X
* [1] W
* [2] R

The index is the access protection and execution protection settings for a PTE.

* [0] XN
* [1] PXN
* [2] AP[0]
* [3] AP[1]

The register value is 16 4-bit fields, in natural order ((_rwx) << (4*prot)).

### IPI registers

These are used for "fast" IPIs not using AIC

#### SYS_IPI_RR_LOCAL

* [3:0] Target CPU
* [29:28] RR Type (0=immediate, 1=retract, 2=deferred, 3=nowake)

#### SYS_IPI_RR_GLOBAL

* [3:0] Target CPU
* [20:16] Target cluster
* [29:28] RR Type (0=immediate, 1=retract, 2=deferred, 3=nowake)

#### SYS_IPI_CR

Global register.

* [15:0] Deferred IPI countdown value (in REFCLK ticks)

#### SYS_IPI_SR

Status register

* [0] IPI pending (write 1 to clear)

Needs a barrier (ISB SY) after clearing to avoid races with IPI handling.

### Virtual Memory System Architecture Lock

#### SYS_VMSA_LOCK

* [0] Lock VBAR
* [1] Lock SCTLR
* [2] Lock TCR
* [3] Lock TTBR0
* [4] Lock TTBR1
* [63] Lock SCTLR M bit

This is used to lock down writes to some Arm registers for security reasons at boot time.

### Pointer Authentication related registers

#### SYS_APCTL_EL1

* [0] Apple Mode
* [1] Kernel Key enable
* [2] AP Key 0 Enable
* [3] AP Key 1 Enable
* [4] User Key Enable

#### SYS_APSTS_EL1

* [0] M Key Valid

### General config registers

#### ACTLR_EL1 (ARM standard-not-standard)

* [1] Enable TSO
* [3] Disable HWP
* [4] Enable APFLG
* [5] Enable AFP
* [6] Enable PRSV
* [12] IC IVAU Enable ASID

### ID registers

#### MIDR_EL1 (ARM standard)

* [15:4] PartNum
  * 2: Fiji (A8 / H7P)
  * 3: Capri (A8X / H7G)
  * 4: Maui (A9 / H8P)
  * 5: Elba (A9X / H8G)
  * 6: Cayman (A10 / H9P)
  * 7: Myst (A10X / H9G)
  * 8: Skye Monsoon (A11 / H10 p-core)
  * 9: Skye Mistral (A11 / H10 e-core)
  * 11: Cyprus Vortex (A12 / H11P p-core)
  * 12: Cyprus Tempest (A12 / H11P e-core)
  * 15: M9 (S4/S5)
  * 16: Aruba Vortex (A12X/Z / H11G p-core)
  * 17: Aruba Tempest (A12X/Z / H11G e-core)
  * 18: Cebu Lightning (A13 / H12 p-core)
  * 19: Cebu Thunder (A13 / H12 e-core)
  * 34: M1 Icestorm (H13G e-core)
  * 35: M1 Firestorm (H13G p-core)
  * 38: Turks (S6 / M10)

* [31:24] Implementer (0x61 = 'a' = Apple)

#### MPIDR_EL1 (ARM standard)

* [23:16] Aff2: 0: e-core, 1:p-core
* [15:8] Aff1: Cluster ID
* [7:0] Aff0: CPU ID

#### AIDR_EL1 (ARM standard-not-standard)

* [0] MUL53
* [1] WKDM
* [2] ARCHRETENTION


### Unknown registers

#### s3_6_c15_c1_0 / s3_6_c15_c1_5 / s3_6_c15_c1_6

These look like a newer version of APRR

#### s3_4_c15_c5_0

Thisn gets written with the core ID (within the cluster) during init.

#### AHCR_EL2

Encoding unknown. Related to ACTLR_EL1[12].

