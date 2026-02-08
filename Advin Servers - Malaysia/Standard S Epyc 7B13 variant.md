# Package Information

```
Standard S:

8 vCPU AMD Epyc Milan 7003
16 GB RAM DDR4
128 GB NVMe SSD Storage
4 TB Transfer Data @ 10 Gbps
KVM Virtualization
Johor, MY

https://advinservers.com/cloud
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
root@ryzumi:~# lscpu
Architecture:             x86_64
  CPU op-mode(s):         32-bit, 64-bit
  Address sizes:          48 bits physical, 48 bits virtual
  Byte Order:             Little Endian
CPU(s):                   8
  On-line CPU(s) list:    0-7
Vendor ID:                AuthenticAMD
  BIOS Vendor ID:         QEMU
  Model name:             AMD EPYC 7B13 64-Core Processor
    BIOS Model name:      pc-i440fx-9.2  CPU @ 2.0GHz
    BIOS CPU family:      1
    CPU family:           25
    Model:                1
    Thread(s) per core:   1
    Core(s) per socket:   8
    Socket(s):            1
    Stepping:             1
    BogoMIPS:             4499.99
    Flags:                fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush mmx fxsr sse sse2 ht syscall nx mmxext fxsr_opt pdpe1gb rdtscp lm rep_good nopl cpuid ext
                          d_apicid tsc_known_freq pni pclmulqdq ssse3 fma cx16 pcid sse4_1 sse4_2 x2apic movbe popcnt tsc_deadline_timer aes xsave avx f16c rdrand hypervisor lahf_lm cmp_legacy sv
                          m cr8_legacy abm sse4a misalignsse 3dnowprefetch osvw perfctr_core invpcid_single ssbd ibrs ibpb stibp vmmcall fsgsbase tsc_adjust bmi1 avx2 smep bmi2 erms invpcid rdsee
                          d adx smap clflushopt clwb sha_ni xsaveopt xsavec xgetbv1 xsaves clzero xsaveerptr wbnoinvd arat npt lbrv nrip_save tsc_scale vmcb_clean flushbyasid pausefilter pfthresh
                          old v_vmsave_vmload vgif umip pku ospke vaes vpclmulqdq rdpid overflow_recov succor fsrm arch_capabilities
Virtualization features:
  Virtualization:         AMD-V
  Hypervisor vendor:      KVM
  Virtualization type:    full
Caches (sum of all):
  L1d:                    512 KiB (8 instances)
  L1i:                    512 KiB (8 instances)
  L2:                     4 MiB (8 instances)
  L3:                     128 MiB (8 instances)
NUMA:
  NUMA node(s):           1
  NUMA node0 CPU(s):      0-7
Vulnerabilities:
  Gather data sampling:   Not affected
  Itlb multihit:          Not affected
  L1tf:                   Not affected
  Mds:                    Not affected
  Meltdown:               Not affected
  Mmio stale data:        Not affected
  Reg file data sampling: Not affected
  Retbleed:               Not affected
  Spec rstack overflow:   Mitigation; safe RET
  Spec store bypass:      Mitigation; Speculative Store Bypass disabled via prctl
  Spectre v1:             Mitigation; usercopy/swapgs barriers and __user pointer sanitization
  Spectre v2:             Mitigation; Retpolines; IBPB conditional; IBRS_FW; STIBP disabled; RSB filling; PBRSB-eIBRS Not affected; BHI Not affected
  Srbds:                  Not affected
  Tsx async abort:        Not affected
```

## YABS Benchmark

```bash
root@ryzumi:~# curl -sL https://yabs.sh | bash
# ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## #
#              Yet-Another-Bench-Script              #
#                     v2025-04-20                    #
# https://github.com/masonr/yet-another-bench-script #
# ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## #

Mon Aug  4 03:33:08 PM UTC 2025

Basic System Information:
---------------------------------
Uptime     : 0 days, 0 hours, 4 minutes
Processor  : AMD EPYC 7B13 64-Core Processor
CPU cores  : 8 @ 2249.998 MHz
AES-NI     : ✔ Enabled
VM-x/AMD-V : ✔ Enabled
RAM        : 15.6 GiB
Swap       : 0.0 KiB
Disk       : 118.1 GiB
Distro     : Debian GNU/Linux 12 (bookworm)
Kernel     : 6.1.0-22-amd64
VM Type    : KVM
IPv4/IPv6  : ✔ Online / ✔ Online

IPv6 Network Information:
---------------------------------
ISP        : Advin Services LLC
ASN        : AS206216 Advin Services LLC
Host       : Advin Services LLC
Location   : Singapore, Central Singapore (01)
Country    : Singapore

fio Disk Speed Tests (Mixed R/W 50/50) (Partition /dev/sda3):
---------------------------------
| Block Size | 4k            (IOPS) | 64k           (IOPS) |
| ---------- | -------------------- | -------------------- |  |----
Read       | 142.02 MB/s  (35.5k) | 1.36 GB/s    (21.4k)
Write      | 142.39 MB/s  (35.5k) | 1.37 GB/s    (21.5k)
Total      | 284.41 MB/s  (71.1k) | 2.74 GB/s    (42.9k)
           |                      |
| Block Size | 512k          (IOPS) | 1m            (IOPS) |
| ---------- | -------------------- | -------------------- |  |----
Read       | 3.36 GB/s     (6.5k) | 3.75 GB/s     (3.6k)
Write      | 3.54 GB/s     (6.9k) | 4.00 GB/s     (3.9k)
Total      | 6.90 GB/s    (13.4k) | 7.75 GB/s     (7.5k)

iperf3 Network Speed Tests (IPv4):
---------------------------------
| Provider  | Location (Link)           | Send Speed     | Recv Speed     | Ping    |
| --------- | ------------------------- | -------------- | -------------- | ------- |
| Clouvider | London, UK (10G)          | 1.13 Gbits/sec | 1.28 Gbits/sec | 153 ms  |
| Eranium   | Amsterdam, NL (100G)      | 5.39 Gbits/sec | 5.41 Gbits/sec | 221 ms  |
| Uztelecom | Tashkent, UZ (10G)        | 6.38 Gbits/sec | 1.51 Gbits/sec | 190 ms  |
| Leaseweb  | Singapore, SG (10G)       | 8.89 Gbits/sec | 7.53 Gbits/sec | 2.17 ms |
| Clouvider | Los Angeles, CA, US (10G) | 1.03 Gbits/sec | 1.34 Gbits/sec | 166 ms  |
| Leaseweb  | NYC, NY, US (10G)         | 3.73 Gbits/sec | 3.67 Gbits/sec | 218 ms  |
| Edgoo     | Sao Paulo, BR (1G)        | 2.12 Gbits/sec | 1.53 Gbits/sec | 369 ms  |

iperf3 Network Speed Tests (IPv6):
---------------------------------
| Provider  | Location (Link)           | Send Speed     | Recv Speed     | Ping    |
| --------- | ------------------------- | -------------- | -------------- | ------- |
| Clouvider | London, UK (10G)          | 1.10 Gbits/sec | 1.36 Gbits/sec | 153 ms  |
| Eranium   | Amsterdam, NL (100G)      | 5.59 Gbits/sec | 4.33 Gbits/sec | 221 ms  |
| Uztelecom | Tashkent, UZ (10G)        | 4.97 Gbits/sec | busy           | 190 ms  |
| Leaseweb  | Singapore, SG (10G)       | 8.53 Gbits/sec | 6.64 Gbits/sec | 2.28 ms |
| Clouvider | Los Angeles, CA, US (10G) | 978 Mbits/sec  | 1.29 Gbits/sec | 166 ms  |
| Leaseweb  | NYC, NY, US (10G)         | 1.77 Gbits/sec | 2.55 Gbits/sec | 218 ms  |
| Edgoo     | Sao Paulo, BR (1G)        | busy           | 1.70 Gbits/sec | 369 ms  |

Geekbench 6 Benchmark Test:
---------------------------------
Test            | Value
                |
Single Core     | 1318
Multi Core      | 7012
Full Test       | https://browser.geekbench.com/v6/cpu/13170807

YABS completed in 15 min 1 sec
```

## Bench.Monster Benchmark

```bash
root@ryzumi:~# curl -sL bench.monster | bash
---------------------------------------------------------------------------
 Region: Global  https://bench.monster v1.7.4 2023-12-15
 Usage : curl -sL bench.monster | bash -s -- -Global
---------------------------------------------------------------------------
 OS           : Debian GNU/Linux 12 (64 Bit)
 Virt/Kernel  : KVM / 6.1.0-22-amd64
 CPU Model    : AMD EPYC 7B13 64-Core Processor
 CPU Cores    : 8 @ 2249.998 MHz x86_64 512 KB Cache
 CPU Flags    : AES-NI Enabled & VM-x/AMD-V Enabled
 Load Average : 0.02, 0.11, 0.19
 Total Space  : 119G (1.9G ~2% used)
 Total RAM    : 15991 MB (453 MB + 1367 MB Buff in use)
 Total SWAP   : 0 MB (0 MB in use)
 IPv4/IPv6    : ✔ Online / ✔ Online
 Uptime       : 0 days 0:32
---------------------------------------------------------------------------
 Location     : Singapore, Singapore (Central Singapore)
 ASN & ISP    : AS206216, Advin Services LLC / Advin Services LLC
---------------------------------------------------------------------------

 ## Geekbench v6 CPU Benchmark:

  Single Core : 1390  (EXCELLENT)
   Multi Core : 7158

 ## IO Test

 CPU Speed:
    bzip2     : 129 MB/s
   sha256     : 228 MB/s
   md5sum     : 509 MB/s

 RAM Speed:
   Avg. write : 2252.8 MB/s
   Avg. read  : 6348.8 MB/s

 Disk Speed:
   1st run    : 774 MB/s
   2nd run    : 792 MB/s
   3rd run    : 740 MB/s
   -----------------------
   Average    : 768.7 MB/s

 ## Global Speedtest.net

 Location                       Upload           Download         Ping
---------------------------------------------------------------------------
 Nearby                         150.61 Mbit/s    466.67 Mbit/s   * 162.941 ms
---------------------------------------------------------------------------
 USA, New York (Starry)         50.90 Mbit/s     146.93 Mbit/s   207.595 ms
 USA, Chicago (Windstream)      3.13 Mbit/s      29.50 Mbit/s    212.707 ms
 USA, Houston (Comcast)         22.97 Mbit/s     119.74 Mbit/s   200.671 ms
 USA, Los Angeles (Windstream)  4.91 Mbit/s      74.94 Mbit/s    164.630 ms
 UK, London (toob Ltd)          108.59 Mbit/s    155.68 Mbit/s   159.476 ms
 Germany, Berlin (DNS:NET)      34.80 Mbit/s     126.69 Mbit/s   160.038 ms
 Spain, Madrid (MasMovil)       115.53 Mbit/s    357.09 Mbit/s   148.804 ms
 Italy, Rome (Unidata)          100.47 Mbit/s    176.75 Mbit/s   166.700 ms
 India, Mumbai (Tatasky)        295.37 Mbit/s    309.05 Mbit/s   58.266 ms
ping: co2dsvr03.speedtest.starhub.com: Name or service not known
 Japan, Tsukuba (SoftEther)     238.39 Mbit/s    172.71 Mbit/s   71.415 ms
ping: s1.speedtest.syd.optusnet.com.au: Name or service not known
---------------------------------------------------------------------------

 Finished in : 19 min 9 sec
 Timestamp   : 2025-08-04 16:20:24 GMT
 Saved in    : /root/speedtest.log

 Share results:
 - https://www.speedtest.net/result/18060137134.png
 - https://browser.geekbench.com/v6/cpu/13171102
```

## Bench.sh Benchmark

```bash
-------------------- A Bench.sh Script By Teddysun -------------------
 Version            : v2025-05-08
 Usage              : wget -qO- bench.sh | bash
----------------------------------------------------------------------
 CPU Model          : AMD EPYC 7B13 64-Core Processor
 CPU Cores          : 8 @ 2249.998 MHz
 CPU Cache          : 512 KB
 AES-NI             : ✓ Enabled
 VM-x/AMD-V         : ✓ Enabled
 Total Disk         : 118.1 GB (1.9 GB Used)
 Total Mem          : 15.6 GB (454.5 MB Used)
 System uptime      : 0 days, 0 hour 23 min
 Load average       : 0.00, 0.31, 0.30
 OS                 : Debian GNU/Linux 12
 Arch               : x86_64 (64 Bit)
 Kernel             : 6.1.0-22-amd64
 TCP CC             : bbr
 Virtualization     : KVM
 IPv4/IPv6          : ✓ Online / ✓ Online
 Organization       : AS206216 Advin Services LLC
 Location           : Singapore / SG
 Region             : Singapore
----------------------------------------------------------------------
 I/O Speed(1st run) : 757 MB/s
 I/O Speed(2nd run) : 752 MB/s
 I/O Speed(3rd run) : 724 MB/s
 I/O Speed(average) : 744.3 MB/s
----------------------------------------------------------------------
 Node Name        Upload Speed      Download Speed      Latency
 Speedtest.net    7975.21 Mbps      6673.41 Mbps        1.66 ms
 Paris, FR        3303.45 Mbps      6646.96 Mbps        147.55 ms
 Amsterdam, NL    738.57 Mbps       2347.87 Mbps        153.69 ms
 Shanghai, CN     1084.98 Mbps      4061.53 Mbps        142.50 ms
 Hong Kong, CN    1967.65 Mbps      5177.47 Mbps        41.30 ms
 Tokyo, JP        459.45 Mbps       6180.02 Mbps        69.43 ms
----------------------------------------------------------------------
 Finished in        : 5 min 39 sec
 Timestamp          : 2025-08-04 15:58:26 UTC
----------------------------------------------------------------------
```

## CPU Steal

```bash
root@ryzumi:~# mpstat 30 5
Linux 6.1.0-22-amd64 (ryzumi)   08/04/2025      _x86_64_        (8 CPU)

03:49:40 PM  CPU    %usr   %nice    %sys %iowait    %irq   %soft  %steal  %guest  %gnice   %idle
03:50:10 PM  all    0.03    0.00    0.10    0.00    0.00    0.08    0.01    0.00    0.00   99.78
03:50:40 PM  all    0.03    0.00    0.07    0.00    0.00    0.05    0.00    0.00    0.00   99.85
03:51:10 PM  all    0.03    0.00    0.10    0.00    0.00    0.06    0.00    0.00    0.00   99.81
03:51:40 PM  all    0.02    0.00    0.10    0.00    0.00    0.07    0.01    0.00    0.00   99.80
03:52:10 PM  all    0.04    0.00    0.08    0.00    0.00    0.06    0.01    0.00    0.00   99.80
Average:     all    0.03    0.00    0.09    0.00    0.00    0.06    0.01    0.00    0.00   99.81
root@ryzumi:~#
```