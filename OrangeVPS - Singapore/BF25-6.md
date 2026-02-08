# Package Information

```
$10.78/Month

BF25-6 Package:

8 vCPU (Dual AMD Epyc 7B13)
16 GB RAM DDR4
160 GB NVMe SSD Storage
12 TB Transfer Data @ 750 Mbps
KVM Virtualization
Singapore, Hong Kong, US

https://portal.orangevps.com/store/vps-budget
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
root@ryzumi-epyc:~# lscpu
Architecture:                x86_64
  CPU op-mode(s):            32-bit, 64-bit
  Address sizes:             48 bits physical, 48 bits virtual
  Byte Order:                Little Endian
CPU(s):                      8
  On-line CPU(s) list:       0-7
Vendor ID:                   AuthenticAMD
  Model name:                AMD EPYC 7B13 64-Core Processor
    CPU family:              25
    Model:                   1
    Thread(s) per core:      1
    Core(s) per socket:      1
    Socket(s):               8
    Stepping:                1
    BogoMIPS:                4500.00
    Flags:                   fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush mmx fxsr sse sse2 syscall nx mmxext fxsr_opt pdpe1gb rdtscp lm rep_good nopl cpuid extd_
                             apicid tsc_known_freq pni pclmulqdq ssse3 fma cx16 pcid sse4_1 sse4_2 x2apic movbe popcnt tsc_deadline_timer aes xsave avx f16c rdrand hypervisor lahf_lm cmp_legacy svm
                              cr8_legacy abm sse4a misalignsse 3dnowprefetch osvw perfctr_core ssbd ibrs ibpb stibp vmmcall fsgsbase tsc_adjust bmi1 avx2 smep bmi2 erms invpcid rdseed adx smap clfl
                             ushopt clwb sha_ni xsaveopt xsavec xgetbv1 xsaves clzero xsaveerptr wbnoinvd arat npt lbrv nrip_save tsc_scale vmcb_clean flushbyasid pausefilter pfthreshold v_vmsave_v
                             mload vgif umip pku ospke vaes vpclmulqdq rdpid overflow_recov succor fsrm arch_capabilities
Virtualization features:
  Virtualization:            AMD-V
  Hypervisor vendor:         KVM
  Virtualization type:       full
Caches (sum of all):
  L1d:                       512 KiB (8 instances)
  L1i:                       512 KiB (8 instances)
  L2:                        4 MiB (8 instances)
  L3:                        128 MiB (8 instances)
NUMA:
  NUMA node(s):              1
  NUMA node0 CPU(s):         0-7
Vulnerabilities:
  Gather data sampling:      Not affected
  Indirect target selection: Not affected
  Itlb multihit:             Not affected
  L1tf:                      Not affected
  Mds:                       Not affected
  Meltdown:                  Not affected
  Mmio stale data:           Not affected
  Reg file data sampling:    Not affected
  Retbleed:                  Not affected
  Spec rstack overflow:      Mitigation; Safe RET
  Spec store bypass:         Mitigation; Speculative Store Bypass disabled via prctl
  Spectre v1:                Mitigation; usercopy/swapgs barriers and __user pointer sanitization
  Spectre v2:                Mitigation; Retpolines; IBPB conditional; IBRS_FW; STIBP disabled; RSB filling; PBRSB-eIBRS Not affected; BHI Not affected
  Srbds:                     Not affected
  Tsa:                       Vulnerable: Clear CPU buffers attempted, no microcode
  Tsx async abort:           Not affected
root@ryzumi-epyc:~#
```

## YABS Benchmark

```bash
root@ryzumi-epyc:~# curl -sL https://yabs.sh | bash
# ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## #
#              Yet-Another-Bench-Script              #
#                     v2025-04-20                    #
# https://github.com/masonr/yet-another-bench-script #
# ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## #

Tue Dec 30 08:46:56 AM UTC 2025

Basic System Information:
---------------------------------
Uptime     : 0 days, 0 hours, 6 minutes
Processor  : AMD EPYC 7B13 64-Core Processor
CPU cores  : 8 @ 2250.000 MHz
AES-NI     : ✔ Enabled
VM-x/AMD-V : ✔ Enabled
RAM        : 15.6 GiB
Swap       : 0.0 KiB
Disk       : 159.9 GiB
Distro     : Debian GNU/Linux 13 (trixie)
Kernel     : 6.12.43+deb13-amd64
VM Type    : KVM
IPv4/IPv6  : ✔ Online / ✔ Online

IPv6 Network Information:
---------------------------------
ISP        : Dromatics Systems Pte Ltd
ASN        : AS134677 Dromatics Systems Pte Ltd
Host       : Dromatics Systems Pte Ltd
Location   : Singapore, North West (03)
Country    : Singapore

fio Disk Speed Tests (Mixed R/W 50/50) (Partition /dev/sda1):
---------------------------------
Block Size | 4k            (IOPS) | 64k           (IOPS)
  ------   | ---            ----  | ----           ----
Read       | 226.07 MB/s  (56.5k) | 1.29 GB/s    (20.1k)
Write      | 226.67 MB/s  (56.6k) | 1.29 GB/s    (20.2k)
Total      | 452.75 MB/s (113.1k) | 2.59 GB/s    (40.4k)
           |                      |
Block Size | 512k          (IOPS) | 1m            (IOPS)
  ------   | ---            ----  | ----           ----
Read       | 1.26 GB/s     (2.4k) | 1.25 GB/s     (1.2k)
Write      | 1.32 GB/s     (2.5k) | 1.33 GB/s     (1.3k)
Total      | 2.59 GB/s     (5.0k) | 2.59 GB/s     (2.5k)

iperf3 Network Speed Tests (IPv4):
---------------------------------
Provider        | Location (Link)           | Send Speed      | Recv Speed      | Ping
-----           | -----                     | ----            | ----            | ----
Clouvider       | London, UK (10G)          | 625 Mbits/sec   | 631 Mbits/sec   | 152 ms
Eranium         | Amsterdam, NL (100G)      | 652 Mbits/sec   | 589 Mbits/sec   | 154 ms
Uztelecom       | Tashkent, UZ (10G)        | 679 Mbits/sec   | 623 Mbits/sec   | 179 ms
Leaseweb        | Singapore, SG (10G)       | 642 Mbits/sec   | 594 Mbits/sec   | 1.84 ms
Clouvider       | Los Angeles, CA, US (10G) | 548 Mbits/sec   | 626 Mbits/sec   | 316 ms
Leaseweb        | NYC, NY, US (10G)         | 580 Mbits/sec   | 505 Mbits/sec   | 238 ms
Edgoo           | Sao Paulo, BR (1G)        | 477 Mbits/sec   | 388 Mbits/sec   | 318 ms

iperf3 Network Speed Tests (IPv6):
---------------------------------
Provider        | Location (Link)           | Send Speed      | Recv Speed      | Ping
-----           | -----                     | ----            | ----            | ----
Clouvider       | London, UK (10G)          | 479 Mbits/sec   | 566 Mbits/sec   | 152 ms
Eranium         | Amsterdam, NL (100G)      | 647 Mbits/sec   | 572 Mbits/sec   | 153 ms
Uztelecom       | Tashkent, UZ (10G)        | 617 Mbits/sec   | 607 Mbits/sec   | 179 ms
Leaseweb        | Singapore, SG (10G)       | 750 Mbits/sec   | 704 Mbits/sec   | 10.8 ms
Clouvider       | Los Angeles, CA, US (10G) | 449 Mbits/sec   | 13.9 Mbits/sec  | 185 ms
Leaseweb        | NYC, NY, US (10G)         | 570 Mbits/sec   | 441 Mbits/sec   | 237 ms
Edgoo           | Sao Paulo, BR (1G)        | 529 Mbits/sec   | 280 Mbits/sec   | 318 ms

Geekbench 6 Benchmark Test:
---------------------------------
Test            | Value
                |
Single Core     | 1677
Multi Core      | 9052
Full Test       | https://browser.geekbench.com/v6/cpu/15842177

YABS completed in 12 min 49 sec
```

## Bench.Monster Benchmark

```bash
root@ryzumi-epyc:~# curl -sL bench.monster | bash
---------------------------------------------------------------------------
 Region: Global  https://bench.laset.com v1.8.5 2025-10-20
 Usage : curl -sL bench.laset.com | bash -s -- -Global
---------------------------------------------------------------------------
 OS           : Debian GNU/Linux 13 (64 Bit)
 Virt/Kernel  : KVM / 6.12.43+deb13-amd64
 CPU Model    : AMD EPYC 7B13 64-Core Processor
 CPU Cores    : 8 @ 2250.000 MHz x86_64 512 KB Cache
 CPU Flags    : AES-NI Enabled & VM-x/AMD-V Enabled
 Load Average : 0.28, 0.40, 0.27
 Total Space  : 160G (4.2G ~3% used)
 Total RAM    : 15998 MB (446 MB + 432 MB Buff in use)
 Total SWAP   : 0 MB (0 MB in use)
 IPv4/IPv6    : ✔ Online / ✔ Online
 Uptime       : 0 days 0:23
---------------------------------------------------------------------------
 Location     : Singapore, Singapore (North West)
 ASN & ISP    : AS134677, Dromatics Systems Pte Ltd / Dromatics Systems Pte Ltd
---------------------------------------------------------------------------

 ## Geekbench v6 CPU Benchmark:

  Single Core : 1705  (EXCELLENT)
   Multi Core : 8957
    CPU Steal : 0%

 ## IO Test

 CPU Speed:
    bzip2     : 153 MB/s
   sha256     : 1.1 GB/s
   md5sum     : 634 MB/s
    Steal     : 0%

 RAM Speed:
   Avg. write : 2321.1 MB/s
   Avg. read  : 11468.8 MB/s

 Disk Speed:
   1st run    : 2.3 GB/s
   2nd run    : 2.3 GB/s
   3rd run    : 2.4 GB/s
   -----------------------
   Average    : 2389.3 MB/s

 ## Global Speedtest.net

 Location                             Upload      Download       Ping    Loss
-------------------------------------------------------------------------------
 Nearby                           749.03 Mbps   702.73 Mbps    0.71 ms      0%
-------------------------------------------------------------------------------
 USA, New York (Optimum)          378.53 Mbps   496.37 Mbps  229.53 ms      0%
 USA, Chicago (Uniti)             452.39 Mbps   652.02 Mbps  210.87 ms     N/A
 USA, Los Angeles (Uniti)         434.92 Mbps   688.75 Mbps  183.01 ms     N/A
 UK, London (Hyperoptic)          708.12 Mbps   674.20 Mbps  153.26 ms     N/A
 Germany, Frankfurt (Plusnet)     697.25 Mbps   487.18 Mbps  149.99 ms      0%
 India, Mumbai (Tata Play)        572.71 Mbps   711.75 Mbps  163.39 ms   0.43%
 Singapore (MyRepublic)           749.28 Mbps   717.03 Mbps    2.00 ms      0%
 Japan, Tokyo (Nearoute)          760.84 Mbps   764.16 Mbps   83.73 ms   1.00%
 Australia, Sydney (Neptune)      547.54 Mbps   739.77 Mbps  166.90 ms   0.33%

 ## Statistics

 Total Traffic    : 15.58 GB
 Total Downloaded : 8.07 GB
 Total Uploaded   : 7.52 GB

 Average Loss     : 0.25 %

---------------------------------------------------------------------------
 Finished in : 12 min 10 sec

 Timestamp   : 2025-12-30 09:15:58 GMT
 Saved in    : /root/speedtest.log

 Share results:
 - https://www.speedtest.net/result/c/2ae8a445-988d-4a92-8732-cf901d8f7eb5
 - https://browser.geekbench.com/v6/cpu/15842300
```

## Bench.sh Benchmark

```bash
-------------------- A Bench.sh Script By Teddysun -------------------
 Version            : v2025-05-08
 Usage              : wget -qO- bench.sh | bash
----------------------------------------------------------------------
 CPU Model          : AMD EPYC 7B13 64-Core Processor
 CPU Cores          : 8 @ 2250.000 MHz
 CPU Cache          : 512 KB
 AES-NI             : ✓ Enabled
 VM-x/AMD-V         : ✓ Enabled
 Total Disk         : 159.9 GB (4.2 GB Used)
 Total Mem          : 15.6 GB (446.7 MB Used)
 System uptime      : 0 days, 0 hour 40 min
 Load average       : 0.01, 0.16, 0.27
 OS                 : Debian GNU/Linux 13
 Arch               : x86_64 (64 Bit)
 Kernel             : 6.12.43+deb13-amd64
 TCP CC             : bbr
 Virtualization     : KVM
 IPv4/IPv6          : ✓ Online / ✓ Online
 Organization       : AS134677 Dromatics Systems Pte Ltd
 Location           : Singapore / SG
 Region             : Singapore
----------------------------------------------------------------------
 I/O Speed(1st run) : 2.1 GB/s
 I/O Speed(2nd run) : 2.3 GB/s
 I/O Speed(3rd run) : 2.3 GB/s
 I/O Speed(average) : 2286.9 MB/s
----------------------------------------------------------------------
 Node Name        Upload Speed      Download Speed      Latency
 Speedtest.net    749.02 Mbps       718.61 Mbps         0.60 ms
 Paris, FR        695.87 Mbps       771.18 Mbps         145.13 ms
 Shanghai, CN     555.78 Mbps       605.53 Mbps         361.03 ms
 Hong Kong, CN    752.49 Mbps       716.42 Mbps         39.43 ms
 Singapore, SG    325.68 Mbps       703.44 Mbps         41.89 ms
 Tokyo, JP        720.07 Mbps       735.56 Mbps         97.94 ms
----------------------------------------------------------------------
 Finished in        : 2 min 52 sec
 Timestamp          : 2025-12-30 09:23:12 UTC
----------------------------------------------------------------------
```

## CPU Steal

```bash
root@ryzumi-epyc:~# mpstat 30 5
Linux 6.12.43+deb13-amd64 (ryzumi-epyc)         12/30/2025      _x86_64_        (8 CPU)

09:16:35 AM  CPU    %usr   %nice    %sys %iowait    %irq   %soft  %steal  %guest  %gnice   %idle
09:17:05 AM  all    0.11    0.00    0.13    0.00    0.00    0.02    0.00    0.00    0.00   99.74
09:17:35 AM  all    0.02    0.00    0.08    0.00    0.00    0.04    0.00    0.00    0.00   99.86
09:18:05 AM  all    0.02    0.00    0.08    0.00    0.00    0.02    0.00    0.00    0.00   99.89
09:18:35 AM  all    0.01    0.00    0.03    0.00    0.00    0.01    0.00    0.00    0.00   99.95
09:19:05 AM  all    0.00    0.00    0.00    0.00    0.00    0.00    0.00    0.00    0.00  100.00
Average:     all    0.03    0.00    0.06    0.00    0.00    0.02    0.00    0.00    0.00   99.89
root@ryzumi-epyc:~#

```