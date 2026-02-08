# Package Information

```
Alice Networks EVO Cloud
Note: This is free service for Developer

SLC.Evo.Standard Package:

4 vCPU AMD EPYC 9654 Genoa
8 GB RAM DDR4
120 GB NVMe SSD Storage
Unlimited @ 5 Gbps
KVM Virtualization
Salt Lake City, USA

https://app.alice.ws/ephemera/console
```

# Table of Content

- [Package Information](#package-information)
- [Table of Content](#table-of-content)
  - [CPU Info](#cpu-info)
  - [YABS Benchmark](#yabs-benchmark)
  - [Bench.Monster Benchmark](#benchmonster-benchmark)
  - [Bench.sh Benchmark](#benchsh-benchmark)
  - [CPU Steal](#cpu-steal)

## CPU Info

```bash
root@Ryzumi:~# lscpu
Architecture:            x86_64
  CPU op-mode(s):        32-bit, 64-bit
  Address sizes:         40 bits physical, 57 bits virtual
  Byte Order:            Little Endian
CPU(s):                  4
  On-line CPU(s) list:   0-3
Vendor ID:               AuthenticAMD
  BIOS Vendor ID:        QEMU
  Model name:            AMD EPYC-Milan Processor
    BIOS Model name:     pc-q35-7.2  CPU @ 2.0GHz
    BIOS CPU family:     1
    CPU family:          25
    Model:               1
    Thread(s) per core:  1
    Core(s) per socket:  1
    Socket(s):           4
    Stepping:            1
    BogoMIPS:            4799.99
    Flags:               fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush mmx fxsr sse sse2 syscall nx mmxext fxsr_opt pdpe1gb rdtscp lm rep_good nopl cpuid extd_ap
                         icid tsc_known_freq pni pclmulqdq ssse3 fma cx16 pcid sse4_1 sse4_2 x2apic movbe popcnt tsc_deadline_timer aes xsave avx f16c rdrand hypervisor lahf_lm cmp_legacy svm cr8
                         _legacy abm sse4a misalignsse 3dnowprefetch osvw topoext perfctr_core invpcid_single ssbd ibrs ibpb stibp vmmcall fsgsbase tsc_adjust bmi1 avx2 smep bmi2 erms invpcid avx
                         512f avx512dq rdseed adx smap avx512ifma clflushopt clwb avx512cd sha_ni avx512bw avx512vl xsaveopt xsavec xgetbv1 xsaves avx512_bf16 clzero xsaveerptr wbnoinvd arat npt
                         lbrv nrip_save tsc_scale vmcb_clean pausefilter pfthreshold v_vmsave_vmload vgif avx512vbmi umip pku ospke avx512_vbmi2 gfni vaes vpclmulqdq avx512_vnni avx512_bitalg avx
                         512_vpopcntdq la57 rdpid fsrm arch_capabilities
Virtualization features:
  Virtualization:        AMD-V
  Hypervisor vendor:     KVM
  Virtualization type:   full
Caches (sum of all):
  L1d:                   128 KiB (4 instances)
  L1i:                   128 KiB (4 instances)
  L2:                    2 MiB (4 instances)
  L3:                    128 MiB (4 instances)
NUMA:
  NUMA node(s):          1
  NUMA node0 CPU(s):     0-3
Vulnerabilities:
  Itlb multihit:         Not affected
  L1tf:                  Not affected
  Mds:                   Not affected
  Meltdown:              Not affected
  Mmio stale data:       Not affected
  Retbleed:              Not affected
  Spec store bypass:     Mitigation; Speculative Store Bypass disabled via prctl
  Spectre v1:            Mitigation; usercopy/swapgs barriers and __user pointer sanitization
  Spectre v2:            Mitigation; Retpolines, IBPB conditional, IBRS_FW, STIBP disabled, RSB filling, PBRSB-eIBRS Not affected
  Srbds:                 Not affected
  Tsx async abort:       Not affected
```

## YABS Benchmark

```bash
root@Ryzumi:~# curl -sL https://yabs.sh | bash
# ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## #
#              Yet-Another-Bench-Script              #
#                     v2025-04-20                    #
# https://github.com/masonr/yet-another-bench-script #
# ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## #

Tue Sep  9 01:57:21 PM BST 2025

Basic System Information:
---------------------------------
Uptime     : 0 days, 0 hours, 4 minutes
Processor  : AMD EPYC-Milan Processor
CPU cores  : 4 @ 2399.998 MHz
AES-NI     : ✔ Enabled
VM-x/AMD-V : ✔ Enabled
RAM        : 7.7 GiB
Swap       : 0.0 KiB
Disk       : 119.9 GiB
Distro     : Debian GNU/Linux 12 (bookworm)
Kernel     : 6.1.0-9-amd64
VM Type    : KVM
IPv4/IPv6  : ✔ Online / ❌ Offline

IPv4 Network Information:
---------------------------------
ISP        : Alice Networks LTD
ASN        : AS215355 Alice Network
Host       : Alice Networks Ltd
Location   : Los Angeles, California (CA)
Country    : United States

fio Disk Speed Tests (Mixed R/W 50/50) (Partition /dev/vda3):
---------------------------------
Block Size | 4k            (IOPS) | 64k           (IOPS)
  ------   | ---            ----  | ----           ----
Read       | 156.76 MB/s  (39.1k) | 468.24 MB/s   (7.3k)
Write      | 157.17 MB/s  (39.2k) | 470.70 MB/s   (7.3k)
Total      | 313.94 MB/s  (78.4k) | 938.95 MB/s  (14.6k)
           |                      |
Block Size | 512k          (IOPS) | 1m            (IOPS)
  ------   | ---            ----  | ----           ----
Read       | 447.11 MB/s    (873) | 441.21 MB/s    (430)
Write      | 470.87 MB/s    (919) | 470.59 MB/s    (459)
Total      | 917.99 MB/s   (1.7k) | 911.80 MB/s    (889)

iperf3 Network Speed Tests (IPv4):
---------------------------------
Provider        | Location (Link)           | Send Speed      | Recv Speed      | Ping
-----           | -----                     | ----            | ----            | ----
Clouvider       | London, UK (10G)          | 505 Mbits/sec   | 849 Mbits/sec   | --
Eranium         | Amsterdam, NL (100G)      | 513 Mbits/sec   | 946 Mbits/sec   | --
Uztelecom       | Tashkent, UZ (10G)        | 484 Mbits/sec   | 242 Mbits/sec   | --
Leaseweb        | Singapore, SG (10G)       | 451 Mbits/sec   | 419 Mbits/sec   | --
Clouvider       | Los Angeles, CA, US (10G) | 554 Mbits/sec   | 1.59 Gbits/sec  | --
Leaseweb        | NYC, NY, US (10G)         | 526 Mbits/sec   | 1.33 Gbits/sec  | --
Edgoo           | Sao Paulo, BR (1G)        | 492 Mbits/sec   | 481 Mbits/sec   | --

Geekbench 6 Benchmark Test:
---------------------------------
Test            | Value
                |
Single Core     | 2068
Multi Core      | 6662
Full Test       | https://browser.geekbench.com/v6/cpu/13725863

YABS completed in 9 min 32 sec
```

## Bench.Monster Benchmark

```bash
root@Ryzumi:~# curl -sL bench.monster | bash
---------------------------------------------------------------------------
 Region: Global  https://bench.monster v1.7.4 2023-12-15
 Usage : curl -sL bench.monster | bash -s -- -Global
---------------------------------------------------------------------------
 OS           : Debian GNU/Linux 12 (64 Bit)
 Virt/Kernel  : KVM / 6.1.0-39-amd64
 CPU Model    : AMD EPYC-Milan Processor
 CPU Cores    : 4 @ 2399.998 MHz x86_64 512 KB Cache
 CPU Flags    : AES-NI Enabled & VM-x/AMD-V Enabled
 Load Average : 0.00, 0.04, 0.02
 Total Space  : 120G (3.2G ~3% used)
 Total RAM    : 7904 MB (400 MB + 114 MB Buff in use)
 Total SWAP   : 0 MB (0 MB in use)
 IPv4/IPv6    : ✔ Online / ❌ Offline
 Uptime       : 0 days 0:7
---------------------------------------------------------------------------
 Location     : United States, Los Angeles (California)
 ASN & ISP    : AS215355, Alice Networks LTD / Alice Networks Ltd
---------------------------------------------------------------------------

 ## Geekbench v6 CPU Benchmark:

  Single Core :   (POOR)
   Multi Core :

 ## IO Test

 CPU Speed:
    bzip2     : 162 MB/s
   sha256     : 332 MB/s
   md5sum     : 600 MB/s

 RAM Speed:
   Avg. write : 3140.3 MB/s
   Avg. read  : 6246.4 MB/s

 Disk Speed:
   1st run    : 435 MB/s
   2nd run    : 431 MB/s
   3rd run    : 429 MB/s
   -----------------------
   Average    : 431.7 MB/s

 ## Global Speedtest.net

 Location                       Upload           Download         Ping
---------------------------------------------------------------------------
 Nearby                         151.19 Mbit/s    360.32 Mbit/s   * 158.287 ms
---------------------------------------------------------------------------
 USA, New York (Starry)         176.23 Mbit/s    316.81 Mbit/s   67.086 ms
 USA, Chicago (Windstream)      9.65 Mbit/s      12.23 Mbit/s    ping error!
 USA, Houston (Comcast)         12.94 Mbit/s     31.18 Mbit/s    ping error!
 USA, Los Angeles (Windstream)  10.39 Mbit/s     40.96 Mbit/s    ping error!
 UK, London (toob Ltd)          150.27 Mbit/s    175.79 Mbit/s   115.533 ms
 Germany, Berlin (DNS:NET)      137.65 Mbit/s    149.83 Mbit/s   137.712 ms
 Spain, Madrid (MasMovil)       138.85 Mbit/s    133.59 Mbit/s   133.623 ms
 Italy, Rome (Unidata)          110.56 Mbit/s    14.92 Mbit/s    144.833 ms
 India, Mumbai (Tatasky)        2.84 Mbit/s      15.56 Mbit/s    267.640 ms
ping: co2dsvr03.speedtest.starhub.com: Name or service not known
 Japan, Tsukuba (SoftEther)     151.90 Mbit/s    36.45 Mbit/s    115.712 ms
---------------------------------------------------------------------------

 Finished in : 15 min 13 sec
 Timestamp   : 2025-09-09 13:36:56 GMT
 Saved in    : /root/speedtest.log

 Share results:
 - https://www.speedtest.net/result/18202404663.png
 - https://browser.geekbench.com/v6/cpu/13726102
```

## Bench.sh Benchmark

```bash
-------------------- A Bench.sh Script By Teddysun -------------------
 Version            : v2025-05-08
 Usage              : wget -qO- bench.sh | bash
----------------------------------------------------------------------
 CPU Model          : AMD EPYC-Milan Processor
 CPU Cores          : 4 @ 2399.998 MHz
 CPU Cache          : 512 KB
 AES-NI             : ✓ Enabled
 VM-x/AMD-V         : ✓ Enabled
 Total Disk         : 119.9 GB (3.2 GB Used)
 Total Mem          : 7.7 GB (384.3 MB Used)
 System uptime      : 0 days, 0 hour 0 min
 Load average       : 0.30, 0.11, 0.04
 OS                 : Debian GNU/Linux 12
 Arch               : x86_64 (64 Bit)
 Kernel             : 6.1.0-39-amd64
 TCP CC             : bbr
 Virtualization     : KVM
 IPv4/IPv6          : ✓ Online / ✗ Offline
 Organization       : AS215355 Alice Network
 Location           : Los Angeles / US
 Region             : California
----------------------------------------------------------------------
 I/O Speed(1st run) : 425 MB/s
 I/O Speed(2nd run) : 430 MB/s
 I/O Speed(3rd run) : 428 MB/s
 I/O Speed(average) : 427.7 MB/s
----------------------------------------------------------------------
 Node Name        Upload Speed      Download Speed      Latency
 Speedtest.net    513.87 Mbps       1293.80 Mbps        14.07 ms
 Paris, FR        520.84 Mbps       2065.39 Mbps        134.77 ms
 Amsterdam, NL    547.15 Mbps       792.22 Mbps         142.12 ms
 Hong Kong, CN    536.86 Mbps       1162.06 Mbps        169.40 ms
 Singapore, SG    66.61 Mbps        428.55 Mbps         186.41 ms
----------------------------------------------------------------------
 Finished in        : 3 min 17 sec
 Timestamp          : 2025-09-09 14:17:55 BST
----------------------------------------------------------------------
```

## CPU Steal

```bash
root@Ryzumi:~# mpstat 30 5
Linux 6.1.0-39-amd64 (Ryzumi.alice.ws)  09/09/2025      _x86_64_        (4 CPU)

02:18:27 PM  CPU    %usr   %nice    %sys %iowait    %irq   %soft  %steal  %guest  %gnice   %idle
02:18:57 PM  all    0.13    0.00    0.37    0.00    0.00    0.08    0.00    0.00    0.00   99.42
02:19:27 PM  all    0.08    0.00    0.31    0.01    0.00    0.03    0.01    0.00    0.00   99.57
02:19:57 PM  all    0.10    0.00    0.34    0.02    0.00    0.04    0.00    0.00    0.00   99.50
02:20:27 PM  all    0.10    0.00    0.35    0.00    0.00    0.03    0.00    0.00    0.00   99.52
02:20:57 PM  all    0.08    0.00    0.31    0.00    0.00    0.04    0.00    0.00    0.00   99.57
Average:     all    0.10    0.00    0.34    0.01    0.00    0.05    0.00    0.00    0.00   99.51
root@Ryzumi:~#

```