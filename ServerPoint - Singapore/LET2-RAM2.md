# Package Information

```
ServerPoint XEON E5v4 deals 2025

LET2-RAM2 Package:

6 vCPUs, Intel E5v4 at 2.1Ghz
16 GBs of RAM
150 GBs SSD storage
15.000 GBs/mo data transfer
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
CPU(s):                      6
  On-line CPU(s) list:       0-5
Vendor ID:                   GenuineIntel
  Model name:                Intel(R) Xeon(R) CPU E5-2699A v4 @ 2.40GHz
    CPU family:              6
    Model:                   79
    Thread(s) per core:      1
    Core(s) per socket:      6
    Socket(s):               1
    Stepping:                1
    BogoMIPS:                4799.97
    Flags:                   fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush mmx fxsr sse sse2 ss ht syscall nx pdpe1gb rdtscp lm constant_tsc arch_perfmon rep_good no
                             pl xtopology cpuid tsc_known_freq pni pclmulqdq vmx ssse3 fma cx16 pdcm pcid sse4_1 sse4_2 x2apic movbe popcnt tsc_deadline_timer aes xsave avx f16c rdrand hypervisor lah
                             f_lm abm 3dnowprefetch cpuid_fault pti ssbd ibrs ibpb stibp tpr_shadow flexpriority ept vpid ept_ad fsgsbase tsc_adjust bmi1 hle avx2 smep bmi2 erms invpcid rtm rdseed ad
                             x smap xsaveopt arat vnmi umip md_clear arch_capabilities
Virtualization features:
  Virtualization:            VT-x
  Hypervisor vendor:         Microsoft
  Virtualization type:       full
Caches (sum of all):
  L1d:                       192 KiB (6 instances)
  L1i:                       192 KiB (6 instances)
  L2:                        24 MiB (6 instances)
  L3:                        16 MiB (1 instance)
NUMA:
  NUMA node(s):              1
  NUMA node0 CPU(s):         0-5
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
#                     v2026-04-29                    #
# https://github.com/masonr/yet-another-bench-script #
# ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## #

Thu Apr 30 05:06:40 PM WIB 2026

Basic System Information:
---------------------------------
Uptime     : 0 days, 3 hours, 54 minutes
Processor  : Intel(R) Xeon(R) CPU E5-2699A v4 @ 2.40GHz
CPU cores  : 6 @ 2399.988 MHz
AES-NI     : ✔ Enabled
VM-x/AMD-V : ✔ Enabled
RAM        : 15.6 GiB
Swap       : 128.0 MiB
Disk       : 147.3 GiB
Distro     : Debian GNU/Linux 13 (trixie)
Kernel     : 6.12.41+deb13-amd64
VM Type    : QEMU
IPv4/IPv6  : ✔ Online / ❌ Offline

IPv4 Network Information:
---------------------------------
ISP        : ServerPoint.com
ASN        : AS26277 ServerPoint.com
Host       : Singapore SG Datacenter
Location   : Singapore, Central Singapore (01)
Country    : Singapore

fio Disk Speed Tests (Mixed R/W 50/50) (Partition /dev/vda1):
---------------------------------
Block Size | 4k            (IOPS) | 64k           (IOPS)
  ------   | ---            ----  | ----           ----
Read       | 32.07 MB/s    (8.0k) | 302.17 MB/s   (4.7k)
Write      | 32.12 MB/s    (8.0k) | 303.76 MB/s   (4.7k)
Total      | 64.19 MB/s   (16.0k) | 605.93 MB/s   (9.4k)
           |                      |
Block Size | 512k          (IOPS) | 1m            (IOPS)
  ------   | ---            ----  | ----           ----
Read       | 423.21 MB/s    (826) | 302.69 MB/s    (295)
Write      | 445.70 MB/s    (870) | 322.85 MB/s    (315)
Total      | 868.92 MB/s   (1.6k) | 625.54 MB/s    (610)

iperf3 Network Speed Tests (IPv4):
---------------------------------
Provider        | Location (Link)           | Send Speed      | Recv Speed      | Ping
-----           | -----                     | ----            | ----            | ----
Clouvider       | London, UK (10G)          | 753 Mbits/sec   | 1.09 Gbits/sec  | 160 ms
Eranium         | Amsterdam, NL (100G)      | 737 Mbits/sec   | 4.70 Gbits/sec  | 231 ms
Uztelecom       | Tashkent, UZ (10G)        | 850 Mbits/sec   | 376 Mbits/sec   | 176 ms
Leaseweb        | Singapore, SG (10G)       | 597 Mbits/sec   | 1.64 Gbits/sec  | --
Clouvider       | Los Angeles, CA, US (10G) | 665 Mbits/sec   | 1.22 Gbits/sec  | 162 ms
Leaseweb        | NYC, NY, US (10G)         | busy            | 3.18 Gbits/sec  | 238 ms
Edgoo           | Sao Paulo, BR (1G)        | busy            | 2.44 Gbits/sec  | 334 ms

Geekbench 6 Benchmark Test:
---------------------------------
Test            | Value
                |
Single Core     | 722
Multi Core      | 3067
Full Test       | https://browser.geekbench.com/v6/cpu/17827916

YABS completed in 15 min 7 sec
```

## Bench.Monster Benchmark

```bash
root@ryzumi-xeon:~# curl -sL bench.monster | bash
---------------------------------------------------------------------------
 Region: Global  https://bench.laset.com v1.8.7 2026-02-02
 Usage : curl -sL bench.laset.com | bash -s -- -Global
---------------------------------------------------------------------------
 OS           : Debian GNU/Linux 13 (64 Bit)
 Virt/Kernel  : Qemu / 6.12.74+deb13+1-amd64
 CPU Model    : Intel(R) Xeon(R) CPU E5-2699A v4 @ 2.40GHz
 CPU Cores    : 6 @ 2399.988 MHz x86_64 16384 KB Cache
 CPU Flags    : AES-NI Enabled & VM-x/AMD-V Enabled
 Load Average : 0.21, 0.06, 0.02
 Total Space  : 148G (3.4G ~3% used)
 Total RAM    : 15998 MB (665 MB + 775 MB Buff in use)
 Total SWAP   : 127 MB (0 MB in use)
 IPv4/IPv6    : ✔ Online / ❌ Offline
 Uptime       : 0 days 0:32
---------------------------------------------------------------------------
 Location     : Singapore, Singapore (Central Singapore)
 ASN & ISP    : AS26277, ServerPoint.com / Singapore SG Datacenter
---------------------------------------------------------------------------

 ## Geekbench v6 CPU Benchmark:

  Single Core : 802  (GOOD)
   Multi Core : 3121
    CPU Steal : 0.03%

 ## IO Test

 CPU Speed:
    bzip2     : 71.9 MB/s
   sha256     : 210 MB/s
   md5sum     : 345 MB/s
    Steal     : 0.11%

 RAM Speed:
   Avg. write : 1365.3 MB/s
   Avg. read  : 4130.1 MB/s

 Disk Speed:
   1st run    : 553 MB/s
   2nd run    : 554 MB/s
   3rd run    : 565 MB/s
   -----------------------
   Average    : 557.3 MB/s

 ## Global Speedtest.net

 Location                             Upload      Download       Ping    Loss
-------------------------------------------------------------------------------
 Nearby                           550.73 Mbps  7054.15 Mbps    0.72 ms      0%
-------------------------------------------------------------------------------
 USA, Chicago (Uniti)             382.75 Mbps  1158.50 Mbps  221.07 ms     N/A
 UK, London (Hyperoptic)          505.70 Mbps  1427.33 Mbps  170.55 ms     N/A
 Germany, Frankfurt (Plusnet)     939.12 Mbps  5938.05 Mbps  176.08 ms      0%
 India, Mumbai (Tata Play)        537.74 Mbps  6697.13 Mbps   56.95 ms      0%
 Singapore (MyRepublic)           998.60 Mbps  7106.07 Mbps    1.59 ms      0%
 Japan, Tokyo (Nearoute)          422.99 Mbps  1762.52 Mbps   69.17 ms   2.17%
 Australia, Sydney (Neptune)      696.11 Mbps  1639.11 Mbps   93.29 ms      0%
 Brazil, Sao Paulo (TIM)           95.12 Mbps   901.19 Mbps  350.80 ms      0%

 ## Statistics

 Total Traffic    : 45.11 GB
 Total Downloaded : 38.53 GB
 Total Uploaded   : 6.58 GB

 Average Loss     : 0.31 %

---------------------------------------------------------------------------
 Finished in : 16 min 37 sec

 Timestamp   : 2026-04-30 11:32:44 GMT
 Saved in    : /root/speedtest.log

 Share results:
 -
https://www.speedtest.net/result/c/5429bacf-99e5-4167-9002-e6dc9a823298
 -

root@ryzumi-xeon:~#
```

## Bench.sh Benchmark

```bash
-------------------- A Bench.sh Script By Teddysun -------------------
 Version            : v2026-01-31
 Usage              : wget -qO- bench.sh | bash
----------------------------------------------------------------------
 CPU Model          : Intel(R) Xeon(R) CPU E5-2699A v4 @ 2.40GHz
 CPU Cores          : 6 @ 2399.988 MHz
 CPU Cache          : 16384 KB
 AES-NI             : ✓ Enabled
 VM-x/AMD-V         : ✓ Enabled
 Total Disk         : 147.5 GB (3.1 GB Used)
 Total RAM          : 15.6 GB (571.1 MB Used)
 Total Swap         : 128.0 MB (0 KB Used)
 System Uptime      : 0 days, 4 hour 14 min
 Load Average       : 0.04, 0.61, 0.62
 OS                 : Debian GNU/Linux 13 (trixie)
 Arch               : x86_64 (64 Bit)
 Kernel             : 6.12.41+deb13-amd64
 TCP Congestion Ctrl: bbr
 Virtualization     : QEMU
 IPv4/IPv6          : ✓ Online / ✗ Offline
 Organization       : AS26277 ServerPoint.com
 Location           : Singapore / SG
 Region             : Singapore
----------------------------------------------------------------------
 I/O Speed(1st run) : 563 MB/s
 I/O Speed(2nd run) : 549 MB/s
 I/O Speed(3rd run) : 583 MB/s
 I/O Speed(average) : 565.0 MB/s
----------------------------------------------------------------------
 Node Name        Upload Speed      Download Speed      Latency
 Speedtest.net    1001.99 Mbps      7123.17 Mbps        0.46 ms
 Los Angeles, US  928.36 Mbps       6023.20 Mbps        164.39 ms
 Dallas, US       831.53 Mbps       953.97 Mbps         201.05 ms
 Montreal, CA     Test failed
 Paris, FR        863.45 Mbps       6738.95 Mbps        168.50 ms
 Amsterdam, NL    Test failed
 Suzhou, CN       91.31 Mbps        756.74 Mbps         344.12 ms
 Ningbo, CN       3.22 Mbps         723.04 Mbps         324.01 ms
 Hong Kong, CN    349.25 Mbps       1563.91 Mbps        33.28 ms
 Singapore, SG    999.18 Mbps       7196.74 Mbps        1.40 ms
 Taipei, CN       994.33 Mbps       7182.69 Mbps        43.23 ms
 Tokyo, JP        816.13 Mbps       2057.19 Mbps        67.56 ms
----------------------------------------------------------------------
 Finished in        : 6 min 39 sec
 Timestamp          : 2026-04-30 17:33:24 WIB
----------------------------------------------------------------------
```

## CPU Steal

```bash
root@ryzumi-xeon:~# mpstat 30 5
Linux 6.12.41+deb13-amd64 (ryzumi-xeon)         04/30/2026      _x86_64_        (6 CPU)

04:53:00 PM  CPU    %usr   %nice    %sys %iowait    %irq   %soft  %steal  %guest  %gnice   %idle
04:53:30 PM  all    0.13    0.00    0.24    0.03    0.00    0.04    0.03    0.00    0.00   99.52
04:54:00 PM  all    0.11    0.00    0.23    0.09    0.00    0.06    0.03    0.00    0.00   99.48
04:54:30 PM  all    0.09    0.00    0.24    0.03    0.00    0.09    0.02    0.00    0.00   99.52
04:55:00 PM  all    0.10    0.00    0.23    0.10    0.00    0.07    0.03    0.00    0.00   99.47
04:55:30 PM  all    0.53    0.00    1.06    0.31    0.00    0.10    1.83    0.00    0.00   96.16
Average:     all    0.19    0.00    0.40    0.11    0.00    0.07    0.39    0.00    0.00   98.82
root@ryzumi-xeon:~#
```