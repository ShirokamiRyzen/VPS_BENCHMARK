# Package Information

```
$12/Month ($11.8 with 10% Recurring disc)

SM25-5 Package:

8 vCPU (Dual Intel Xeon E5-2699 v4)
16 GB RAM DDR4
200 GB NVMe SSD Storage
10 TB Transfer Data @ 1 Gbps
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
root@ryzumi:~# lscpu
Architecture:            x86_64
  CPU op-mode(s):        32-bit, 64-bit
  Address sizes:         46 bits physical, 48 bits virtual
  Byte Order:            Little Endian
CPU(s):                  8
  On-line CPU(s) list:   0-7
Vendor ID:               GenuineIntel
  BIOS Vendor ID:        Red Hat
  Model name:            Intel(R) Xeon(R) CPU E5-2699 v4 @ 2.20GHz
    BIOS Model name:     RHEL 7.6.0 PC (i440FX + PIIX, 1996)  CPU @ 2.0GHz
    BIOS CPU family:     1
    CPU family:          6
    Model:               79
    Thread(s) per core:  1
    Core(s) per socket:  1
    Socket(s):           8
    Stepping:            1
    BogoMIPS:            4399.99
    Flags:               fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush mmx fxsr sse sse2 ss syscall nx pdpe1gb rdtscp lm constant_tsc arch_perfmon rep_good nopl xt
                         opology cpuid tsc_known_freq pni pclmulqdq vmx ssse3 fma cx16 pdcm pcid sse4_1 sse4_2 x2apic movbe popcnt tsc_deadline_timer aes xsave avx f16c rdrand hypervisor lahf_lm ab
                         m 3dnowprefetch cpuid_fault invpcid_single pti ssbd ibrs ibpb stibp tpr_shadow vnmi flexpriority ept vpid ept_ad fsgsbase tsc_adjust bmi1 hle avx2 smep bmi2 erms invpcid rt
                         m rdseed adx smap xsaveopt arat umip md_clear flush_l1d arch_capabilities
Virtualization features:
  Virtualization:        VT-x
  Hypervisor vendor:     KVM
  Virtualization type:   full
Caches (sum of all):
  L1d:                   256 KiB (8 instances)
  L1i:                   256 KiB (8 instances)
  L2:                    32 MiB (8 instances)
  L3:                    128 MiB (8 instances)
NUMA:
  NUMA node(s):          1
  NUMA node0 CPU(s):     0-7
Vulnerabilities:
  Itlb multihit:         Not affected
  L1tf:                  Mitigation; PTE Inversion; VMX flush not necessary, SMT disabled
  Mds:                   Mitigation; Clear CPU buffers; SMT Host state unknown
  Meltdown:              Mitigation; PTI
  Mmio stale data:       Mitigation; Clear CPU buffers; SMT Host state unknown
  Retbleed:              Not affected
  Spec store bypass:     Mitigation; Speculative Store Bypass disabled via prctl
  Spectre v1:            Mitigation; usercopy/swapgs barriers and __user pointer sanitization
  Spectre v2:            Mitigation; Retpolines, IBPB conditional, IBRS_FW, STIBP disabled, RSB filling, PBRSB-eIBRS Not affected
  Srbds:                 Not affected
  Tsx async abort:       Mitigation; Clear CPU buffers; SMT Host state unknown
```

## YABS Benchmark

```bash
root@ryzumi:~# curl -sL https://yabs.sh | bash
# ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## #
#              Yet-Another-Bench-Script              #
#                     v2025-04-20                    #
# https://github.com/masonr/yet-another-bench-script #
# ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## #

Wed Jul  2 11:53:54 AM UTC 2025

Basic System Information:
---------------------------------
Uptime     : 8 days, 2 hours, 35 minutes
Processor  : Intel(R) Xeon(R) CPU E5-2699 v4 @ 2.20GHz
CPU cores  : 8 @ 2199.996 MHz
AES-NI     : ✔ Enabled
VM-x/AMD-V : ✔ Enabled
RAM        : 15.6 GiB
Swap       : 0.0 KiB
Disk       : 199.9 GiB
Distro     : Debian GNU/Linux 12 (bookworm)
Kernel     : 6.1.0-9-amd64
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
Read       | 164.23 MB/s  (41.0k) | 1.26 GB/s    (19.6k)
Write      | 164.67 MB/s  (41.1k) | 1.26 GB/s    (19.7k)
Total      | 328.91 MB/s  (82.2k) | 2.52 GB/s    (39.4k)
           |                      |
Block Size | 512k          (IOPS) | 1m            (IOPS)
  ------   | ---            ----  | ----           ----
Read       | 1.32 GB/s     (2.5k) | 1.31 GB/s     (1.2k)
Write      | 1.39 GB/s     (2.7k) | 1.40 GB/s     (1.3k)
Total      | 2.72 GB/s     (5.3k) | 2.72 GB/s     (2.6k)

iperf3 Network Speed Tests (IPv4):
---------------------------------
Provider        | Location (Link)           | Send Speed      | Recv Speed      | Ping
-----           | -----                     | ----            | ----            | ----
Clouvider       | London, UK (10G)          | 277 Mbits/sec   | 666 Mbits/sec   | 155 ms
Eranium         | Amsterdam, NL (100G)      | 722 Mbits/sec   | 804 Mbits/sec   | 154 ms
Uztelecom       | Tashkent, UZ (10G)        | 706 Mbits/sec   | 197 Mbits/sec   | 236 ms
Leaseweb        | Singapore, SG (10G)       | 847 Mbits/sec   | 305 Mbits/sec   | 2.58 ms
Clouvider       | Los Angeles, CA, US (10G) | 567 Mbits/sec   | 118 Mbits/sec   | 203 ms
Leaseweb        | NYC, NY, US (10G)         | 570 Mbits/sec   | 258 Mbits/sec   | 235 ms
Edgoo           | Sao Paulo, BR (1G)        | 244 Mbits/sec   | 383 Mbits/sec   | 315 ms

iperf3 Network Speed Tests (IPv6):
---------------------------------
Provider        | Location (Link)           | Send Speed      | Recv Speed      | Ping
-----           | -----                     | ----            | ----            | ----
Clouvider       | London, UK (10G)          | 548 Mbits/sec   | 557 Mbits/sec   | 155 ms
Eranium         | Amsterdam, NL (100G)      | 698 Mbits/sec   | 780 Mbits/sec   | 156 ms
Uztelecom       | Tashkent, UZ (10G)        | 591 Mbits/sec   | 702 Mbits/sec   | 237 ms
Leaseweb        | Singapore, SG (10G)       | 841 Mbits/sec   | 865 Mbits/sec   | 2.10 ms
Clouvider       | Los Angeles, CA, US (10G) | 560 Mbits/sec   | 477 Mbits/sec   | 203 ms
Leaseweb        | NYC, NY, US (10G)         | 552 Mbits/sec   | 593 Mbits/sec   | 234 ms
Edgoo           | Sao Paulo, BR (1G)        | 516 Mbits/sec   | 583 Mbits/sec   | 314 ms

Geekbench 6 Benchmark Test:
---------------------------------
Test            | Value
                |
Single Core     | 884
Multi Core      | 4744
Full Test       | https://browser.geekbench.com/v6/cpu/12689176

YABS completed in 14 min 56 sec
```

## Bench.Monster Benchmark

```bash
root@ryzumi:~# curl -sL bench.monster | bash
---------------------------------------------------------------------------
 Region: Global  https://bench.monster v1.7.4 2023-12-15
 Usage : curl -sL bench.monster | bash -s -- -Global
---------------------------------------------------------------------------
 OS           : Debian GNU/Linux 12 (64 Bit)
 Virt/Kernel  : Dedicated / 6.1.0-9-amd64
 CPU Model    : Intel(R) Xeon(R) CPU E5-2699 v4 @ 2.20GHz
 CPU Cores    : 8 @ 2199.996 MHz x86_64 16384 KB Cache
 CPU Flags    : AES-NI Enabled & VM-x/AMD-V Enabled
 Load Average : 0.42, 0.99, 0.58
 Total Space  : 200G (5.1G ~3% used)
 Total RAM    : 15992 MB (844 MB + 2993 MB Buff in use)
 Total SWAP   : 0 MB (0 MB in use)
 IPv4/IPv6    : ✔ Online / ✔ Online
 Uptime       : 8 days 2:51
---------------------------------------------------------------------------
 Location     : Singapore, Singapore (North West)
 ASN & ISP    : AS134677, Dromatics Systems Pte Ltd / Dromatics Systems Pte Ltd
---------------------------------------------------------------------------

 ## Geekbench v6 CPU Benchmark:

  Single Core : 908  (GOOD)
   Multi Core : 4730

 ## IO Test

 CPU Speed:
    bzip2     :  99.6 MB/s
   sha256     : 161 MB/s
   md5sum     : 444 MB/s

 RAM Speed:
   Avg. write : 1809.1 MB/s
   Avg. read  : 3891.2 MB/s

 Disk Speed:
   1st run    : 995 MB/s
   2nd run    : 987 MB/s
   3rd run    : 1.1 GB/s
   -----------------------
   Average    : 1036.1 MB/s

 ## Global Speedtest.net

 Location                       Upload           Download         Ping
---------------------------------------------------------------------------
 Nearby                         368.55 Mbit/s    305.04 Mbit/s    4.318 ms
---------------------------------------------------------------------------
 USA, New York (Starry)         56.46 Mbit/s     13.98 Mbit/s    226.929 ms
 USA, Chicago (Windstream)      86.95 Mbit/s     44.43 Mbit/s    189.122 ms
 USA, Houston (Comcast)         35.04 Mbit/s     100.89 Mbit/s   199.642 ms
 USA, Los Angeles (Windstream)  86.21 Mbit/s     30.28 Mbit/s    202.031 ms
 UK, London (toob Ltd)          109.67 Mbit/s    173.80 Mbit/s   172.363 ms
 Germany, Berlin (DNS:NET)      17.55 Mbit/s     100.13 Mbit/s   257.168 ms
 Spain, Madrid (MasMovil)       117.06 Mbit/s    119.56 Mbit/s   152.861 ms
 Italy, Rome (Unidata)          97.89 Mbit/s     54.97 Mbit/s    167.290 ms
 India, Mumbai (Tatasky)        78.68 Mbit/s     120.80 Mbit/s   183.183 ms
 Singapore (StarHub)            796.16 Mbit/s    272.88 Mbit/s   1.770 ms
 Japan, Tsukuba (SoftEther)     8.42 Mbit/s      1.61 Mbit/s     458.289 ms
ping: s1.speedtest.syd.optusnet.com.au: Name or service not known
---------------------------------------------------------------------------

 Finished in : 18 min 9 sec
 Timestamp   : 2025-07-02 12:28:37 GMT
 Saved in    : /root/speedtest.log

 Share results:
 - https://www.speedtest.net/result/17924637265.png
 - https://browser.geekbench.com/v6/cpu/12689325
```

## Bench.sh Benchmark

```bash
-------------------- A Bench.sh Script By Teddysun -------------------
 Version            : v2025-05-08
 Usage              : wget -qO- bench.sh | bash
----------------------------------------------------------------------
 CPU Model          : Intel(R) Xeon(R) CPU E5-2699 v4 @ 2.20GHz
 CPU Cores          : 8 @ 2199.996 MHz
 CPU Cache          : 16384 KB
 AES-NI             : ✓ Enabled
 VM-x/AMD-V         : ✓ Enabled
 Total Disk         : 199.9 GB (5.0 GB Used)
 Total Mem          : 15.6 GB (850.1 MB Used)
 System uptime      : 8 days, 3 hour 11 min
 Load average       : 0.03, 0.28, 0.52
 OS                 : Debian GNU/Linux 12
 Arch               : x86_64 (64 Bit)
 Kernel             : 6.1.0-9-amd64
 TCP CC             : bbr
 Virtualization     : KVM
 IPv4/IPv6          : ✓ Online / ✓ Online
 Organization       : AS134677 Dromatics Systems Pte Ltd
 Location           : Singapore / SG
 Region             : Singapore
----------------------------------------------------------------------
 I/O Speed(1st run) : 982 MB/s
 I/O Speed(2nd run) : 1.1 GB/s
 I/O Speed(3rd run) : 1.1 GB/s
 I/O Speed(average) : 1078.3 MB/s
----------------------------------------------------------------------
 Node Name        Upload Speed      Download Speed      Latency
 Speedtest.net    812.63 Mbps       334.52 Mbps         1.34 ms
 Paris, FR        744.26 Mbps       926.26 Mbps         147.66 ms
 Amsterdam, NL    547.35 Mbps       294.18 Mbps         163.20 ms
 Hong Kong, CN    788.97 Mbps       327.28 Mbps         34.00 ms
 Singapore, SG    826.44 Mbps       367.81 Mbps         90.69 ms
 Tokyo, JP        804.26 Mbps       879.93 Mbps         68.91 ms
----------------------------------------------------------------------
 Finished in        : 2 min 56 sec
 Timestamp          : 2025-07-02 12:33:23 UTC
----------------------------------------------------------------------
```

## CPU Steal

```bash
root@ryzumi:~# mpstat 30 5
Linux 6.1.0-9-amd64 (ryzumi)    07/02/2025      _x86_64_        (8 CPU)

11:50:10 AM  CPU    %usr   %nice    %sys %iowait    %irq   %soft  %steal  %guest  %gnice   %idle
11:50:40 AM  all    0.40    0.00    0.18    0.00    0.00    0.01    0.00    0.00    0.00   99.41
11:51:10 AM  all    0.42    0.00    0.17    0.00    0.00    0.02    0.00    0.00    0.00   99.39
11:51:40 AM  all    0.45    0.00    0.15    0.00    0.00    0.00    0.00    0.00    0.00   99.39
11:52:10 AM  all    0.39    0.00    0.18    0.00    0.00    0.02    0.00    0.00    0.00   99.41
11:52:40 AM  all    0.46    0.00    0.20    0.00    0.00    0.01    0.00    0.00    0.00   99.32
Average:     all    0.42    0.00    0.18    0.00    0.00    0.01    0.00    0.00    0.00   99.38
root@ryzumi:~#

```