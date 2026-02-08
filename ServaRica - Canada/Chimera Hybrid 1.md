# Package Information

```
ServaRica KVM Hybrid deals 2025

Chimera Hybrid - 1 Package:

2 vCPU Intel Xeon Gold 5118
4 GB RAM DDR4
65 GB NVMe SSD Storage
2TB HDD
12TB @ 1 Gbps
KVM Virtualization
Montreal, Canada

https://clients.servarica.com/store/bf-2025-kvm-hybrid
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
root@ryzumi-drive:~# lscpu
Architecture:                x86_64
  CPU op-mode(s):            32-bit, 64-bit
  Address sizes:             46 bits physical, 48 bits virtual
  Byte Order:                Little Endian
CPU(s):                      2
  On-line CPU(s) list:       0,1
Vendor ID:                   GenuineIntel
  Model name:                Intel(R) Xeon(R) Gold 5118 CPU @ 2.30GHz
    CPU family:              6
    Model:                   85
    Thread(s) per core:      1
    Core(s) per socket:      2
    Socket(s):               1
    Stepping:                4
    BogoMIPS:                4599.99
    Flags:                   fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush mmx fxsr sse sse2 ss ht syscall nx pdpe1gb rdtscp lm constant_tsc arch_perfmon r
                             ep_good nopl xtopology cpuid tsc_known_freq pni pclmulqdq vmx ssse3 fma cx16 pdcm pcid sse4_1 sse4_2 x2apic movbe popcnt tsc_deadline_timer aes xsave avx f16c r
                             drand hypervisor lahf_lm abm 3dnowprefetch cpuid_fault pti ssbd ibrs ibpb stibp tpr_shadow flexpriority ept vpid ept_ad fsgsbase tsc_adjust bmi1 hle avx2 smep b
                             mi2 erms invpcid rtm mpx avx512f avx512dq rdseed adx smap clflushopt clwb avx512cd avx512bw avx512vl xsaveopt xsavec xgetbv1 xsaves arat vnmi umip pku ospke md_
                             clear flush_l1d arch_capabilities
Virtualization features:
  Virtualization:            VT-x
  Hypervisor vendor:         KVM
  Virtualization type:       full
Caches (sum of all):
  L1d:                       64 KiB (2 instances)
  L1i:                       64 KiB (2 instances)
  L2:                        8 MiB (2 instances)
  L3:                        16 MiB (1 instance)
NUMA:
  NUMA node(s):              1
  NUMA node0 CPU(s):         0,1
Vulnerabilities:
  Gather data sampling:      Not affected
  Indirect target selection: Mitigation; Aligned branch/return thunks
  Itlb multihit:             Not affected
  L1tf:                      Mitigation; PTE Inversion; VMX flush not necessary, SMT disabled
  Mds:                       Mitigation; Clear CPU buffers; SMT Host state unknown
  Meltdown:                  Mitigation; PTI
  Mmio stale data:           Mitigation; Clear CPU buffers; SMT Host state unknown
  Reg file data sampling:    Not affected
  Retbleed:                  Mitigation; IBRS
  Spec rstack overflow:      Not affected
  Spec store bypass:         Mitigation; Speculative Store Bypass disabled via prctl
  Spectre v1:                Mitigation; usercopy/swapgs barriers and __user pointer sanitization
  Spectre v2:                Mitigation; IBRS; IBPB conditional; STIBP disabled; RSB filling; PBRSB-eIBRS Not affected; BHI SW loop, KVM SW loop
  Srbds:                     Not affected
  Tsa:                       Not affected
  Tsx async abort:           Mitigation; Clear CPU buffers; SMT Host state unknown
  Vmscape:                   Not affected
```

## YABS Benchmark

```bash
root@ryzumi-drive:~# curl -sL https://yabs.sh | bash
# ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## #
#              Yet-Another-Bench-Script              #
#                     v2025-04-20                    #
# https://github.com/masonr/yet-another-bench-script #
# ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## #

Sun Feb  8 16:08:17 WIB 2026

Basic System Information:
---------------------------------
Uptime     : 4 days, 18 hours, 30 minutes
Processor  : Intel(R) Xeon(R) Gold 5118 CPU @ 2.30GHz
CPU cores  : 2 @ 2299.998 MHz
AES-NI     : ✔ Enabled
VM-x/AMD-V : ✔ Enabled
RAM        : 3.8 GiB
Swap       : 4.0 GiB
Disk       : 2.0 TiB
Distro     : Debian GNU/Linux 13 (trixie)
Kernel     : 6.12.63+deb13-cloud-amd64
VM Type    : KVM
IPv4/IPv6  : ✔ Online / ✔ Online

IPv6 Network Information:
---------------------------------
ISP        : Rica Web Services
ASN        : AS26832 Rica Web Services
Host       : Rica Web Services
Location   : Montreal, Quebec (QC)
Country    : Canada

fio Disk Speed Tests (Mixed R/W 50/50) (Partition /dev/sda1):
---------------------------------
Block Size | 4k            (IOPS) | 64k           (IOPS)
  ------   | ---            ----  | ----           ----
Read       | 247.50 MB/s  (61.8k) | 488.70 MB/s   (7.6k)
Write      | 248.15 MB/s  (62.0k) | 491.27 MB/s   (7.6k)
Total      | 495.66 MB/s (123.9k) | 979.97 MB/s  (15.3k)
           |                      |
Block Size | 512k          (IOPS) | 1m            (IOPS)
  ------   | ---            ----  | ----           ----
Read       | 549.01 MB/s   (1.0k) | 522.41 MB/s    (510)
Write      | 578.18 MB/s   (1.1k) | 557.20 MB/s    (544)
Total      | 1.12 GB/s     (2.2k) | 1.07 GB/s     (1.0k)

iperf3 Network Speed Tests (IPv4):
---------------------------------
Provider        | Location (Link)           | Send Speed      | Recv Speed      | Ping
-----           | -----                     | ----            | ----            | ----
Clouvider       | London, UK (10G)          | 732 Mbits/sec   | 941 Mbits/sec   | 76.8 ms
Eranium         | Amsterdam, NL (100G)      | 939 Mbits/sec   | 912 Mbits/sec   | 82.1 ms
Uztelecom       | Tashkent, UZ (10G)        | 748 Mbits/sec   | 825 Mbits/sec   | 168 ms
Leaseweb        | Singapore, SG (10G)       | 501 Mbits/sec   | 793 Mbits/sec   | 249 ms
Clouvider       | Los Angeles, CA, US (10G) | 685 Mbits/sec   | 940 Mbits/sec   | 81.3 ms
Leaseweb        | NYC, NY, US (10G)         | 1.03 Gbits/sec  | 978 Mbits/sec   | 9.58 ms
Edgoo           | Sao Paulo, BR (1G)        | 876 Mbits/sec   | busy            | 118 ms

iperf3 Network Speed Tests (IPv6):
---------------------------------
Provider        | Location (Link)           | Send Speed      | Recv Speed      | Ping
-----           | -----                     | ----            | ----            | ----
Clouvider       | London, UK (10G)          | 687 Mbits/sec   | 925 Mbits/sec   | 76.8 ms
Eranium         | Amsterdam, NL (100G)      | 939 Mbits/sec   | 895 Mbits/sec   | 82.0 ms
Uztelecom       | Tashkent, UZ (10G)        | 779 Mbits/sec   | 831 Mbits/sec   | 168 ms
Leaseweb        | Singapore, SG (10G)       | busy            | 770 Mbits/sec   | 271 ms
Clouvider       | Los Angeles, CA, US (10G) | 639 Mbits/sec   | 928 Mbits/sec   | 81.2 ms
Leaseweb        | NYC, NY, US (10G)         | 1.03 Gbits/sec  | 968 Mbits/sec   | 27.1 ms
Edgoo           | Sao Paulo, BR (1G)        | 876 Mbits/sec   | 898 Mbits/sec   | 117 ms

Running GB6 benchmark test... *cue elevator music*
Geekbench 6 Benchmark Test:
---------------------------------
Test            | Value
                |
Single Core     | 848
Multi Core      | 1450
Full Test       | https://browser.geekbench.com/v6/cpu/16477142

YABS completed in 16 min 45 sec
```

## Bench.Monster Benchmark

```bash
root@ryzumi-drive:~# curl -sL bench.monster | bash
---------------------------------------------------------------------------
 Region: Global  https://bench.laset.com v1.8.7 2026-02-02
 Usage : curl -sL bench.laset.com | bash -s -- -Global
---------------------------------------------------------------------------
 OS           : Debian GNU/Linux 13 (64 Bit)
 Virt/Kernel  : KVM / 6.12.63+deb13-cloud-amd64
 CPU Model    : Intel(R) Xeon(R) Gold 5118 CPU @ 2.30GHz
 CPU Cores    : 2 @ 2299.998 MHz x86_64 16384 KB Cache
 CPU Flags    : AES-NI Enabled & VM-x/AMD-V Enabled
 Load Average : 0.27, 0.71, 0.55
 Total Space  : 2.0T (19G ~1% used)
 Total RAM    : 3922 MB (873 MB + 1450 MB Buff in use)
 Total SWAP   : 4095 MB (0 MB in use)
 IPv4/IPv6    : ✔ Online / ✔ Online
 Uptime       : 4 days 18:50
---------------------------------------------------------------------------
 Location     : Canada, Montreal (Quebec)
 ASN & ISP    : AS26832, Rica Web Services / Servarica
---------------------------------------------------------------------------

 ## Geekbench v6 CPU Benchmark:

  Single Core : 796  (GOOD)
   Multi Core : 1486
    CPU Steal : 0.01%

 ## IO Test

 CPU Speed:
    bzip2     : 84.0 MB/s
   sha256     : 267 MB/s
   md5sum     : 456 MB/s
    Steal     : 0%

 RAM Speed:
   Avg. write : 1740.8 MB/s
   Avg. read  : 6246.4 MB/s

 Disk Speed:
   1st run    : 674 MB/s
   2nd run    : 553 MB/s
   3rd run    : 539 MB/s
   -----------------------
   Average    : 588.7 MB/s

 ## Global Speedtest.net

 Location                             Upload      Download       Ping    Loss
-------------------------------------------------------------------------------
 Nearby                          1023.94 Mbps   987.00 Mbps    0.60 ms      0%
-------------------------------------------------------------------------------
 USA, New York (Optimum)         1034.74 Mbps   978.95 Mbps   10.31 ms      0%
 USA, Chicago (Uniti)            1007.54 Mbps   969.17 Mbps   22.09 ms     N/A
 USA, Los Angeles (Uniti)         426.86 Mbps   967.89 Mbps   78.60 ms     N/A
 UK, London (Hyperoptic)          924.32 Mbps   984.38 Mbps   85.08 ms     N/A
 Germany, Frankfurt (Plusnet)     853.95 Mbps  1020.81 Mbps   90.31 ms      0%
 India, Mumbai (Tata Play)        155.81 Mbps   981.86 Mbps  240.57 ms      0%
 Japan, Tokyo (Nearoute)          793.90 Mbps  1045.69 Mbps  140.11 ms   1.00%
 Australia, Sydney (Neptune)      105.34 Mbps  1015.67 Mbps  194.85 ms      0%

 ## Statistics

 Total Traffic    : 18.19 GB
 Total Downloaded : 10.93 GB
 Total Uploaded   : 7.27 GB

 Average Loss     : 0.17 %

---------------------------------------------------------------------------
 Finished in : 16 min 29 sec

 Timestamp   : 2026-02-08 09:44:13 GMT
 Saved in    : /root/speedtest.log

 Share results:
 - https://www.speedtest.net/result/c/e63f7469-83af-4f86-b511-97343bce63cf
 - https://browser.geekbench.com/v6/cpu/16477267

root@ryzumi-drive:~#
```

## Bench.sh Benchmark

```bash
-------------------- A Bench.sh Script By Teddysun -------------------
 Version            : v2026-01-31
 Usage              : wget -qO- bench.sh | bash
----------------------------------------------------------------------
 CPU Model          : Intel(R) Xeon(R) Gold 5118 CPU @ 2.30GHz
 CPU Cores          : 2 @ 2299.998 MHz
 CPU Cache          : 16384 KB
 AES-NI             : ✓ Enabled
 VM-x/AMD-V         : ✓ Enabled
 Total Disk         : 2.0 TB (18.2 GB Used)
 Total RAM          : 3.8 GB (782.4 MB Used)
 Total Swap         : 4.0 GB (780.0 KB Used)
 System Uptime      : 4 days, 18 hour 23 min
 Load Average       : 0.47, 0.17, 0.05
 OS                 : Debian GNU/Linux 13 (trixie)
 Arch               : x86_64 (64 Bit)
 Kernel             : 6.12.63+deb13-cloud-amd64
 TCP Congestion Ctrl: bbr
 Virtualization     : KVM
 IPv4/IPv6          : ✓ Online / ✓ Online
 Organization       : AS26832 Rica Web Services
 Location           : Montréal / CA
 Region             : Quebec
----------------------------------------------------------------------
 I/O Speed(1st run) : 817 MB/s
 I/O Speed(2nd run) : 639 MB/s
 I/O Speed(3rd run) : 634 MB/s
 I/O Speed(average) : 696.7 MB/s
----------------------------------------------------------------------
 Node Name        Upload Speed      Download Speed      Latency
 Speedtest.net    1032.89 Mbps      968.00 Mbps         0.57 ms
 Los Angeles, US  943.55 Mbps       1035.80 Mbps        72.83 ms
 Dallas, US       1013.83 Mbps      1019.68 Mbps        40.36 ms
 Montreal, CA     829.84 Mbps       951.39 Mbps         36.04 ms
 Paris, FR        913.56 Mbps       988.40 Mbps         87.54 ms
 Amsterdam, NL    443.59 Mbps       962.25 Mbps         88.92 ms
 Suzhou, CN       190.85 Mbps       970.39 Mbps         212.21 ms
 Ningbo, CN       22.50 Mbps        994.09 Mbps         400.71 ms
 Hong Kong, CN    2.47 Mbps         3.12 Mbps           211.18 ms
 Singapore, SG    21.03 Mbps        237.65 Mbps         246.25 ms
 Taipei, CN       717.22 Mbps       939.40 Mbps         175.27 ms
 Tokyo, JP        683.47 Mbps       1032.30 Mbps        179.24 ms
----------------------------------------------------------------------
 Finished in        : 6 min 1 sec
 Timestamp          : 2026-02-08 16:06:58 WIB
----------------------------------------------------------------------
```

## CPU Steal

```bash
root@ryzumi-drive:~# mpstat 30 5
Linux 6.12.63+deb13-cloud-amd64 (ryzumi-drive)  02/08/26        _x86_64_        (2 CPU)

15:57:54     CPU    %usr   %nice    %sys %iowait    %irq   %soft  %steal  %guest  %gnice   %idle
15:58:24     all    0.80    0.00    0.77    0.02    0.00    0.03    0.00    0.00    0.00   98.38
15:58:54     all    0.74    0.00    0.85    0.02    0.00    0.00    0.00    0.00    0.00   98.40
15:59:24     all    1.00    0.00    0.73    0.08    0.00    0.02    0.00    0.00    0.00   98.15
15:59:54     all    0.65    0.00    0.95    0.02    0.00    0.02    0.00    0.00    0.00   98.36
16:00:24     all    1.47    0.00    0.92    2.27    0.00    0.02    0.00    0.00    0.00   95.32
Average:     all    0.93    0.00    0.85    0.48    0.00    0.02    0.00    0.00    0.00   97.72
root@ryzumi-drive:~#

```