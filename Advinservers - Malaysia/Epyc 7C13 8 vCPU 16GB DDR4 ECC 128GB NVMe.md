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
Architecture:                x86_64
  CPU op-mode(s):            32-bit, 64-bit
  Address sizes:             48 bits physical, 48 bits virtual
  Byte Order:                Little Endian
CPU(s):                      8
  On-line CPU(s) list:       0-7
Vendor ID:                   AuthenticAMD
  BIOS Vendor ID:            QEMU
  Model name:                AMD EPYC 7C13 64-Core Processor
    BIOS Model name:         pc-i440fx-9.2  CPU @ 2.0GHz
    BIOS CPU family:         1
    CPU family:              25
    Model:                   1
    Thread(s) per core:      1
    Core(s) per socket:      8
    Socket(s):               1
    Stepping:                1
    BogoMIPS:                3999.99
    Flags:                   fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush mmx fxsr sse sse2 ht syscall nx mmxext fxsr_opt pdpe1gb rdtscp lm rep_good nopl cpuid
                             extd_apicid tsc_known_freq pni pclmulqdq ssse3 fma cx16 pcid sse4_1 sse4_2 x2apic movbe popcnt tsc_deadline_timer aes xsave avx f16c rdrand hypervisor lahf_lm cmp_leg
                             acy svm cr8_legacy abm sse4a misalignsse 3dnowprefetch osvw perfctr_core invpcid_single ssbd ibrs ibpb stibp vmmcall fsgsbase tsc_adjust bmi1 avx2 smep bmi2 erms invp
                             cid rdseed adx smap clflushopt clwb sha_ni xsaveopt xsavec xgetbv1 xsaves clzero xsaveerptr wbnoinvd arat npt lbrv nrip_save tsc_scale vmcb_clean flushbyasid pausefil
                             ter pfthreshold v_vmsave_vmload vgif umip pku ospke vaes vpclmulqdq rdpid overflow_recov succor fsrm arch_capabilities
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
  Spec rstack overflow:      Mitigation; safe RET
  Spec store bypass:         Mitigation; Speculative Store Bypass disabled via prctl
  Spectre v1:                Mitigation; usercopy/swapgs barriers and __user pointer sanitization
  Spectre v2:                Mitigation; Retpolines; IBPB conditional; IBRS_FW; STIBP disabled; RSB filling; PBRSB-eIBRS Not affected; BHI Not affected
  Srbds:                     Not affected
  Tsx async abort:           Not affected
```

## YABS Benchmark

```bash
root@ryzumi:~# curl -sL https://yabs.sh | bash
# ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## #
#              Yet-Another-Bench-Script              #
#                     v2025-04-20                    #
# https://github.com/masonr/yet-another-bench-script #
# ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## #

Tue Jul 22 01:53:12 AM UTC 2025

Basic System Information:
---------------------------------
Uptime     : 0 days, 0 hours, 15 minutes
Processor  : AMD EPYC 7C13 64-Core Processor
CPU cores  : 8 @ 1999.997 MHz
AES-NI     : ✔ Enabled
VM-x/AMD-V : ✔ Enabled
RAM        : 15.6 GiB
Swap       : 0.0 KiB
Disk       : 118.1 GiB
Distro     : Debian GNU/Linux 12 (bookworm)
Kernel     : 6.1.0-37-amd64
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
Block Size | 4k            (IOPS) | 64k           (IOPS)
  ------   | ---            ----  | ----           ----
Read       | 160.04 MB/s  (40.0k) | 1.62 GB/s    (25.4k)
Write      | 160.47 MB/s  (40.1k) | 1.63 GB/s    (25.5k)
Total      | 320.51 MB/s  (80.1k) | 3.26 GB/s    (50.9k)
           |                      |
Block Size | 512k          (IOPS) | 1m            (IOPS)
  ------   | ---            ----  | ----           ----
Read       | 4.58 GB/s     (8.9k) | 4.95 GB/s     (4.8k)
Write      | 4.82 GB/s     (9.4k) | 5.27 GB/s     (5.1k)
Total      | 9.40 GB/s    (18.3k) | 10.23 GB/s    (9.9k)

iperf3 Network Speed Tests (IPv4):
---------------------------------
Provider        | Location (Link)           | Send Speed      | Recv Speed      | Ping
-----           | -----                     | ----            | ----            | ----
Clouvider       | London, UK (10G)          | 1.08 Gbits/sec  | 1.41 Gbits/sec  | 158 ms
Eranium         | Amsterdam, NL (100G)      | 6.28 Gbits/sec  | 4.48 Gbits/sec  | 170 ms
Uztelecom       | Tashkent, UZ (10G)        | 5.46 Gbits/sec  | 3.12 Gbits/sec  | 188 ms
Leaseweb        | Singapore, SG (10G)       | 2.96 Gbits/sec  | 5.00 Gbits/sec  | 2.16 ms
Clouvider       | Los Angeles, CA, US (10G) | 996 Mbits/sec   | 1.30 Gbits/sec  | 207 ms
Leaseweb        | NYC, NY, US (10G)         | 3.39 Gbits/sec  | 3.09 Gbits/sec  | 229 ms
Edgoo           | Sao Paulo, BR (1G)        | busy            | 2.73 Mbits/sec  | 368 ms

iperf3 Network Speed Tests (IPv6):
---------------------------------
Provider        | Location (Link)           | Send Speed      | Recv Speed      | Ping
-----           | -----                     | ----            | ----            | ----
Clouvider       | London, UK (10G)          | 1.02 Gbits/sec  | 1.28 Gbits/sec  | 158 ms
Eranium         | Amsterdam, NL (100G)      | 5.99 Gbits/sec  | 4.41 Gbits/sec  | 170 ms
Uztelecom       | Tashkent, UZ (10G)        | 5.39 Gbits/sec  | 2.90 Gbits/sec  | 188 ms
Leaseweb        | Singapore, SG (10G)       | 8.57 Gbits/sec  | 6.78 Gbits/sec  | 2.30 ms
Clouvider       | Los Angeles, CA, US (10G) | 921 Mbits/sec   | 1.21 Gbits/sec  | 171 ms
Leaseweb        | NYC, NY, US (10G)         | 3.42 Gbits/sec  | 2.30 Gbits/sec  | 235 ms
Edgoo           | Sao Paulo, BR (1G)        | busy            | 1.51 Mbits/sec  | 368 ms

Geekbench 6 Benchmark Test:
---------------------------------
Test            | Value
                |
Single Core     | 1516
Multi Core      | 8316
Full Test       | https://browser.geekbench.com/v6/cpu/12965149

YABS completed in 14 min 4 sec
```

## Bench.Monster Benchmark

```bash
root@ryzumi:~# curl -sL bench.monster | bash
---------------------------------------------------------------------------
 Region: Global  https://bench.monster v1.7.4 2023-12-15
 Usage : curl -sL bench.monster | bash -s -- -Global
---------------------------------------------------------------------------
 OS           : Debian GNU/Linux 12 (64 Bit)
 Virt/Kernel  : KVM / 6.1.0-37-amd64
 CPU Model    : AMD EPYC 7C13 64-Core Processor
 CPU Cores    : 8 @ 1999.997 MHz x86_64 512 KB Cache
 CPU Flags    : AES-NI Enabled & VM-x/AMD-V Enabled
 Load Average : 0.01, 0.13, 0.20
 Total Space  : 119G (1.9G ~2% used)
 Total RAM    : 15991 MB (402 MB + 246 MB Buff in use)
 Total SWAP   : 0 MB (0 MB in use)
 IPv4/IPv6    : ✔ Online / ✔ Online
 Uptime       : 0 days 0:40
---------------------------------------------------------------------------
 Location     : Singapore, Singapore (Central Singapore)
 ASN & ISP    : AS206216, Advin Services LLC / Advin Services LLC
---------------------------------------------------------------------------

 ## Geekbench v6 CPU Benchmark:

  Single Core : 1504  (EXCELLENT)
   Multi Core : 8284

 ## IO Test

 CPU Speed:
    bzip2     : 137 MB/s
   sha256     : 225 MB/s
   md5sum     : 497 MB/s

 RAM Speed:
   Avg. write : 2252.8 MB/s
   Avg. read  : 6485.3 MB/s

 Disk Speed:
   1st run    : 781 MB/s
   2nd run    : 787 MB/s
   3rd run    : 806 MB/s
   -----------------------
   Average    : 791.3 MB/s

 ## Global Speedtest.net

 Location                       Upload           Download         Ping
---------------------------------------------------------------------------
 Nearby                         20.61 Mbit/s     76.55 Mbit/s    * 337.752 ms
---------------------------------------------------------------------------
 USA, New York (Starry)         44.32 Mbit/s     130.66 Mbit/s   230.040 ms
 USA, Chicago (Windstream)      34.77 Mbit/s     105.49 Mbit/s   237.161 ms
 USA, Houston (Comcast)         34.39 Mbit/s     147.94 Mbit/s   207.874 ms
 USA, Los Angeles (Windstream)  78.73 Mbit/s     222.79 Mbit/s   184.004 ms
 UK, London (toob Ltd)          100.60 Mbit/s    97.78 Mbit/s    232.989 ms
 Germany, Berlin (DNS:NET)      11.82 Mbit/s     47.90 Mbit/s    275.910 ms
 Spain, Madrid (MasMovil)       115.91 Mbit/s    362.97 Mbit/s   153.656 ms
 Italy, Rome (Unidata)          95.00 Mbit/s     149.32 Mbit/s   171.640 ms
 India, Mumbai (Tatasky)        345.15 Mbit/s    84.19 Mbit/s    51.784 ms
ping: co2dsvr03.speedtest.starhub.com: Name or service not known
 Japan, Tsukuba (SoftEther)     237.54 Mbit/s    260.43 Mbit/s   70.230 ms
ping: s1.speedtest.syd.optusnet.com.au: Name or service not known
---------------------------------------------------------------------------

 Finished in : 17 min 14 sec
 Timestamp   : 2025-07-22 02:35:11 GMT
 Saved in    : /root/speedtest.log

 Share results:
 - https://www.speedtest.net/result/18004471698.png
 - https://browser.geekbench.com/v6/cpu/12965380
```

## Bench.sh Benchmark

```bash
-------------------- A Bench.sh Script By Teddysun -------------------
 Version            : v2025-05-08
 Usage              : wget -qO- bench.sh | bash
----------------------------------------------------------------------
 CPU Model          : AMD EPYC 7C13 64-Core Processor
 CPU Cores          : 8 @ 1999.997 MHz
 CPU Cache          : 512 KB
 AES-NI             : ✓ Enabled
 VM-x/AMD-V         : ✓ Enabled
 Total Disk         : 118.1 GB (1.9 GB Used)
 Total Mem          : 15.6 GB (403.3 MB Used)
 System uptime      : 0 days, 0 hour 30 min
 Load average       : 0.44, 0.67, 0.35
 OS                 : Debian GNU/Linux 12
 Arch               : x86_64 (64 Bit)
 Kernel             : 6.1.0-37-amd64
 TCP CC             : bbr
 Virtualization     : KVM
 IPv4/IPv6          : ✓ Online / ✓ Online
 Organization       : AS206216 Advin Services LLC
 Location           : Singapore / SG
 Region             : Singapore
----------------------------------------------------------------------
 I/O Speed(1st run) : 810 MB/s
 I/O Speed(2nd run) : 798 MB/s
 I/O Speed(3rd run) : 777 MB/s
 I/O Speed(average) : 795.0 MB/s
----------------------------------------------------------------------
 Node Name        Upload Speed      Download Speed      Latency
 Speedtest.net    8513.30 Mbps      7380.97 Mbps        1.51 ms
 Paris, FR        3155.92 Mbps      6791.19 Mbps        151.66 ms
 Amsterdam, NL    709.36 Mbps       4061.16 Mbps        160.19 ms
 Hong Kong, CN    2468.61 Mbps      4927.46 Mbps        32.26 ms
 Singapore, SG    342.68 Mbps       3669.25 Mbps        34.10 ms
 Tokyo, JP        427.31 Mbps       3980.97 Mbps        176.82 ms
----------------------------------------------------------------------
 Finished in        : 3 min 11 sec
 Timestamp          : 2025-07-22 02:11:33 UTC
----------------------------------------------------------------------
```

## CPU Steal

```bash
root@ryzumi:~# mpstat 30 5
Linux 6.1.0-37-amd64 (ryzumi)   07/22/2025      _x86_64_        (8 CPU)

02:14:12 AM  CPU    %usr   %nice    %sys %iowait    %irq   %soft  %steal  %guest  %gnice   %idle
02:14:42 AM  all    0.04    0.00    0.08    0.00    0.00    0.02    0.00    0.00    0.00   99.87
02:15:12 AM  all    0.03    0.00    0.08    0.00    0.00    0.03    0.00    0.00    0.00   99.86
02:15:42 AM  all    0.03    0.00    0.08    0.00    0.00    0.01    0.00    0.00    0.00   99.88
02:16:12 AM  all    0.03    0.00    0.08    0.00    0.00    0.03    0.00    0.00    0.00   99.86
02:16:42 AM  all    0.01    0.00    0.09    0.00    0.00    0.01    0.00    0.00    0.00   99.88
Average:     all    0.03    0.00    0.08    0.00    0.00    0.02    0.00    0.00    0.00   99.87
root@ryzumi:~#
```