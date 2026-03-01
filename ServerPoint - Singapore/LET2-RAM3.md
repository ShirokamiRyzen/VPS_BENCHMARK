# Package Information

```
ServerPoint XEON E5v4 deals 2025

LET2-RAM3 Package:

8 vCPUs, Intel E5v4 at 2.1Ghz
32 GBs of RAM
200 GBs SSD storage
20.000 GBs/mo data transfer
1 IPv4 IP included
1gbps network port
Private VLAN included
DDoS protection included

https://portal.serverpoint.com/#/public/checkout/vs/letmar25
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
root@ryzumi-xeon:~# lscpu
Architecture:                x86_64
  CPU op-mode(s):            32-bit, 64-bit
  Address sizes:             46 bits physical, 48 bits virtual
  Byte Order:                Little Endian
CPU(s):                      8
  On-line CPU(s) list:       0-7
Vendor ID:                   GenuineIntel
  Model name:                Intel(R) Xeon(R) CPU E5-2699A v4 @ 2.40GHz
    CPU family:              6
    Model:                   79
    Thread(s) per core:      1
    Core(s) per socket:      4
    Socket(s):               2
    Stepping:                1
    BogoMIPS:                4799.99
    Flags:                   fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush mmx fxsr sse sse2 ss ht syscall nx pdpe1gb rdtscp lm constant_tsc arch_perfmon rep_good
                              nopl xtopology cpuid tsc_known_freq pni pclmulqdq vmx ssse3 fma cx16 pdcm pcid sse4_1 sse4_2 x2apic movbe popcnt tsc_deadline_timer aes xsave avx f16c rdrand hypervis
                             or lahf_lm abm 3dnowprefetch cpuid_fault pti ssbd ibrs ibpb stibp tpr_shadow flexpriority ept vpid ept_ad fsgsbase tsc_adjust bmi1 hle avx2 smep bmi2 erms invpcid rtm
                             rdseed adx smap xsaveopt arat vnmi umip md_clear arch_capabilities
Virtualization features:
  Virtualization:            VT-x
  Hypervisor vendor:         Microsoft
  Virtualization type:       full
Caches (sum of all):
  L1d:                       256 KiB (8 instances)
  L1i:                       256 KiB (8 instances)
  L2:                        32 MiB (8 instances)
  L3:                        32 MiB (2 instances)
NUMA:
  NUMA node(s):              1
  NUMA node0 CPU(s):         0-7
Vulnerabilities:
  Gather data sampling:      Not affected
  Indirect target selection: Mitigation; Aligned branch/return thunks
  Itlb multihit:             Not affected
  L1tf:                      Mitigation; PTE Inversion; VMX flush not necessary, SMT disabled
  Mds:                       Mitigation; Clear CPU buffers; SMT Host state unknown
  Meltdown:                  Mitigation; PTI
  Mmio stale data:           Vulnerable: Clear CPU buffers attempted, no microcode; SMT Host state unknown
  Reg file data sampling:    Not affected
  Retbleed:                  Not affected
  Spec rstack overflow:      Not affected
  Spec store bypass:         Mitigation; Speculative Store Bypass disabled via prctl
  Spectre v1:                Mitigation; usercopy/swapgs barriers and __user pointer sanitization
  Spectre v2:                Mitigation; Retpolines; IBPB conditional; IBRS_FW; STIBP disabled; RSB filling; PBRSB-eIBRS Not affected; BHI Retpoline
  Srbds:                     Not affected
  Tsa:                       Not affected
  Tsx async abort:           Mitigation; Clear CPU buffers; SMT Host state unknown
```

## YABS Benchmark

```bash
root@ryzumi-xeon:~# curl -sL https://yabs.sh | bash
# ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## #
#              Yet-Another-Bench-Script              #
#                     v2025-04-20                    #
# https://github.com/masonr/yet-another-bench-script #
# ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## #

Mon Mar  2 05:29:07 AM +08 2026

Basic System Information:
---------------------------------
Uptime     : 0 days, 0 hours, 16 minutes
Processor  : Intel(R) Xeon(R) CPU E5-2699A v4 @ 2.40GHz
CPU cores  : 8 @ 2399.998 MHz
AES-NI     : ✔ Enabled
VM-x/AMD-V : ✔ Enabled
RAM        : 31.3 GiB
Swap       : 128.0 MiB
Disk       : 196.6 GiB
Distro     : Debian GNU/Linux 13 (trixie)
Kernel     : 6.12.41+deb13-amd64
VM Type    : QEMU
IPv4/IPv6  : ✔ Online / ✔ Online

IPv6 Network Information:
---------------------------------
ISP        : Las Vegas NV Datacenter
ASN        : AS26277 ServerPoint.com
Host       : ServerPoint.com
Location   : Singapore, North West (03)
Country    : Singapore

fio Disk Speed Tests (Mixed R/W 50/50) (Partition /dev/vda1):
---------------------------------
Block Size | 4k            (IOPS) | 64k           (IOPS)
  ------   | ---            ----  | ----           ----
Read       | 76.22 MB/s   (19.0k) | 471.41 MB/s   (7.3k)
Write      | 76.42 MB/s   (19.1k) | 473.89 MB/s   (7.4k)
Total      | 152.64 MB/s  (38.1k) | 945.30 MB/s  (14.7k)
           |                      |
Block Size | 512k          (IOPS) | 1m            (IOPS)
  ------   | ---            ----  | ----           ----
Read       | 499.48 MB/s    (975) | 500.75 MB/s    (489)
Write      | 526.02 MB/s   (1.0k) | 534.10 MB/s    (521)
Total      | 1.02 GB/s     (2.0k) | 1.03 GB/s     (1.0k)

iperf3 Network Speed Tests (IPv4):
---------------------------------
Provider        | Location (Link)           | Send Speed      | Recv Speed      | Ping
-----           | -----                     | ----            | ----            | ----
Clouvider       | London, UK (10G)          | 929 Mbits/sec   | 1.28 Gbits/sec  | 160 ms
Eranium         | Amsterdam, NL (100G)      | 797 Mbits/sec   | 1.38 Gbits/sec  | 173 ms
Uztelecom       | Tashkent, UZ (10G)        | 839 Mbits/sec   | 1.57 Gbits/sec  | 258 ms
Leaseweb        | Singapore, SG (10G)       | 1.01 Gbits/sec  | 7.09 Gbits/sec  | 1.16 ms
Clouvider       | Los Angeles, CA, US (10G) | 541 Mbits/sec   | 713 Mbits/sec   | 169 ms
Leaseweb        | NYC, NY, US (10G)         | busy            | 2.89 Gbits/sec  | 311 ms
Edgoo           | Sao Paulo, BR (1G)        | busy            | 46.5 Mbits/sec  | 322 ms

iperf3 Network Speed Tests (IPv6):
---------------------------------
Provider        | Location (Link)           | Send Speed      | Recv Speed      | Ping
-----           | -----                     | ----            | ----            | ----
Clouvider       | London, UK (10G)          | 929 Mbits/sec   | 1.21 Gbits/sec  | 160 ms
Eranium         | Amsterdam, NL (100G)      | 4.34 Gbits/sec  | 1.38 Gbits/sec  | 173 ms
Uztelecom       | Tashkent, UZ (10G)        | 1.01 Gbits/sec  | 1.50 Gbits/sec  | 258 ms
Leaseweb        | Singapore, SG (10G)       | 6.34 Gbits/sec  | 7.29 Gbits/sec  | 1.16 ms
Clouvider       | Los Angeles, CA, US (10G) | 1.04 Gbits/sec  | 733 Mbits/sec   | 169 ms
Leaseweb        | NYC, NY, US (10G)         | busy            | 2.80 Gbits/sec  | 311 ms
Edgoo           | Sao Paulo, BR (1G)        | busy            | 40.5 Mbits/sec  | 325 ms

Geekbench 6 Benchmark Test:
---------------------------------
Test            | Value
                |
Single Core     | 901
Multi Core      | 4242
Full Test       | https://browser.geekbench.com/v6/cpu/16817136

YABS completed in 20 min 23 sec
```

## Bench.Monster Benchmark

```bash
root@ryzumi-xeon:~# curl -sL bench.monster | bash
---------------------------------------------------------------------------
 Region: Global  https://bench.laset.com v1.8.7 2026-02-02
 Usage : curl -sL bench.laset.com | bash -s -- -Global
---------------------------------------------------------------------------
 OS           : Debian GNU/Linux 13 (64 Bit)
 Virt/Kernel  : Qemu / 6.12.41+deb13-amd64
 CPU Model    : Intel(R) Xeon(R) CPU E5-2699A v4 @ 2.40GHz
 CPU Cores    : 8 @ 2399.998 MHz x86_64 16384 KB Cache
 CPU Flags    : AES-NI Enabled & VM-x/AMD-V Enabled
 Load Average : 0.23, 0.56, 0.50
 Total Space  : 197G (1.9G ~2% used)
 Total RAM    : 32102 MB (683 MB + 465 MB Buff in use)
 Total SWAP   : 127 MB (0 MB in use)
 IPv4/IPv6    : ✔ Online / ✔ Online
 Uptime       : 0 days 0:41
---------------------------------------------------------------------------
 Location     : Singapore, Singapore (Central Singapore)
 ASN & ISP    : AS26277, ServerPoint.com / Singapore SG Datacenter
---------------------------------------------------------------------------

 ## Geekbench v6 CPU Benchmark:

  Single Core : 907  (GOOD)
   Multi Core : 4297
    CPU Steal : 0.03%

 ## IO Test

 CPU Speed:
    bzip2     : 95.8 MB/s
   sha256     : 237 MB/s
   md5sum     : 406 MB/s
    Steal     : 0.03%

 RAM Speed:
   Avg. write : 1501.9 MB/s
   Avg. read  : 4539.7 MB/s

 Disk Speed:
   1st run    : 626 MB/s
   2nd run    : 622 MB/s
   3rd run    : 630 MB/s
   -----------------------
   Average    : 626.0 MB/s

 ## Global Speedtest.net

 Location                             Upload      Download       Ping    Loss
-------------------------------------------------------------------------------
 Nearby                          7852.90 Mbps    77.06 Mbps    0.31 ms      0%
-------------------------------------------------------------------------------
 USA, New York (Optimum)          426.18 Mbps   780.46 Mbps  230.99 ms      0%
 USA, Chicago (Uniti)             332.01 Mbps   880.90 Mbps  232.76 ms     N/A
 USA, Los Angeles (Uniti)         522.63 Mbps   878.17 Mbps  173.64 ms     N/A
 UK, London (Hyperoptic)         2954.70 Mbps   979.50 Mbps  151.13 ms     N/A
 Germany, Frankfurt (Plusnet)    2733.94 Mbps   780.46 Mbps  180.69 ms      0%
 India, Mumbai (Tata Play)        471.12 Mbps   779.07 Mbps   49.19 ms   0.83%
 Singapore (MyRepublic)           997.90 Mbps  6694.38 Mbps    1.64 ms      0%
 Japan, Tokyo (Nearoute)         2461.24 Mbps   979.61 Mbps   79.09 ms      0%
 Australia, Sydney (Neptune)      803.52 Mbps   981.81 Mbps   93.35 ms      0%

 ## Statistics

 Total Traffic    : 104.28 GB
 Total Downloaded : 82.36 GB
 Total Uploaded   : 21.92 GB

 Average Loss     : 0.12 %

---------------------------------------------------------------------------
 Finished in : 15 min 14 sec

 Timestamp   : 2026-03-01 22:09:45 GMT
 Saved in    : /root/speedtest.log

 Share results:
 - https://www.speedtest.net/result/c/0bdcc73d-df25-4768-9dc4-28b502334fc1
 - https://browser.geekbench.com/v6/cpu/16817285

root@ryzumi-xeon:~#
```

## Bench.sh Benchmark

```bash
-------------------- A Bench.sh Script By Teddysun -------------------
 Version            : v2026-01-31
 Usage              : wget -qO- bench.sh | bash
----------------------------------------------------------------------
 CPU Model          : Intel(R) Xeon(R) CPU E5-2699A v4 @ 2.40GHz
 CPU Cores          : 8 @ 2399.998 MHz
 CPU Cache          : 16384 KB
 AES-NI             : ✓ Enabled
 VM-x/AMD-V         : ✓ Enabled
 Total Disk         : 196.7 GB (1.9 GB Used)
 Total RAM          : 31.3 GB (513.3 MB Used)
 Total Swap         : 128.0 MB (0 KB Used)
 System Uptime      : 0 days, 0 hour 0 min
 Load Average       : 0.10, 0.03, 0.01
 OS                 : Debian GNU/Linux 13 (trixie)
 Arch               : x86_64 (64 Bit)
 Kernel             : 6.12.41+deb13-amd64
 TCP Congestion Ctrl: bbr
 Virtualization     : QEMU
 IPv4/IPv6          : ✓ Online / ✓ Online
 Organization       : AS26277 ServerPoint.com
 Location           : Singapore / SG
 Region             : Singapore
----------------------------------------------------------------------
 I/O Speed(1st run) : 540 MB/s
 I/O Speed(2nd run) : 662 MB/s
 I/O Speed(3rd run) : 596 MB/s
 I/O Speed(average) : 599.3 MB/s
----------------------------------------------------------------------
 Node Name        Upload Speed      Download Speed      Latency
 Speedtest.net    8070.96 Mbps      77.15 Mbps          0.30 ms
 Los Angeles, US  861.30 Mbps       1071.37 Mbps        183.14 ms
 Dallas, US       1807.45 Mbps      979.01 Mbps         202.17 ms
 Montreal, CA     358.70 Mbps       979.36 Mbps         215.21 ms
 Paris, FR        3043.44 Mbps      882.25 Mbps         161.10 ms
 Amsterdam, NL    518.54 Mbps       782.66 Mbps         172.79 ms
 Suzhou, CN       270.40 Mbps       362.34 Mbps         329.68 ms
 Ningbo, CN       Test faile
 Hong Kong, CN    298.04 Mbps       511.10 Mbps         186.09 ms
 Singapore, SG    7462.10 Mbps      6278.10 Mbps        3.21 ms
 Taipei, CN       4441.01 Mbps      978.36 Mbps         43.21 ms
 Tokyo, JP        2951.01 Mbps      1280.40 Mbps        70.17 ms
----------------------------------------------------------------------
 Finished in        : 7 min 4 sec
 Timestamp          : 2026-03-02 06:42:05 +08
----------------------------------------------------------------------
```

## CPU Steal

```bash
root@ryzumi-xeon:~# mpstat 30 5
Linux 6.12.41+deb13-amd64 (ryzumi-xeon)         03/02/2026      _x86_64_        (8 CPU)

06:45:03 AM  CPU    %usr   %nice    %sys %iowait    %irq   %soft  %steal  %guest  %gnice   %idle
06:45:33 AM  all    0.28    0.00    0.26    0.25    0.00    0.03    0.01    0.00    0.00   99.17
06:46:03 AM  all    0.25    0.00    0.26    0.14    0.00    0.07    0.01    0.00    0.00   99.27
06:46:33 AM  all    0.19    0.00    0.24    0.12    0.00    0.06    0.01    0.00    0.00   99.38
06:47:03 AM  all    0.28    0.00    0.24    0.09    0.00    0.05    0.01    0.00    0.00   99.34
06:47:33 AM  all    0.23    0.00    0.23    0.10    0.00    0.05    0.00    0.00    0.00   99.38
Average:     all    0.25    0.00    0.24    0.14    0.00    0.05    0.01    0.00    0.00   99.31
root@ryzumi-xeon:~#

```