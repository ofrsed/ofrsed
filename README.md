 $ ls /dev/input/
by-id    event0  event2  event4  event6  event8  mice    mouse1
by-path  event1  event3  event5  event7  event9  mouse0
root1@raspberrypi:~ $ sudo dmesg
[sudo] password for root1: 
[    0.000000] Booting Linux on physical CPU 0x0000000000 [0x410fd083]
[    0.000000] Linux version 6.12.47+rpt-rpi-v8 (serge@raspberrypi.com) (aarch64-linux-gnu-gcc-14 (Debian 14.2.0-19) 14.2.0, GNU ld (GNU Binutils for Debian) 2.44) #1 SMP PREEMPT Debian 1:6.12.47-1+rpt1 (2025-09-16)
[    0.000000] KASLR enabled
[    0.000000] random: crng init done
[    0.000000] Machine model: Raspberry Pi 4 Model B Rev 1.5
[    0.000000] efi: UEFI not found.
[    0.000000] Reserved memory: created CMA memory pool at 0x000000000dc00000, size 512 MiB
[    0.000000] OF: reserved mem: initialized node linux,cma, compatible id shared-dma-pool
[    0.000000] OF: reserved mem: 0x000000000dc00000..0x000000002dbfffff (524288 KiB) map reusable linux,cma
[    0.000000] OF: reserved mem: 0x000000003ef73340..0x000000003ef73375 (0 KiB) nomap non-reusable nvram@0
[    0.000000] OF: reserved mem: 0x000000003ef73100..0x000000003ef732ff (0 KiB) nomap non-reusable nvram@1
[    0.000000] NUMA: Faking a node at [mem 0x0000000000000000-0x000000007fffffff]
[    0.000000] Faking node 0 at [mem 0x0000000000000000-0x000000007fffffff] (2048MB)
[    0.000000] NUMA: Initialized distance table, cnt=1
[    0.000000] NODE_DATA(0) allocated [mem 0x7fbdb300-0x7fbddfff]
[    0.000000] Zone ranges:
[    0.000000]   DMA      [mem 0x0000000000000000-0x000000003fffffff]
[    0.000000]   DMA32    [mem 0x0000000040000000-0x000000007fffffff]
[    0.000000]   Normal   empty
[    0.000000] Movable zone start for each node
[    0.000000] Early memory node ranges
[    0.000000]   node   0: [mem 0x0000000000000000-0x000000003b3fffff]
[    0.000000]   node   0: [mem 0x0000000040000000-0x000000007fffffff]
[    0.000000] Initmem setup node 0 [mem 0x0000000000000000-0x000000007fffffff]
[    0.000000] On node 0, zone DMA32: 19456 pages in unavailable ranges
[    0.000000] percpu: Embedded 33 pages/cpu s95256 r8192 d31720 u135168
[    0.000000] pcpu-alloc: s95256 r8192 d31720 u135168 alloc=33*4096
[    0.000000] pcpu-alloc: [0] 0 [0] 1 [0] 2 [0] 3 
[    0.000000] Detected PIPT I-cache on CPU0
[    0.000000] CPU features: detected: Spectre-v2
[    0.000000] CPU features: detected: Spectre-v3a
[    0.000000] CPU features: detected: Spectre-v4
[    0.000000] CPU features: detected: Spectre-BHB
[    0.000000] CPU features: kernel page table isolation forced ON by KASLR
[    0.000000] CPU features: detected: Kernel page table isolation (KPTI)
[    0.000000] CPU features: detected: ARM erratum 1742098
[    0.000000] CPU features: detected: ARM errata 1165522, 1319367, or 1530923
[    0.000000] alternatives: applying boot alternatives
[    0.000000] Kernel command line: coherent_pool=1M 8250.nr_uarts=1 snd_bcm2835.enable_headphones=0 cgroup_disable=memory numa_policy=interleave nvme.max_host_mem_size_mb=0 snd_bcm2835.enable_headphones=1 snd_bcm2835.enable_hdmi=1 snd_bcm2835.enable_hdmi=0  numa=fake=1 system_heap.max_order=0 smsc95xx.macaddr=2C:CF:67:F3:4C:03 vc_mem.mem_base=0x3ec00000 vc_mem.mem_size=0x40000000  console=tty1 console=ttyS0,115200 root=PARTUUID=10ec7e24-02 rootfstype=ext4 fsck.repair=yes rootwait cfg80211.ieee80211_regdom=GB
[    0.000000] cgroup: Disabling memory control group subsystem
[    0.000000] mempolicy: NUMA default policy overridden to 'interleave:0'
[    0.000000] Dentry cache hash table entries: 262144 (order: 9, 2097152 bytes, linear)
[    0.000000] Inode-cache hash table entries: 131072 (order: 8, 1048576 bytes, linear)
[    0.000000] Fallback order for Node 0: 0 
[    0.000000] Built 1 zonelists, mobility grouping on.  Total pages: 504832
[    0.000000] Policy zone: DMA32
[    0.000000] mem auto-init: stack:all(zero), heap alloc:off, heap free:off
[    0.000000] software IO TLB: area num 4.
[    0.000000] software IO TLB: mapped [mem 0x0000000037400000-0x000000003b400000] (64MB)
[    0.000000] SLUB: HWalign=64, Order=0-3, MinObjects=0, CPUs=4, Nodes=1
[    0.000000] ftrace: allocating 45279 entries in 177 pages
[    0.000000] ftrace: allocated 177 pages with 4 groups
[    0.000000] rcu: Preemptible hierarchical RCU implementation.
[    0.000000] rcu: 	RCU event tracing is enabled.
[    0.000000] 	Trampoline variant of Tasks RCU enabled.
[    0.000000] 	Rude variant of Tasks RCU enabled.
[    0.000000] 	Tracing variant of Tasks RCU enabled.
[    0.000000] rcu: RCU calculated value of scheduler-enlistment delay is 25 jiffies.
[    0.000000] RCU Tasks: Setting shift to 2 and lim to 1 rcu_task_cb_adjust=1 rcu_task_cpu_ids=4.
[    0.000000] RCU Tasks Rude: Setting shift to 2 and lim to 1 rcu_task_cb_adjust=1 rcu_task_cpu_ids=4.
[    0.000000] RCU Tasks Trace: Setting shift to 2 and lim to 1 rcu_task_cb_adjust=1 rcu_task_cpu_ids=4.
[    0.000000] NR_IRQS: 64, nr_irqs: 64, preallocated irqs: 0
[    0.000000] Root IRQ handler: gic_handle_irq
[    0.000000] GIC: Using split EOI/Deactivate mode
[    0.000000] rcu: srcu_init: Setting srcu_struct sizes based on contention.
[    0.000000] arch_timer: cp15 timer(s) running at 54.00MHz (phys).
[    0.000000] clocksource: arch_sys_counter: mask: 0xffffffffffffff max_cycles: 0xc743ce346, max_idle_ns: 440795203123 ns
[    0.000000] sched_clock: 56 bits at 54MHz, resolution 18ns, wraps every 4398046511102ns
[    0.000153] Console: colour dummy device 80x25
[    0.000162] printk: legacy console [tty1] enabled
[    0.000436] Calibrating delay loop (skipped), value calculated using timer frequency.. 108.00 BogoMIPS (lpj=216000)
[    0.000450] pid_max: default: 32768 minimum: 301
[    0.000483] LSM: initializing lsm=capability
[    0.000590] Mount-cache hash table entries: 4096 (order: 3, 32768 bytes, linear)
[    0.000612] Mountpoint-cache hash table entries: 4096 (order: 3, 32768 bytes, linear)
[    0.001934] rcu: Hierarchical SRCU implementation.
[    0.001951] rcu: 	Max phase no-delay instances is 1000.
[    0.002090] Timer migration: 1 hierarchy levels; 8 children per group; 1 crossnode level
[    0.002716] EFI services will not be available.
[    0.002891] smp: Bringing up secondary CPUs ...
[    0.003212] Detected PIPT I-cache on CPU1
[    0.003279] CPU1: Booted secondary processor 0x0000000001 [0x410fd083]
[    0.003614] Detected PIPT I-cache on CPU2
[    0.003648] CPU2: Booted secondary processor 0x0000000002 [0x410fd083]
[    0.003995] Detected PIPT I-cache on CPU3
[    0.004031] CPU3: Booted secondary processor 0x0000000003 [0x410fd083]
[    0.004075] smp: Brought up 1 node, 4 CPUs
[    0.004107] SMP: Total of 4 processors activated.
[    0.004112] CPU: All CPU(s) started at EL2
[    0.004127] CPU features: detected: 32-bit EL0 Support
[    0.004132] CPU features: detected: 32-bit EL1 Support
[    0.004139] CPU features: detected: CRC32 instructions
[    0.004173] alternatives: applying system-wide alternatives
[    0.005038] Memory: 1340268K/2019328K available (14336K kernel code, 2406K rwdata, 4824K rodata, 2048K init, 577K bss, 149372K reserved, 524288K cma-reserved)
[    0.005370] devtmpfs: initialized
[    0.009468] Enabled cp15_barrier support
[    0.009505] Enabled setend support
[    0.009590] clocksource: jiffies: mask: 0xffffffff max_cycles: 0xffffffff, max_idle_ns: 7645041785100000 ns
[    0.009608] futex hash table entries: 1024 (order: 4, 65536 bytes, linear)
[    0.018259] 2G module region forced by RANDOMIZE_MODULE_REGION_FULL
[    0.018296] 0 pages in range for non-PLT usage
[    0.018298] 518176 pages in range for PLT usage
[    0.018455] pinctrl core: initialized pinctrl subsystem
[    0.018794] DMI not present or invalid.
[    0.020329] NET: Registered PF_NETLINK/PF_ROUTE protocol family
[    0.020967] DMA: preallocated 1024 KiB GFP_KERNEL pool for atomic allocations
[    0.021060] DMA: preallocated 1024 KiB GFP_KERNEL|GFP_DMA pool for atomic allocations
[    0.021211] DMA: preallocated 1024 KiB GFP_KERNEL|GFP_DMA32 pool for atomic allocations
[    0.021244] audit: initializing netlink subsys (disabled)
[    0.021388] audit: type=2000 audit(0.020:1): state=initialized audit_enabled=0 res=1
[    0.021621] thermal_sys: Registered thermal governor 'step_wise'
[    0.021642] cpuidle: using governor menu
[    0.021742] hw-breakpoint: found 6 breakpoint and 4 watchpoint registers.
[    0.021797] ASID allocator initialised with 32768 entries
[    0.022219] Serial: AMBA PL011 UART driver
[    0.024873] /soc/interrupt-controller@40041000: Fixed dependency cycle(s) with /soc/interrupt-controller@40041000
[    0.025282] bcm2835-mbox fe00b880.mailbox: mailbox enabled
[    0.032091] raspberrypi-firmware soc:firmware: Attached to firmware from 2025-08-20T17:02:31, variant start
[    0.036097] raspberrypi-firmware soc:firmware: Firmware hash is cd866525580337c0aee4b25880e1f5f9f674fb24
[    0.041446] /scb/pcie@7d500000: Fixed dependency cycle(s) with /scb/pcie@7d500000
[    0.041547] /scb/pcie@7d500000: Fixed dependency cycle(s) with /scb/pcie@7d500000
[    0.044460] bcm2835-dma fe007000.dma-controller: DMA legacy API manager, dmachans=0x1
[    0.045151] iommu: Default domain type: Translated
[    0.045161] iommu: DMA domain TLB invalidation policy: strict mode
[    0.045778] SCSI subsystem initialized
[    0.045867] usbcore: registered new interface driver usbfs
[    0.045887] usbcore: registered new interface driver hub
[    0.045907] usbcore: registered new device driver usb
[    0.046088] pps_core: LinuxPPS API ver. 1 registered
[    0.046095] pps_core: Software ver. 5.3.6 - Copyright 2005-2007 Rodolfo Giometti <giometti@linux.it>
[    0.046107] PTP clock support registered
[    0.046696] vgaarb: loaded
[    0.046943] clocksource: Switched to clocksource arch_sys_counter
[    0.405987] VFS: Disk quotas dquot_6.6.0
[    0.406036] VFS: Dquot-cache hash table entries: 512 (order 0, 4096 bytes)
[    0.408992] NET: Registered PF_INET protocol family
[    0.409174] IP idents hash table entries: 32768 (order: 6, 262144 bytes, linear)
[    0.410282] tcp_listen_portaddr_hash hash table entries: 1024 (order: 2, 16384 bytes, linear)
[    0.410318] Table-perturb hash table entries: 65536 (order: 6, 262144 bytes, linear)
[    0.410331] TCP established hash table entries: 16384 (order: 5, 131072 bytes, linear)
[    0.410392] TCP bind hash table entries: 16384 (order: 7, 524288 bytes, linear)
[    0.410898] TCP: Hash tables configured (established 16384 bind 16384)
[    0.411094] MPTCP token hash table entries: 2048 (order: 3, 49152 bytes, linear)
[    0.411171] UDP hash table entries: 1024 (order: 3, 32768 bytes, linear)
[    0.411194] UDP-Lite hash table entries: 1024 (order: 3, 32768 bytes, linear)
[    0.411285] NET: Registered PF_UNIX/PF_LOCAL protocol family
[    0.411640] RPC: Registered named UNIX socket transport module.
[    0.411650] RPC: Registered udp transport module.
[    0.411656] RPC: Registered tcp transport module.
[    0.411661] RPC: Registered tcp-with-tls transport module.
[    0.411666] RPC: Registered tcp NFSv4.1 backchannel transport module.
[    0.411679] PCI: CLS 0 bytes, default 64
[    0.411990] Trying to unpack rootfs image as initramfs...
[    0.421844] kvm [1]: nv: 554 coarse grained trap handlers
[    0.422120] kvm [1]: IPA Size Limit: 44 bits
[    0.422777] kvm [1]: vgic interrupt IRQ9
[    0.422820] kvm [1]: Hyp nVHE mode initialized successfully
[    0.423879] Initialise system trusted keyrings
[    0.424163] workingset: timestamp_bits=42 max_order=19 bucket_order=0
[    0.424655] NFS: Registering the id_resolver key type
[    0.424690] Key type id_resolver registered
[    0.424696] Key type id_legacy registered
[    0.424709] nfs4filelayout_init: NFSv4 File Layout Driver Registering...
[    0.424717] nfs4flexfilelayout_init: NFSv4 Flexfile Layout Driver Registering...
[    0.425138] Key type asymmetric registered
[    0.425162] Asymmetric key parser 'x509' registered
[    0.425203] Block layer SCSI generic (bsg) driver version 0.4 loaded (major 247)
[    0.425375] io scheduler mq-deadline registered
[    0.425390] io scheduler kyber registered
[    0.425416] io scheduler bfq registered
[    0.425956] irq_brcmstb_l2: registered L2 intc (/soc/interrupt-controller@7ef00100, parent irq: 23)
[    0.427848] pinctrl-bcm2835 fe200000.gpio: GPIO_OUT persistence: yes
[    0.735274] Freeing initrd memory: 17924K
[    0.738831] ledtrig-cpu: registered to indicate activity on CPUs
[    0.740401] brcm-pcie fd500000.pcie: host bridge /scb/pcie@7d500000 ranges:
[    0.740487] brcm-pcie fd500000.pcie:   No bus range found for /scb/pcie@7d500000, using [bus 00-ff]
[    0.740521] brcm-pcie fd500000.pcie:      MEM 0x0600000000..0x063fffffff -> 0x00c0000000
[    0.740545] brcm-pcie fd500000.pcie:   IB MEM 0x0000000000..0x007fffffff -> 0x0400000000
[    0.741897] brcm-pcie fd500000.pcie: PCI host bridge to bus 0000:00
[    0.741962] pci_bus 0000:00: root bus resource [bus 00-ff]
[    0.741976] pci_bus 0000:00: root bus resource [mem 0x600000000-0x63fffffff] (bus address [0xc0000000-0xffffffff])
[    0.742078] pci 0000:00:00.0: [14e4:2711] type 01 class 0x060400 PCIe Root Port
[    0.742104] pci 0000:00:00.0: PCI bridge to [bus 00]
[    0.742117] pci 0000:00:00.0:   bridge window [mem 0x80000000-0xbfffffff]
[    0.742189] pci 0000:00:00.0: PME# supported from D0 D3hot
[    0.744099] pci 0000:00:00.0: bridge configuration invalid ([bus 00-00]), reconfiguring
[    0.744242] pci_bus 0000:01: supply vpcie3v3 not found, using dummy regulator
[    0.744313] pci_bus 0000:01: supply vpcie3v3aux not found, using dummy regulator
[    0.744340] pci_bus 0000:01: supply vpcie12v not found, using dummy regulator
[    0.846958] brcm-pcie fd500000.pcie: clkreq-mode set to default
[    0.849033] brcm-pcie fd500000.pcie: link up, 5.0 GT/s PCIe x1 (SSC)
[    0.849166] pci 0000:01:00.0: [1106:3483] type 00 class 0x0c0330 PCIe Endpoint
[    0.849222] pci 0000:01:00.0: BAR 0 [mem 0x00000000-0x00000fff 64bit]
[    0.849316] pci 0000:01:00.0: ASPM: VL805 fixup applied
[    0.849402] pci 0000:01:00.0: PME# supported from D0 D3hot
[    0.854999] pci_bus 0000:01: busn_res: [bus 01-ff] end is updated to 01
[    0.855022] pci 0000:00:00.0: bridge window [mem 0x600000000-0x6000fffff]: assigned
[    0.855033] pci 0000:01:00.0: BAR 0 [mem 0x600000000-0x600000fff 64bit]: assigned
[    0.855078] pci 0000:00:00.0: PCI bridge to [bus 01]
[    0.855086] pci 0000:00:00.0:   bridge window [mem 0x600000000-0x6000fffff]
[    0.855096] pci_bus 0000:00: resource 4 [mem 0x600000000-0x63fffffff]
[    0.855104] pci_bus 0000:01: resource 1 [mem 0x600000000-0x6000fffff]
[    0.855238] pcieport 0000:00:00.0: enabling device (0000 -> 0002)
[    0.855308] pcieport 0000:00:00.0: PME: Signaling with IRQ 27
[    0.855490] pcieport 0000:00:00.0: AER: enabled with IRQ 27
[    0.855888] simple-framebuffer 3e99a000.framebuffer: framebuffer at 0x3e99a000, 0x260000 bytes
[    0.855900] simple-framebuffer 3e99a000.framebuffer: format=a8r8g8b8, mode=1024x600x32, linelength=4096
[    0.857030] Console: switching to colour frame buffer device 128x37
[    0.857920] simple-framebuffer 3e99a000.framebuffer: fb0: simplefb registered!
[    0.861459] Serial: 8250/16550 driver, 1 ports, IRQ sharing enabled
[    0.862353] iproc-rng200 fe104000.rng: hwrng registered
[    0.862461] vc-mem: phys_addr:0x00000000 mem_base=0x3ec00000 mem_size:0x40000000(1024 MiB)
[    0.866641] brd: module loaded
[    0.869101] loop: module loaded
[    0.869476] Loading iSCSI transport class v2.0-870.
[    0.871951] bcmgenet fd580000.ethernet: GENET 5.0 EPHY: 0x0000
[    1.078975] unimac-mdio unimac-mdio.-19: Broadcom UniMAC MDIO bus
[    1.080069] usbcore: registered new interface driver lan78xx
[    1.080624] usbcore: registered new interface driver smsc95xx
[    1.173158] xhci_hcd 0000:01:00.0: xHCI Host Controller
[    1.173693] xhci_hcd 0000:01:00.0: new USB bus registered, assigned bus number 1
[    1.175060] xhci_hcd 0000:01:00.0: hcc params 0x002841eb hci version 0x100 quirks 0x0300240000000890
[    1.176063] xhci_hcd 0000:01:00.0: xHCI Host Controller
[    1.176598] xhci_hcd 0000:01:00.0: new USB bus registered, assigned bus number 2
[    1.177133] xhci_hcd 0000:01:00.0: Host supports USB 3.0 SuperSpeed
[    1.177768] usb usb1: New USB device found, idVendor=1d6b, idProduct=0002, bcdDevice= 6.12
[    1.178303] usb usb1: New USB device strings: Mfr=3, Product=2, SerialNumber=1
[    1.178833] usb usb1: Product: xHCI Host Controller
[    1.179379] usb usb1: Manufacturer: Linux 6.12.47+rpt-rpi-v8 xhci-hcd
[    1.179917] usb usb1: SerialNumber: 0000:01:00.0
[    1.180707] hub 1-0:1.0: USB hub found
[    1.181294] hub 1-0:1.0: 1 port detected
[    1.182127] usb usb2: New USB device found, idVendor=1d6b, idProduct=0003, bcdDevice= 6.12
[    1.182695] usb usb2: New USB device strings: Mfr=3, Product=2, SerialNumber=1
[    1.183270] usb usb2: Product: xHCI Host Controller
[    1.183837] usb usb2: Manufacturer: Linux 6.12.47+rpt-rpi-v8 xhci-hcd
[    1.184401] usb usb2: SerialNumber: 0000:01:00.0
[    1.185129] hub 2-0:1.0: USB hub found
[    1.185731] hub 2-0:1.0: 4 ports detected
[    1.186712] dwc_otg: version 3.00a 10-AUG-2012 (platform bus)
[    1.187318] dwc_otg: FIQ enabled
[    1.187321] dwc_otg: NAK holdoff enabled
[    1.187324] dwc_otg: FIQ split-transaction FSM enabled
[    1.187328] Module dwc_common_port init
[    1.187831] usbcore: registered new interface driver uas
[    1.188403] usbcore: registered new interface driver usb-storage
[    1.189128] mousedev: PS/2 mouse device common for all mice
[    1.191125] sdhci: Secure Digital Host Controller Interface driver
[    1.191665] sdhci: Copyright(c) Pierre Ossman
[    1.192274] sdhci-pltfm: SDHCI platform and OF driver helper
[    1.193036] hid: raw HID events driver (C) Jiri Kosina
[    1.193630] usbcore: registered new interface driver usbhid
[    1.194167] usbhid: USB HID core driver
[    1.197452] hw perfevents: enabled with armv8_cortex_a72 PMU driver, 7 (0,8000003f) counters available
[    1.198668] NET: Registered PF_PACKET protocol family
[    1.199374] Key type dns_resolver registered
[    1.209639] registered taskstats version 1
[    1.210369] Loading compiled-in X.509 certificates
[    1.214467] Demotion targets for Node 0: null
[    1.215555] Key type .fscrypt registered
[    1.216116] Key type fscrypt-provisioning registered
[    1.220073] uart-pl011 fe201000.serial: there is not valid maps for state default
[    1.220908] uart-pl011 fe201000.serial: cts_event_workaround enabled
[    1.221640] fe201000.serial: ttyAMA1 at MMIO 0xfe201000 (irq = 39, base_baud = 0) is a PL011 rev3
[    1.222313] serial serial0: tty port ttyAMA1 registered
[    1.223574] bcm2835-aux-uart fe215040.serial: there is not valid maps for state default
[    1.224545] printk: legacy console [ttyS0] disabled
[    1.225377] fe215040.serial: ttyS0 at MMIO 0xfe215040 (irq = 40, base_baud = 62500000) is a 16550
[    1.226025] printk: legacy console [ttyS0] enabled
[    2.875242] bcm2835-wdt bcm2835-wdt: Broadcom BCM2835 watchdog timer
[    2.882710] bcm2835-power bcm2835-power: Broadcom BCM2835 power domains driver
[    2.891159] mmc-bcm2835 fe300000.mmcnr: mmc_debug:0 mmc_debug2:0
[    2.897853] mmc-bcm2835 fe300000.mmcnr: DMA channel allocated
[    2.927086] of_cfs_init
[    2.930324] of_cfs_init: OK
[    2.934140] clk: Disabling unused clocks
[    2.938918] PM: genpd: Disabling unused power domains
[    2.971528] mmc0: SDHCI controller on fe340000.mmc [fe340000.mmc] using ADMA
[    2.982115] Freeing unused kernel memory: 2048K
[    2.987454] Run /init as init process
[    2.991203] usb 1-1: new high-speed USB device number 2 using xhci_hcd
[    2.991746]   with arguments:
[    2.991748]     /init
[    2.998979]   with environment:
[    2.998982]     HOME=/
[    2.998984]     TERM=linux
[    3.013699] mmc1: new high speed SDIO card at address 0001
[    3.028201] mmc0: new high speed SDXC card at address b368
[    3.035049] mmcblk0: mmc0:b368 NCard 58.2 GiB
[    3.042696]  mmcblk0: p1 p2
[    3.046875] mmcblk0: mmc0:b368 NCard 58.2 GiB
[    3.137655] usb 1-1: New USB device found, idVendor=2109, idProduct=3431, bcdDevice= 4.21
[    3.146648] usb 1-1: New USB device strings: Mfr=0, Product=1, SerialNumber=0
[    3.154492] usb 1-1: Product: USB2.0 Hub
[    3.160612] hub 1-1:1.0: USB hub found
[    3.165324] hub 1-1:1.0: 4 ports detected
[    3.325072] v3d fec00000.v3d: [drm] Transparent Hugepage support is recommended for optimal performance on this platform!
[    3.341608] [drm] Initialized v3d 1.0.0 for fec00000.v3d on minor 0
[    3.366446] Console: switching to colour dummy device 80x25
[    3.414962] vc4-drm gpu: bound fe400000.hvs (ops vc4_hvs_ops [vc4])
[    3.454961] usb 1-1.2: new full-speed USB device number 3 using xhci_hcd
[    3.559467] usb 1-1.2: New USB device found, idVendor=5566, idProduct=0008, bcdDevice= 1.00
[    3.567964] usb 1-1.2: New USB device strings: Mfr=1, Product=2, SerialNumber=3
[    3.575388] usb 1-1.2: Product: PANTEON T2 PRO RS
[    3.580160] usb 1-1.2: Manufacturer: RGBMicroChip
[    3.584931] usb 1-1.2: SerialNumber: 2022-12-12
[    3.601090] input: RGBMicroChip PANTEON T2 PRO RS Keyboard as /devices/platform/scb/fd500000.pcie/pci0000:00/0000:00:00.0/0000:01:00.0/usb1/1-1/1-1.2/1-1.2:1.0/0003:5566:0008.0001/input/input0
[    3.787117] input: RGBMicroChip PANTEON T2 PRO RS Mouse as /devices/platform/scb/fd500000.pcie/pci0000:00/0000:00:00.0/0000:01:00.0/usb1/1-1/1-1.2/1-1.2:1.0/0003:5566:0008.0001/input/input2
[    3.804413] input: RGBMicroChip PANTEON T2 PRO RS Wireless Radio Control as /devices/platform/scb/fd500000.pcie/pci0000:00/0000:00:00.0/0000:01:00.0/usb1/1-1/1-1.2/1-1.2:1.0/0003:5566:0008.0001/input/input3
[    3.823211] hid-generic 0003:5566:0008.0001: input,hiddev96,hidraw0: USB HID v1.10 Keyboard [RGBMicroChip PANTEON T2 PRO RS] on usb-0000:01:00.0-1.2/input0
[    3.838706] vc4-drm gpu: bound fe400000.hvs (ops vc4_hvs_ops [vc4])
[    3.851101] vc4-drm gpu: bound fe400000.hvs (ops vc4_hvs_ops [vc4])
[    3.851164] input: RGBMicroChip PANTEON T2 PRO RS as /devices/platform/scb/fd500000.pcie/pci0000:00/0000:00:00.0/0000:01:00.0/usb1/1-1/1-1.2/1-1.2:1.1/0003:5566:0008.0002/input/input4
[    4.003239] hid-generic 0003:5566:0008.0002: input,hidraw1: USB HID v1.10 Keyboard [RGBMicroChip PANTEON T2 PRO RS] on usb-0000:01:00.0-1.2/input1
[    4.017815] vc4-drm gpu: bound fe400000.hvs (ops vc4_hvs_ops [vc4])
[    4.027503] input: RGBMicroChip PANTEON T2 PRO RS as /devices/platform/scb/fd500000.pcie/pci0000:00/0000:00:00.0/0000:01:00.0/usb1/1-1/1-1.2/1-1.2:1.2/0003:5566:0008.0003/input/input5
[    4.044285] hid-generic 0003:5566:0008.0003: input,hidraw2: USB HID v1.10 Device [RGBMicroChip PANTEON T2 PRO RS] on usb-0000:01:00.0-1.2/input2
[    4.058734] vc4-drm gpu: bound fe400000.hvs (ops vc4_hvs_ops [vc4])
[    5.935159] EXT4-fs (mmcblk0p2): orphan cleanup on readonly fs
[    5.942829] EXT4-fs (mmcblk0p2): mounted filesystem 37d2cb52-513e-40e1-b90f-213aa6096cba ro with ordered data mode. Quota mode: none.
[    6.917116] systemd[1]: System time advanced to timestamp on /var/lib/systemd/timesync/clock: Sat 2025-10-25 18:22:03 BST
[    7.113199] NET: Registered PF_INET6 protocol family
[    7.118932] Segment Routing with IPv6
[    7.122688] In-situ OAM (IOAM) with IPv6
[    7.269360] systemd[1]: systemd 257.8-1~deb13u2 running in system mode (+PAM +AUDIT +SELINUX +APPARMOR +IMA +IPE +SMACK +SECCOMP +GCRYPT -GNUTLS +OPENSSL +ACL +BLKID +CURL +ELFUTILS +FIDO2 +IDN2 -IDN +IPTC +KMOD +LIBCRYPTSETUP +LIBCRYPTSETUP_PLUGINS +LIBFDISK +PCRE2 +PWQUALITY +P11KIT +QRENCODE +TPM2 +BZIP2 +LZ4 +XZ +ZLIB +ZSTD +BPF_FRAMEWORK +BTF -XKBCOMMON -UTMP +SYSVINIT +LIBARCHIVE)
[    7.304176] systemd[1]: Detected architecture arm64.
[    7.341048] systemd[1]: Hostname set to <raspberrypi>.
[    7.595118] systemd[1]: bpf-restrict-fs: BPF LSM hook not enabled in the kernel, BPF LSM not supported.
[    7.604955] systemd[1]: Using hardware watchdog 'Broadcom BCM2835 Watchdog timer', version 0, device /dev/watchdog0
[    7.615610] systemd[1]: Watchdog running with a hardware timeout of 1min.
[    8.071093] zram_generator::config[220]: zram0: system has too much memory (1845MB), limit is 0MB, ignoring.
[   10.254111] systemd[1]: Queued start job for default target graphical.target.
[   10.312938] systemd[1]: Created slice system-getty.slice - Slice /system/getty.
[   10.321312] systemd[1]: Created slice system-modprobe.slice - Slice /system/modprobe.
[   10.330076] systemd[1]: Created slice system-rpi\x2dsetup\x2dloop.slice - Slice /system/rpi-setup-loop.
[   10.341009] systemd[1]: Created slice system-serial\x2dgetty.slice - Slice /system/serial-getty.
[   10.351418] systemd[1]: Created slice system-systemd\x2dfsck.slice - Slice /system/systemd-fsck.
[   10.361611] systemd[1]: Created slice system-systemd\x2dzram\x2dsetup.slice - Slice /system/systemd-zram-setup.
[   10.372972] systemd[1]: Created slice user.slice - User and Session Slice.
[   10.380427] systemd[1]: Started systemd-ask-password-wall.path - Forward Password Requests to Wall Directory Watch.
[   10.391928] systemd[1]: Set up automount proc-sys-fs-binfmt_misc.automount - Arbitrary Executable File Formats File System Automount Point.
[   10.405050] systemd[1]: Expecting device dev-disk-by\x2dpartuuid-10ec7e24\x2d01.device - /dev/disk/by-partuuid/10ec7e24-01...
[   10.417122] systemd[1]: Expecting device dev-dri-card0.device - /dev/dri/card0...
[   10.425420] systemd[1]: Expecting device dev-dri-renderD128.device - /dev/dri/renderD128...
[   10.434574] systemd[1]: Expecting device dev-ttyS0.device - /dev/ttyS0...
[   10.442163] systemd[1]: Expecting device dev-zram0.device - /dev/zram0...
[   10.449820] systemd[1]: Reached target nss-user-lookup.target - User and Group Name Lookups.
[   10.459072] systemd[1]: Reached target slices.target - Slice Units.
[   10.497716] systemd[1]: Listening on rpcbind.socket - RPCbind Server Activation Socket.
[   10.510499] systemd[1]: Listening on systemd-creds.socket - Credential Encryption/Decryption.
[   10.519725] systemd[1]: Listening on systemd-initctl.socket - initctl Compatibility Named Pipe.
[   10.529208] systemd[1]: Listening on systemd-journald-dev-log.socket - Journal Socket (/dev/log).
[   10.538972] systemd[1]: Listening on systemd-journald.socket - Journal Sockets.
[   10.546886] systemd[1]: systemd-pcrextend.socket - TPM PCR Measurements was skipped because of an unmet condition check (ConditionSecurity=measured-uki).
[   10.561443] systemd[1]: systemd-pcrlock.socket - Make TPM PCR Policy was skipped because of an unmet condition check (ConditionSecurity=measured-uki).
[   10.575989] systemd[1]: Listening on systemd-udevd-control.socket - udev Control Socket.
[   10.584872] systemd[1]: Listening on systemd-udevd-kernel.socket - udev Kernel Socket.
[   10.593703] systemd[1]: dev-hugepages.mount - Huge Pages File System was skipped because of an unmet condition check (ConditionPathExists=/sys/kernel/mm/hugepages).
[   10.612595] systemd[1]: Mounting dev-mqueue.mount - POSIX Message Queue File System...
[   10.623666] systemd[1]: Mounting run-lock.mount - Legacy Locks Directory /run/lock...
[   10.634190] systemd[1]: Mounting sys-kernel-debug.mount - Kernel Debug File System...
[   10.655501] systemd[1]: Mounting sys-kernel-tracing.mount - Kernel Trace File System...
[   10.664763] systemd[1]: auth-rpcgss-module.service - Kernel Module supporting RPCSEC_GSS was skipped because of an unmet condition check (ConditionPathExists=/etc/krb5.keytab).
[   10.683400] systemd[1]: Starting keyboard-setup.service - Set the console keyboard layout...
[   10.695246] systemd[1]: Starting kmod-static-nodes.service - Create List of Static Device Nodes...
[   10.707791] systemd[1]: Starting modprobe@configfs.service - Load Kernel Module configfs...
[   10.719947] systemd[1]: Starting modprobe@drm.service - Load Kernel Module drm...
[   10.731397] systemd[1]: Starting modprobe@efi_pstore.service - Load Kernel Module efi_pstore...
[   10.746226] systemd[1]: Starting modprobe@fuse.service - Load Kernel Module fuse...
[   10.755494] systemd[1]: systemd-fsck-root.service - File System Check on Root Device was skipped because of an unmet condition check (ConditionPathExists=!/run/initramfs/fsck-root).
[   10.772506] systemd[1]: systemd-hibernate-clear.service - Clear Stale Hibernate Storage Info was skipped because of an unmet condition check (ConditionPathExists=/sys/firmware/efi/efivars/HibernateLocation-8cf2644b-4b0b-428f-9387-6d876050dc67).
[   10.796851] fuse: init (API version 7.41)
[   10.797350] systemd[1]: Starting systemd-journald.service - Journal Service...
[   10.814862] systemd[1]: Starting systemd-modules-load.service - Load Kernel Modules...
[   10.823924] systemd[1]: systemd-pcrmachine.service - TPM PCR Machine ID Measurement was skipped because of an unmet condition check (ConditionSecurity=measured-uki).
[   10.841610] systemd[1]: Starting systemd-remount-fs.service - Remount Root and Kernel File Systems...
[   10.851850] systemd[1]: systemd-tpm2-setup-early.service - Early TPM SRK Setup was skipped because of an unmet condition check (ConditionSecurity=measured-uki).
[   10.869195] systemd[1]: Starting systemd-udev-load-credentials.service - Load udev Rules from Credentials...
[   10.882727] systemd[1]: Starting systemd-udev-trigger.service - Coldplug All udev Devices...
[   10.914875] zram: Added device: zram0
[   10.918859] systemd[1]: Mounted dev-mqueue.mount - POSIX Message Queue File System.
[   10.932517] systemd[1]: Mounted run-lock.mount - Legacy Locks Directory /run/lock.
[   10.941466] systemd[1]: Mounted sys-kernel-debug.mount - Kernel Debug File System.
[   10.950327] systemd[1]: Mounted sys-kernel-tracing.mount - Kernel Trace File System.
[   10.959546] systemd[1]: Finished kmod-static-nodes.service - Create List of Static Device Nodes.
[   10.971949] systemd[1]: modprobe@configfs.service: Deactivated successfully.
[   10.980251] systemd[1]: Finished modprobe@configfs.service - Load Kernel Module configfs.
[   10.990304] systemd[1]: Finished keyboard-setup.service - Set the console keyboard layout.
[   10.999892] systemd[1]: modprobe@drm.service: Deactivated successfully.
[   11.007621] systemd[1]: Finished modprobe@drm.service - Load Kernel Module drm.
[   11.015546] EXT4-fs (mmcblk0p2): re-mounted 37d2cb52-513e-40e1-b90f-213aa6096cba r/w.
[   11.016214] systemd[1]: modprobe@efi_pstore.service: Deactivated successfully.
[   11.032578] systemd[1]: Finished modprobe@efi_pstore.service - Load Kernel Module efi_pstore.
[   11.036510] systemd-journald[305]: Collecting audit messages is disabled.
[   11.049200] i2c_dev: i2c /dev entries driver
[   11.051368] systemd[1]: modprobe@fuse.service: Deactivated successfully.
[   11.063127] systemd[1]: Finished modprobe@fuse.service - Load Kernel Module fuse.
[   11.072165] systemd[1]: Finished systemd-modules-load.service - Load Kernel Modules.
[   11.086897] systemd[1]: Finished systemd-remount-fs.service - Remount Root and Kernel File Systems.
[   11.097399] systemd[1]: Started systemd-journald.service - Journal Service.
[   11.249637] systemd-journald[305]: Received client request to flush runtime journal.
[   12.200975] loop0: detected capacity change from 0 to 3778560
[   13.106173] zram: setup backing device /dev/disk/by-backingfile/var-swap
[   13.124024] zram0: detected capacity change from 0 to 3778560
[   13.459372] rpi-gpiomem fe200000.gpiomem: window base 0xfe200000 size 0x00001000
[   13.459600] rpi-gpiomem fe200000.gpiomem: initialised 1 regions as /dev/gpiomem
[   13.460912] vc4-drm gpu: bound fe400000.hvs (ops vc4_hvs_ops [vc4])
[   13.466518] vc4-drm gpu: bound fe400000.hvs (ops vc4_hvs_ops [vc4])
[   13.502674] Adding 1889276k swap on /dev/zram0.  Priority:100 extents:1 across:1889276k SS
[   13.517462] vc4-drm gpu: bound fe400000.hvs (ops vc4_hvs_ops [vc4])
[   13.524832] vc4-drm gpu: bound fe400000.hvs (ops vc4_hvs_ops [vc4])
[   13.565029] snd_bcm2835: module is from the staging directory, the quality is unknown, you have been warned.
[   13.566700] bcm2835-audio bcm2835-audio: card created with 8 channels
[   13.567933] vc4-drm gpu: bound fe400000.hvs (ops vc4_hvs_ops [vc4])
[   13.647432] brcmstb-i2c fef04500.i2c:  @97500hz registered in polling mode
[   13.648754] vc4-drm gpu: bound fe400000.hvs (ops vc4_hvs_ops [vc4])
[   13.650371] Registered IR keymap rc-cec
[   13.650453] rc rc0: vc4-hdmi-0 as /devices/platform/soc/fef00700.hdmi/rc/rc0
[   13.650537] input: vc4-hdmi-0 as /devices/platform/soc/fef00700.hdmi/rc/rc0/input6
[   13.650619] brcmstb-i2c fef09500.i2c:  @97500hz registered in polling mode
[   13.654776] input: vc4-hdmi-0 HDMI Jack as /devices/platform/soc/fef00700.hdmi/sound/card1/input7
[   13.658354] vc4-drm gpu: bound fef00700.hdmi (ops vc4_hdmi_ops [vc4])
[   13.659503] Registered IR keymap rc-cec
[   13.659598] rc rc1: vc4-hdmi-1 as /devices/platform/soc/fef05700.hdmi/rc/rc1
[   13.659694] input: vc4-hdmi-1 as /devices/platform/soc/fef05700.hdmi/rc/rc1/input8
[   13.662983] input: vc4-hdmi-1 HDMI Jack as /devices/platform/soc/fef05700.hdmi/sound/card2/input9
[   13.663267] vc4-drm gpu: bound fef05700.hdmi (ops vc4_hdmi_ops [vc4])
[   13.663568] vc4-drm gpu: bound fe004000.txp (ops vc4_txp_ops [vc4])
[   13.663742] vc4-drm gpu: bound fe206000.pixelvalve (ops vc4_crtc_ops [vc4])
[   13.663880] vc4-drm gpu: bound fe207000.pixelvalve (ops vc4_crtc_ops [vc4])
[   13.664028] vc4-drm gpu: bound fe20a000.pixelvalve (ops vc4_crtc_ops [vc4])
[   13.664105] vc4-drm gpu: bound fe216000.pixelvalve (ops vc4_crtc_ops [vc4])
[   13.664210] vc4-drm gpu: bound fec12000.pixelvalve (ops vc4_crtc_ops [vc4])
[   13.666549] [drm] Initialized vc4 0.0.0 for gpu on minor 1
[   13.682692] mc: Linux media interface: v0.10
[   13.739774] Console: switching to colour frame buffer device 128x37
[   13.761516] vc4-drm gpu: [drm] fb0: vc4drmfb frame buffer device
[   13.824147] videodev: Linux video capture interface: v2.00
[   13.966290] Bluetooth: Core ver 2.22
[   13.966379] NET: Registered PF_BLUETOOTH protocol family
[   13.966385] Bluetooth: HCI device and connection manager initialized
[   13.966402] Bluetooth: HCI socket layer initialized
[   13.966410] Bluetooth: L2CAP socket layer initialized
[   13.966422] Bluetooth: SCO socket layer initialized
[   14.012756] vc_sm_cma: module is from the staging directory, the quality is unknown, you have been warned.
[   14.013383] bcm2835_vc_sm_cma_probe: Videocore shared memory driver
[   14.013395] [vc_sm_connected_init]: start
[   14.022679] [vc_sm_connected_init]: installed successfully
[   14.030796] bcm2835_mmal_vchiq: module is from the staging directory, the quality is unknown, you have been warned.
[   14.053606] Bluetooth: HCI UART driver ver 2.3
[   14.053627] Bluetooth: HCI UART protocol H4 registered
[   14.053678] Bluetooth: HCI UART protocol Three-wire (H5) registered
[   14.053837] Bluetooth: HCI UART protocol Broadcom registered
[   14.055289] hci_uart_bcm serial0-0: supply vbat not found, using dummy regulator
[   14.055413] hci_uart_bcm serial0-0: supply vddio not found, using dummy regulator
[   14.056906] bcm2835_isp: module is from the staging directory, the quality is unknown, you have been warned.
[   14.066218] bcm2835-isp bcm2835-isp: Device node output[0] registered as /dev/video13
[   14.066539] bcm2835-isp bcm2835-isp: Device node capture[0] registered as /dev/video14
[   14.066771] bcm2835-isp bcm2835-isp: Device node capture[1] registered as /dev/video15
[   14.066969] bcm2835-isp bcm2835-isp: Device node stats[2] registered as /dev/video16
[   14.067014] bcm2835-isp bcm2835-isp: Register output node 0 with media controller
[   14.067025] bcm2835-isp bcm2835-isp: Register capture node 1 with media controller
[   14.067030] bcm2835-isp bcm2835-isp: Register capture node 2 with media controller
[   14.067035] bcm2835-isp bcm2835-isp: Register capture node 3 with media controller
[   14.068360] bcm2835_codec: module is from the staging directory, the quality is unknown, you have been warned.
[   14.073011] bcm2835-isp bcm2835-isp: Device node output[0] registered as /dev/video20
[   14.073293] bcm2835-isp bcm2835-isp: Device node capture[0] registered as /dev/video21
[   14.073550] bcm2835-isp bcm2835-isp: Device node capture[1] registered as /dev/video22
[   14.073710] bcm2835-isp bcm2835-isp: Device node stats[2] registered as /dev/video23
[   14.073724] bcm2835-isp bcm2835-isp: Register output node 0 with media controller
[   14.073733] bcm2835-isp bcm2835-isp: Register capture node 1 with media controller
[   14.073739] bcm2835-isp bcm2835-isp: Register capture node 2 with media controller
[   14.073744] bcm2835-isp bcm2835-isp: Register capture node 3 with media controller
[   14.073840] bcm2835-isp bcm2835-isp: Loaded V4L2 bcm2835-isp
[   14.078818] bcm2835_v4l2: module is from the staging directory, the quality is unknown, you have been warned.
[   14.083234] bcm2835-codec bcm2835-codec: Device registered as /dev/video10
[   14.083275] bcm2835-codec bcm2835-codec: Loaded V4L2 decode
[   14.091781] bcm2835-codec bcm2835-codec: Device registered as /dev/video11
[   14.091813] bcm2835-codec bcm2835-codec: Loaded V4L2 encode
[   14.102870] bcm2835-codec bcm2835-codec: Device registered as /dev/video12
[   14.102899] bcm2835-codec bcm2835-codec: Loaded V4L2 isp
[   14.105574] bcm2835-codec bcm2835-codec: Device registered as /dev/video18
[   14.105612] bcm2835-codec bcm2835-codec: Loaded V4L2 image_fx
[   14.109731] bcm2835-codec bcm2835-codec: Device registered as /dev/video31
[   14.109764] bcm2835-codec bcm2835-codec: Loaded V4L2 encode_image
[   14.115783] cfg80211: Loading compiled-in X.509 certificates for regulatory database
[   14.116467] rpi-hevc-dec feb00000.codec: Device registered as /dev/video19
[   14.131660] Loaded X.509 cert 'benh@debian.org: 577e021cb980e0e820821ba7b54b4961b8b4fadf'
[   14.131979] Loaded X.509 cert 'romain.perier@gmail.com: 3abbc6ec146e09d1b6016ab9d6cf71dd233f0328'
[   14.132268] Loaded X.509 cert 'sforshee: 00b28ddf47aef9cea7'
[   14.132559] Loaded X.509 cert 'wens: 61c038651aabdcf94bd0ac7ff06c7248db18c600'
[   14.417437] Bluetooth: hci0: BCM: chip id 107
[   14.417685] Bluetooth: hci0: BCM: features 0x2f
[   14.418994] Bluetooth: hci0: BCM4345C0
[   14.419014] Bluetooth: hci0: BCM4345C0 (003.001.025) build 0000
[   14.451345] brcmfmac: F1 signature read @0x18000000=0x15264345
[   14.454889] brcmfmac: brcmf_fw_alloc_request: using brcm/brcmfmac43455-sdio for chip BCM4345/6
[   14.455395] usbcore: registered new interface driver brcmfmac
[   14.523753] Bluetooth: hci0: BCM4345C0 'brcm/BCM4345C0.raspberrypi,4-model-b.hcd' Patch
[   14.717850] Goodix-TS 1-0014: supply AVDD28 not found, using dummy regulator
[   14.717970] Goodix-TS 1-0014: supply VDDIO not found, using dummy regulator
[   14.801369] brcmfmac: brcmf_c_process_txcap_blob: no txcap_blob available (err=-2)
[   14.801872] brcmfmac: brcmf_c_preinit_dcmds: Firmware: BCM4345/6 wl0: Aug 29 2023 01:47:08 version 7.45.265 (28bca26 CY) FWID 01-b677b91b
[   14.818766] Goodix-TS 1-0014: Error reading 1 bytes from 0x8140: -5
[   14.839286] Goodix-TS 1-0014: Error reading 1 bytes from 0x8140: -5
[   14.863057] Goodix-TS 1-0014: I2C communication failure: -5
[   14.863492] Goodix-TS 1-0014: probe with driver Goodix-TS failed with error -5
[   15.283684] Bluetooth: hci0: BCM: features 0x2f
[   15.284937] Bluetooth: hci0: BCM43455 37.4MHz Raspberry Pi 3+-0190
[   15.284943] Bluetooth: hci0: BCM4345C0 (003.001.025) build 0382
[   21.247768] Bluetooth: BNEP (Ethernet Emulation) ver 1.3
[   21.247789] Bluetooth: BNEP filters: protocol multicast
[   21.247801] Bluetooth: BNEP socket layer initialized
[   21.251379] Bluetooth: MGMT ver 1.23
[   21.275958] NET: Registered PF_ALG protocol family
[   21.964979] Bluetooth: RFCOMM TTY layer initialized
[   21.965007] Bluetooth: RFCOMM socket layer initialized
[   21.965026] Bluetooth: RFCOMM ver 1.11
[   27.588310] bcmgenet fd580000.ethernet: configuring instance for external RGMII (RX delay)
[   27.590131] bcmgenet fd580000.ethernet eth0: Link is Down
[   27.603288] brcmfmac: brcmf_cfg80211_set_power_mgmt: power save enabled
[   34.497510] ieee80211 phy0: brcmf_cfg80211_reg_notifier: Firmware rejected country setting
[   54.744207] input: M720 Triathlon Keyboard as /devices/virtual/misc/uhid/0005:046D:B015.0004/input/input10
[   54.744790] input: M720 Triathlon Mouse as /devices/virtual/misc/uhid/0005:046D:B015.0004/input/input11
[   54.745127] hid-generic 0005:046D:B015.0004: input,hidraw3: BLUETOOTH HID v0.13 Keyboard [M720 Triathlon] on 2c:cf:67:f3:4c:06
[   55.407270] input: Logitech M720 Triathlon Multi-Device Mouse as /devices/virtual/misc/uhid/0005:046D:B015.0004/input/input13
[   55.409397] logitech-hidpp-device 0005:046D:B015.0004: input,hidraw3: BLUETOOTH HID v0.13 Keyboard [Logitech M720 Triathlon Multi-Device Mouse] on 2c:cf:67:f3:4c:06
[   55.429459] logitech-hidpp-device 0005:046D:B015.0004: HID++ 4.5 device connected.
[  105.232261] warning: `ThreadPoolForeg' uses wireless extensions which will stop working for Wi-Fi 7 hardware; use nl80211
root1@raspberrypi:~ $ 


## Hi there 👋
<div id="header" align="center">
  <img src="https://github.com/ofrsed/ofrsed/blob/main/bongo-cat-typing.gif" width="100"/>
</div>


<div id="badges" align="center">
  <a href="https://t.me/ofrsed">
    <img src="https://img.shields.io/badge/Telegram-blue?style=for-the-badge&logo=telegram&logoColor=white" alt="LinkedIn Badge"/>
 
  </a>
</div>

## Intro

I started getting interested in programming while still working as an automation engineer. My acquaintance began with Arduino (C++), but then I got interested in Python. After some time, the company closed, and I decided to delve even deeper into IT. And this is, of course, complete madness 🧐. I spent almost a year looking for a job, surviving on Telegram bots, small sites and parsing :anguished: (Press F). Now I am putting my efforts into a cool company.

## Language and Tools
<div>
  <img src="https://github.com/devicons/devicon/blob/master/icons/python/python-original.svg" title="python" alt="python" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/pytest/pytest-original.svg" title="pytest" alt="pytest" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/php/php-original.svg" title="php" alt="php" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/lua/lua-original.svg" title="lua" alt="lua" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/django/django-plain.svg" title="django" alt="django" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/postman/postman-original.svg" title="postman" alt="postman" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/djangorest/djangorest-original.svg" title="djangorest" alt="djangorest" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/flask/flask-original.svg" title="flask" alt="flask" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/css3/css3-plain-wordmark.svg"  title="CSS3" alt="CSS" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/html5/html5-original.svg" title="HTML5" alt="HTML" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/mysql/mysql-original-wordmark.svg" title="MySQL"  alt="MySQL" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/git/git-original-wordmark.svg" title="Git" **alt="Git" width="40" height="40"/>
  <img src="https://github.com/devicons/devicon/blob/master/icons/gitlab/gitlab-original.svg" title="gitlab" **alt="gitlab" width="40" height="40"/>
  <img src="https://github.com/devicons/devicon/blob/master/icons/figma/figma-original.svg" title="figma" **alt="figma" width="40" height="40"/>
  <img src="https://github.com/devicons/devicon/blob/master/icons/pycharm/pycharm-original.svg" title="pycharm" **alt="pycharm" width="40" height="40"/>
</div>


## Certificates
<div>
<h1>
  <img src="https://github.com/ofrsed/ofrsed/blob/main/certificates/1-1.png" width="200px"/>
  <img src="https://github.com/ofrsed/ofrsed/blob/main/certificates/2-1.png" width="200px"/>
  <img src="https://github.com/ofrsed/ofrsed/blob/main/certificates/3-1.png" width="200px"/>
  <img src="https://github.com/ofrsed/ofrsed/blob/main/certificates/4-1.png" width="200px"/>
  <img src="https://github.com/ofrsed/ofrsed/blob/main/certificates/5-1.png" width="200px"/>
  <img src="https://github.com/ofrsed/ofrsed/blob/main/certificates/6-1.png" width="200px"/>
  <img src="https://github.com/ofrsed/ofrsed/blob/main/certificates/7-1.png" width="200px"/>
  <img src="https://github.com/ofrsed/ofrsed/blob/main/certificates/8-1.png" width="200px"/>
  <img src="https://github.com/ofrsed/ofrsed/blob/main/certificates/9-1.png" width="200px"/>
  <img src="https://github.com/ofrsed/ofrsed/blob/main/certificates/10-1.png" width="200px"/>
  <img src="https://github.com/ofrsed/ofrsed/blob/main/certificates/11-1.png" width="200px"/>
  <img src="https://github.com/ofrsed/ofrsed/blob/main/certificates/12-1.png" width="200px"/>
  <img src="https://github.com/ofrsed/ofrsed/blob/main/certificates/13-1.png" width="200px"/>
  <img src="https://github.com/ofrsed/ofrsed/blob/main/certificates/14-1.png" width="200px"/>


</h1>
</div>

## Notes / Road map

Programming language
  - [x] [Python](https://github.com/ofrsed/Notes/blob/main/Python/python_notes.md)
    - [x] [OOP](https://github.com/ofrsed/Notes/blob/main/Python/python_oop_notes.md)
    - [x] Frameworks
      - [x] [Asyncio](https://github.com/ofrsed/Notes/blob/main/Python/Frameworks/asyncio.md), [Multithreading](https://github.com/ofrsed/Notes/blob/main/Python/Frameworks/multithreading.md),  [Matplotlib](https://github.com/ofrsed/Notes/blob/main/Python/Frameworks/matplotlib.md), Aiogram, BeautifulSoup4, Selenium, Django, Flask
      - [ ] Pandas, NumPy
  - [ ] [C++](https://github.com/ofrsed/Notes/blob/main/%D0%A1/C%2B%2B.md)
  - [ ] [JS](https://github.com/ofrsed/Notes/blob/main/JavaScript/javascript_notes.md)
  - [x] PHP

- Databases and SQL
  - [x] [Neo4j](https://github.com/ofrsed/Notes/blob/main/neo4j/neo4j_notes.md)
  - [x] [SQL](https://github.com/ofrsed/Notes/blob/main/SQL/sql_notes.md)
  - [x] Redis
- Data structures and algorithms
  - [x] [Структуры данных](https://github.com/ofrsed/Notes/blob/main/data%20structures%20and%20algorithms/data%20structures.md) 
  - [x] [Grokking Algorithms](https://github.com/ofrsed/ofrsed/blob/main/Grokaem_algoritmy.pdf)
- VCS
  - [x] Git
- Communication as a Service
  - [x] [k8s](https://github.com/ofrsed/Notes/blob/main/communication_as_a_service/k8s.md)
  - [x] [Docker](https://github.com/ofrsed/Notes/blob/main/communication_as_a_service/docker.md)
  - [x] [Брокеры сообщений](https://github.com/ofrsed/Notes/blob/main/communication_as_a_service/message_broker.md)
- Operating System
  - [x] [Linux](https://github.com/ofrsed/Notes/blob/main/Linux/linux_notes.md)
  - [x] Windows 


## Tasks

- [ ] [🎥](https://www.youtube.com/watch?v=WlCDcr8JYFU) __Clean Architecture__ 5:57 6:03-7:10

<details>
  <summary>Запланированные задачи</summary>

- [ ] 📚 __Поколение Python: алгоритмы и структуры данных__ - курс выходит 1 апреля  
- [ ] [📚](https://stepik.org/course/193691/syllabus) __C/C++__
- [ ] [🎥](https://www.youtube.com/watch?v=eDuuKvIWzew&list=PLA0M1Bcd0w8zmegfAUfFMiACPKfdW4ifD) __NumPy__
- [ ] [🎥](https://www.youtube.com/watch?v=HemPVRvVm40&list=PLBP4Q3FNSLK2EujXiPUeTIOVnydZS8YJk) __Pandas__
- [ ] [🎥](https://www.youtube.com/watch?v=gA3A_epB3So&t=755s) __База по оптимизации PostgreSQL__
- [ ] 🌐 __K8S__
- [ ] 🌐 __модуль OS__
- [ ] 🌐 __Chrome DevTools__
- [ ] 🌐 __1C__
- [ ] 🌐 __Bitrix__
- [ ] 🌐 __Балансировщики нагрузки__
- [ ] 🌐 __sqlalchemy (доп.)__
- [ ] 🌐 __WSGI__
- [ ] 🌐 __TDD__
- [ ] 🌐 __профилирование__

sqlalchemy 
</details>
<details>
  <summary>Завершенные задачи</summary>

от 15.02
- [x] [📚](https://stepik.org/course/199114/syllabus) Брокеры сообщений. Apache Kafka
- [x] [🎥](https://www.youtube.com/watch?v=bcMZGPIeGzk) __Middleware in FastAPI__
- [x] [🎥](https://www.youtube.com/playlist?list=PLDyvV36pndZFHXjXuwA_NywNrVQO0aQqb) __GIT (пусть хранится тут)__
- [x] [🎥](https://www.youtube.com/watch?v=dKxiHlZvULQ) __Типизирование (пусть хранится тут)__

</details>

## Hot Keys

`DELETE FROM alembic_version;`

`alembic revision --autogenerate`

`alembic upgrade head`

`alembic stamp head`


## interview questions
[for interview](https://github.com/ofrsed/Notes/blob/main/interview_questions.md)

[Памятка PHP/GoLang разработчику](https://backendinterview.ru/os)

[math](https://github.com/ofrsed/Notes/blob/main/math.md)

[база #2](https://github.com/yakimka/python_interview_questions)




<!--
**ofrsed/ofrsed** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.


Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
