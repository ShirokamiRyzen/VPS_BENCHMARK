# Package Information

```
ServaRica V1 UniFied Expanding

1x Slice Package:

1 Dedicated Core AMD EPYC 7551P
4 GB RAM DDR4
125 GB NVMe SSD Storage
500 GB SAN Storage with unlimited grow 1GB/Day
Unlimited Bandwidth @ 250Mbps with +1mbps Daily increase maximum of 1gbps or
Limited Bandwidth (4TB) x (Number Of Slices) on 10Gbps Port
XEN Virtualization
Montreal, Canada

https://clients.servarica.com/cart.php?a=confproduct&i=0
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
root@storage-vm:~# lscpu
Architecture:                x86_64
  CPU op-mode(s):            32-bit, 64-bit
  Address sizes:             48 bits physical, 48 bits virtual
  Byte Order:                Little Endian
CPU(s):                      1
  On-line CPU(s) list:       0
Vendor ID:                   AuthenticAMD
  Model name:                AMD EPYC 7551P 32-Core Processor
    CPU family:              23
    Model:                   1
    Thread(s) per core:      1
    Core(s) per socket:      1
    Socket(s):               1
    Stepping:                2
    BogoMIPS:                3992.50
    Flags:                   fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush mmx fxsr sse sse2 ht syscall nx mmxext fxsr_opt pdpe1gb rdtscp lm rep_good nopl cpuid extd
                             _apicid tsc_known_freq pni pclmulqdq ssse3 fma cx16 sse4_1 sse4_2 x2apic movbe popcnt aes xsave avx f16c rdrand hypervisor lahf_lm cmp_legacy cr8_legacy abm sse4a misalig
                             nsse 3dnowprefetch bpext ssbd ibpb vmmcall fsgsbase bmi1 avx2 smep bmi2 rdseed adx smap clflushopt sha_ni xsaveopt xsavec xgetbv1 xsaves clzero xsaveerptr virt_ssbd arat
Virtualization features:
  Hypervisor vendor:         Microsoft
  Virtualization type:       full
Caches (sum of all):
  L1d:                       32 KiB (1 instance)
  L1i:                       64 KiB (1 instance)
  L2:                        512 KiB (1 instance)
  L3:                        64 MiB (1 instance)
NUMA:
  NUMA node(s):              1
  NUMA node0 CPU(s):         0
Vulnerabilities:
  Gather data sampling:      Not affected
  Indirect target selection: Not affected
  Itlb multihit:             Not affected
  L1tf:                      Not affected
  Mds:                       Not affected
  Meltdown:                  Not affected
  Mmio stale data:           Not affected
  Reg file data sampling:    Not affected
  Retbleed:                  Mitigation; untrained return thunk; SMT disabled
  Spec rstack overflow:      Mitigation; SMT disabled
  Spec store bypass:         Mitigation; Speculative Store Bypass disabled via prctl
  Spectre v1:                Mitigation; usercopy/swapgs barriers and __user pointer sanitization
  Spectre v2:                Mitigation; Retpolines; IBPB conditional; STIBP disabled; RSB filling; PBRSB-eIBRS Not affected; BHI Not affected
  Srbds:                     Not affected
  Tsa:                       Not affected
  Tsx async abort:           Not affected
  Vmscape:                   Not affected
```

## YABS Benchmark

```bash
root@storage-vm:~# curl -sL https://yabs.sh | bash
# ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## #
#              Yet-Another-Bench-Script              #
#                     v2025-04-20                    #
# https://github.com/masonr/yet-another-bench-script #
# ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## #

Fri Apr 24 09:15:25 AM WIB 2026

Basic System Information:
---------------------------------
Uptime     : 0 days, 20 hours, 12 minutes
Processor  : AMD EPYC 7551P 32-Core Processor
CPU cores  : 1 @ 1996.253 MHz
AES-NI     : ✔ Enabled
VM-x/AMD-V : ❌ Disabled
RAM        : 3.8 GiB
Swap       : 8.0 GiB
Disk       : 615.0 GiB
Distro     : Debian GNU/Linux 13 (trixie)
Kernel     : 6.12.74+deb13+1-amd64
VM Type    : XEN
IPv4/IPv6  : ✔ Online / ❌ Offline

IPv4 Network Information:
---------------------------------
ISP        : Rica Web Services
ASN        : AS26832 Rica Web Services
Host       : Rica Web Services
Location   : Montreal, Quebec (QC)
Country    : Canada

fio Disk Speed Tests (Mixed R/W 50/50) (Partition /dev/mapper/unified--nvme-main):
---------------------------------
Block Size | 4k            (IOPS) | 64k           (IOPS)
  ------   | ---            ----  | ----           ----
Read       | 31.66 MB/s    (7.9k) | 222.13 MB/s   (3.4k)
Write      | 31.71 MB/s    (7.9k) | 223.30 MB/s   (3.4k)
Total      | 63.37 MB/s   (15.8k) | 445.44 MB/s   (6.9k)
           |                      |
Block Size | 512k          (IOPS) | 1m            (IOPS)
  ------   | ---            ----  | ----           ----
Read       | 316.23 MB/s    (617) | 307.13 MB/s    (299)
Write      | 333.03 MB/s    (650) | 327.59 MB/s    (319)
Total      | 649.27 MB/s   (1.2k) | 634.73 MB/s    (618)

iperf3 Network Speed Tests (IPv4):
---------------------------------
Provider        | Location (Link)           | Send Speed      | Recv Speed      | Ping
-----           | -----                     | ----            | ----            | ----
Clouvider       | London, UK (10G)          | 236 Mbits/sec   | 398 Mbits/sec   | 95.0 ms
Eranium         | Amsterdam, NL (100G)      | 240 Mbits/sec   | 4.64 Gbits/sec  | 80.1 ms
Uztelecom       | Tashkent, UZ (10G)        | 221 Mbits/sec   | 217 Mbits/sec   | 169 ms
Leaseweb        | Singapore, SG (10G)       | 205 Mbits/sec   | 907 Mbits/sec   | 238 ms
Clouvider       | Los Angeles, CA, US (10G) | 242 Mbits/sec   | 688 Mbits/sec   | 68.6 ms
Leaseweb        | NYC, NY, US (10G)         | 251 Mbits/sec   | 1.18 Gbits/sec  | 10.2 ms
Edgoo           | Sao Paulo, BR (1G)        | 232 Mbits/sec   | 354 Mbits/sec   | 118 ms

Geekbench 6 Benchmark Test:
---------------------------------
Test            | Value
                |
Single Core     | 799
Multi Core      | 805
Full Test       | https://browser.geekbench.com/v6/cpu/17775708

YABS completed in 17 min 52 sec
```

## Bench.Monster Benchmark

```bash
root@storage-vm:~# curl -sL bench.monster | bash
---------------------------------------------------------------------------
 Region: Global  https://bench.laset.com v1.8.7 2026-02-02
 Usage : curl -sL bench.laset.com | bash -s -- -Global
---------------------------------------------------------------------------
 OS           : Debian GNU/Linux 13 (64 Bit)
 Virt/Kernel  : Xen / 6.12.74+deb13+1-amd64
 CPU Model    : AMD EPYC 7551P 32-Core Processor
 CPU Cores    : 1 @ 1996.253 MHz x86_64 512 KB Cache
 CPU Flags    : AES-NI Enabled & VM-x/AMD-V Disabled
 Load Average : 0.38, 0.88, 1.02
 Total Space  : 615G (26G ~5% used)
 Total RAM    : 3918 MB (1348 MB + 1036 MB Buff in use)
 Total SWAP   : 8191 MB (394 MB in use)
 IPv4/IPv6    : ✔ Online / ❌ Offline
 Uptime       : 0 days 20:52
---------------------------------------------------------------------------
 Location     : Canada, Montreal (Quebec)
 ASN & ISP    : AS26832, Rica Web Services / Rica Web Services
---------------------------------------------------------------------------

 ## Geekbench v6 CPU Benchmark:

  Single Core : 810  (GOOD)
   Multi Core : 801
    CPU Steal : 0.13%

 ## IO Test

 CPU Speed:
    bzip2     : 77.2 MB/s
   sha256     : 714 MB/s
   md5sum     : 363 MB/s
    Steal     : 0.11%

 RAM Speed:
   Avg. write : 1433.6 MB/s
   Avg. read  : 7236.3 MB/s

 Disk Speed:
   1st run    : 381 MB/s
   2nd run    : 421 MB/s
   3rd run    : 483 MB/s
   -----------------------
   Average    : 428.3 MB/s

 ## Global Speedtest.net

 Location                             Upload      Download       Ping    Loss
-------------------------------------------------------------------------------
 Nearby                           249.22 Mbps  2220.87 Mbps    6.91 ms      0%
-------------------------------------------------------------------------------
 USA, New York (Optimum)          250.44 Mbps  2049.82 Mbps   10.36 ms      0%
 USA, Chicago (Uniti)             251.18 Mbps  1434.54 Mbps   23.74 ms     N/A
 USA, Los Angeles (Uniti)         253.11 Mbps  1231.40 Mbps   78.53 ms     N/A
 UK, London (Hyperoptic)          254.87 Mbps  1130.49 Mbps   81.15 ms     N/A
 Germany, Frankfurt (Plusnet)     252.80 Mbps  1867.02 Mbps   90.24 ms      0%

 ## Statistics

 Total Traffic    : 15.58 GB
 Total Downloaded : 13.77 GB
 Total Uploaded   : 1.81 GB

 Average Loss     : 0.00 %

---------------------------------------------------------------------------
 Finished in : 19 min 26 sec

 Timestamp   : 2026-04-24 03:14:54 GMT
 Saved in    : /root/speedtest.log

 Share results:
 - https://www.speedtest.net/result/c/97cf7a87-1726-479d-a2ed-74b4bf03d8d8
 - https://browser.geekbench.com/v6/cpu/17776002

root@storage-vm:~#
```

## Bench.sh Benchmark

```bash
-------------------- A Bench.sh Script By Teddysun -------------------
 Version            : v2026-01-31
 Usage              : wget -qO- bench.sh | bash
----------------------------------------------------------------------
 CPU Model          : AMD EPYC 7551P 32-Core Processor
 CPU Cores          : 1 @ 1996.253 MHz
 CPU Cache          : 512 KB
 AES-NI             : ✓ Enabled
 VM-x/AMD-V         : ✗ Disabled
 Total Disk         : 623.0 GB (26.2 GB Used)
 Total RAM          : 3.8 GB (1.3 GB Used)
 Total Swap         : 8.0 GB (394.2 MB Used)
 System Uptime      : 0 days, 20 hour 41 min
 Load Average       : 0.01, 0.11, 0.34
 OS                 : Debian GNU/Linux 13 (trixie)
 Arch               : x86_64 (64 Bit)
 Kernel             : 6.12.74+deb13+1-amd64
 TCP Congestion Ctrl: bbr
 Virtualization     : XEN
 IPv4/IPv6          : ✓ Online / ✗ Offline
 Organization       : AS26832 Rica Web Services
 Location           : Montréal / CA
 Region             : Quebec
----------------------------------------------------------------------
 I/O Speed(1st run) : 355 MB/s
 I/O Speed(2nd run) : 481 MB/s
 I/O Speed(3rd run) : 479 MB/s
 I/O Speed(average) : 438.3 MB/s
----------------------------------------------------------------------
 Node Name        Upload Speed      Download Speed      Latency
 Speedtest.net    249.63 Mbps       2584.46 Mbps        6.94 ms
 Los Angeles, US  248.56 Mbps       3404.20 Mbps        68.81 ms
 Dallas, US       250.58 Mbps       1099.45 Mbps        41.55 ms
 Montreal, CA     249.76 Mbps       2310.13 Mbps        7.79 ms
 Paris, FR        Test failed
 Amsterdam, NL    253.31 Mbps       965.92 Mbps         78.93 ms
 Suzhou, CN       Test failed
 Ningbo, CN       Test failed
 Hong Kong, CN    Test failed
 Singapore, SG    Test failed
 Taipei, CN       Test failed
 Tokyo, JP        237.78 Mbps       2677.16 Mbps        154.14 ms
----------------------------------------------------------------------
 Finished in        : 5 min 10 sec
 Timestamp          : 2026-04-24 09:49:17 WIB
----------------------------------------------------------------------
```

## CPU Steal

```bash
root@storage-vm:~# mpstat 30 5
Linux 6.12.74+deb13+1-amd64 (storage-vm)        04/24/2026      _x86_64_        (1 CPU)

09:39:46 AM  CPU    %usr   %nice    %sys %iowait    %irq   %soft  %steal  %guest  %gnice   %idle
09:40:16 AM  all    6.17    0.00    3.10    0.10    0.00    0.10    0.30    0.00    0.00   90.23
09:40:46 AM  all    3.57    0.00    2.26    0.03    0.00    0.07    0.30    0.00    0.00   93.76
09:41:16 AM  all    1.72    0.00    2.02    0.03    0.00    0.03    0.30    0.00    0.00   95.89
09:41:46 AM  all    1.38    0.00    1.72    0.03    0.00    0.00    0.34    0.00    0.00   96.53
09:42:16 AM  all    1.55    0.00    2.19    0.03    0.00    0.03    0.30    0.00    0.00   95.89
Average:     all    2.88    0.00    2.26    0.05    0.00    0.05    0.31    0.00    0.00   94.46
root@storage-vm:~#
```