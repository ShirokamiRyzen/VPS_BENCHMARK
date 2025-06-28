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
root@ryzumi:~# curl -sL https://yabs.sh | bash -s -- -r
# ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## #
#              Yet-Another-Bench-Script              #
#                     v2025-04-20                    #
# https://github.com/masonr/yet-another-bench-script #
# ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## #

Fri Jun 27 06:50:13 AM UTC 2025

Basic System Information:
---------------------------------
Uptime     : 2 days, 21 hours, 31 minutes
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
Read       | 160.94 MB/s  (40.2k) | 1.28 GB/s    (20.1k)
Write      | 161.37 MB/s  (40.3k) | 1.29 GB/s    (20.2k)
Total      | 322.31 MB/s  (80.5k) | 2.58 GB/s    (40.4k)
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
Clouvider       | London, UK (10G)          | 317 Mbits/sec   | 783 Mbits/sec   | 155 ms
Leaseweb        | Singapore, SG (10G)       | 825 Mbits/sec   | 300 Mbits/sec   | 2.14 ms
Leaseweb        | NYC, NY, US (10G)         | 611 Mbits/sec   | 191 Mbits/sec   | 217 ms

iperf3 Network Speed Tests (IPv6):
---------------------------------
Provider        | Location (Link)           | Send Speed      | Recv Speed      | Ping
-----           | -----                     | ----            | ----            | ----
Clouvider       | London, UK (10G)          | 528 Mbits/sec   | 764 Mbits/sec   | 155 ms
Leaseweb        | Singapore, SG (10G)       | 805 Mbits/sec   | 882 Mbits/sec   | 90.3 ms
Leaseweb        | NYC, NY, US (10G)         | 595 Mbits/sec   | 751 Mbits/sec   | 217 ms

Geekbench 6 Benchmark Test:
---------------------------------
Test            | Value
                |
Single Core     | 918
Multi Core      | 4700
Full Test       | https://browser.geekbench.com/v6/cpu/12617265

YABS completed in 10 min 58 sec
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
 Load Average : 0.04, 0.20, 0.32
 Total Space  : 200G (4.6G ~3% used)
 Total RAM    : 15992 MB (677 MB + 2355 MB Buff in use)
 Total SWAP   : 0 MB (0 MB in use)
 IPv4/IPv6    : ✔ Online / ✔ Online
 Uptime       : 2 days 21:52
---------------------------------------------------------------------------
 Location     : Singapore, Singapore (North West)
 ASN & ISP    : AS134677, Dromatics Systems Pte Ltd / Dromatics Systems Pte Ltd
---------------------------------------------------------------------------

 ## Geekbench v6 CPU Benchmark:

  Single Core : 885  (GOOD)
   Multi Core : 4783

 ## IO Test

 CPU Speed:
    bzip2     : 101 MB/s
   sha256     : 163 MB/s
   md5sum     : 426 MB/s

 RAM Speed:
   Avg. write : 1843.2 MB/s
   Avg. read  : 3788.8 MB/s

 Disk Speed:
   1st run    : 1.1 GB/s
   2nd run    : 1.1 GB/s
   3rd run    : 1.1 GB/s
   -----------------------
   Average    : 1126.4 MB/s

 ## Global Speedtest.net

 Location                       Upload           Download         Ping
---------------------------------------------------------------------------
 Nearby                         367.67 Mbit/s    576.96 Mbit/s    7.519 ms
---------------------------------------------------------------------------
 USA, New York (Starry)         22.94 Mbit/s     6.05 Mbit/s     ping error!
 USA, Chicago (Windstream)      74.68 Mbit/s     91.90 Mbit/s    189.277 ms
 USA, Houston (Comcast)         53.30 Mbit/s     93.15 Mbit/s    199.397 ms
 USA, Los Angeles (Windstream)  102.27 Mbit/s    231.60 Mbit/s   173.733 ms
 UK, London (toob Ltd)          109.60 Mbit/s    137.46 Mbit/s   170.647 ms
 Germany, Berlin (DNS:NET)      18.87 Mbit/s     4.44 Mbit/s     249.163 ms
 Spain, Madrid (MasMovil)       119.24 Mbit/s    16.43 Mbit/s    149.606 ms
 Italy, Rome (Unidata)          94.79 Mbit/s     165.61 Mbit/s   169.225 ms
 India, Mumbai (Tatasky)        4.13 Mbit/s      0.46 Mbit/s     293.132 ms
 Singapore (StarHub)            819.72 Mbit/s    193.39 Mbit/s   1.883 ms
 Japan, Tsukuba (SoftEther)     12.74 Mbit/s     3.01 Mbit/s     198.065 ms
ping: s1.speedtest.syd.optusnet.com.au: Name or service not known
---------------------------------------------------------------------------

 Finished in : 17 min 54 sec
 Timestamp   : 2025-06-27 07:28:55 GMT
 Saved in    : /root/speedtest.log

 Share results:
 - https://www.speedtest.net/result/17903881761.png
 - https://browser.geekbench.com/v6/cpu/12617432
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
 Total Disk         : 199.9 GB (4.6 GB Used)
 Total Mem          : 15.6 GB (675.0 MB Used)
 System uptime      : 2 days, 21 hour 47 min
 Load average       : 0.00, 0.42, 0.41
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
 I/O Speed(1st run) : 956 MB/s
 I/O Speed(2nd run) : 1.0 GB/s
 I/O Speed(3rd run) : 1.1 GB/s
 I/O Speed(average) : 1035.5 MB/s
----------------------------------------------------------------------
 Node Name        Upload Speed      Download Speed      Latency
 Speedtest.net    767.01 Mbps       857.92 Mbps         1.31 ms
 Paris, FR        780.29 Mbps       750.23 Mbps         146.09 ms
 Amsterdam, NL    620.36 Mbps       275.61 Mbps         162.54 ms
 Shanghai, CN     334.79 Mbps       218.85 Mbps         90.46 ms
 Hong Kong, CN    801.52 Mbps       237.93 Mbps         32.82 ms
 Singapore, SG    872.13 Mbps       378.20 Mbps         80.79 ms
 Tokyo, JP        744.86 Mbps       879.87 Mbps         68.89 ms
----------------------------------------------------------------------
 Finished in        : 3 min 22 sec
 Timestamp          : 2025-06-27 07:10:03 UTC
----------------------------------------------------------------------
root@ryzumi:~#
```

## CPU Steal

```bash
root@ryzumi:~# mpstat 1
Linux 6.1.0-9-amd64 (ryzumi)    06/27/2025      _x86_64_        (8 CPU)

07:05:47 AM  CPU    %usr   %nice    %sys %iowait    %irq   %soft  %steal  %guest  %gnice   %idle
07:05:48 AM  all    0.12    0.00    0.12    0.00    0.00    0.00    0.00    0.00    0.00   99.75
07:05:49 AM  all    0.25    0.00    0.00    0.00    0.00    0.00    0.00    0.00    0.00   99.75
07:05:50 AM  all    0.00    0.00    0.00    0.00    0.00    0.00    0.00    0.00    0.00  100.00
07:05:51 AM  all    0.00    0.00    0.12    0.00    0.00    0.00    0.00    0.00    0.00   99.88
07:05:52 AM  all    0.12    0.00    0.12    0.00    0.00    0.00    0.00    0.00    0.00   99.75
07:05:53 AM  all    0.00    0.00    0.13    0.00    0.00    0.00    0.00    0.00    0.00   99.87
07:05:54 AM  all    0.13    0.00    0.13    0.00    0.00    0.00    0.00    0.00    0.00   99.75
07:05:55 AM  all    0.12    0.00    0.25    0.00    0.00    0.00    0.00    0.00    0.00   99.63
07:05:56 AM  all    0.12    0.00    0.25    0.00    0.00    0.00    0.00    0.00    0.00   99.63
07:05:57 AM  all    0.13    0.00    0.13    0.00    0.00    0.00    0.00    0.00    0.00   99.75
Average:     all    0.10    0.00    0.12    0.00    0.00    0.00    0.00    0.00    0.00   99.78
root@ryzumi:~#

```