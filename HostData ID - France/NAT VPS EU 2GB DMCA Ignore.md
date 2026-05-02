# Package Information

```
ServerPoint XEON E5v4 deals 2025

NAT VPS EU (Torrent) 2GB Package:

2GB RAM
1 vCPU
100 GB HDD
3 TB Bandwidth
Shared IPv4
Dedicated IPv6
20 VDF Records
Domain Forwarding
OpenVZ7
Support VPN, Torrent dan Tunneling

https://hostdata.id/portal/index.php?rp=/store/nat-vps-torrent
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
root@ryzumi-proxy:~# lscpu
Architecture:            x86_64
  CPU op-mode(s):        32-bit, 64-bit
  Address sizes:         46 bits physical, 48 bits virtual
  Byte Order:            Little Endian
CPU(s):                  1
  On-line CPU(s) list:   0
Vendor ID:               GenuineIntel
  Model name:            Intel(R) Xeon(R) CPU E5-2620 v4 @ 2.10GHz
    CPU family:          6
    Model:               79
    Thread(s) per core:  2
    Core(s) per socket:  1
    Socket(s):           1
    Stepping:            1
    BogoMIPS:            4199.97
    Flags:               fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush dts acpi mmx fxsr sse sse2 ss ht tm pbe syscall nx pdpe1gb rdtscp lm constant_tsc arch_perfmon
                          pebs bts rep_good nopl xtopology nonstop_tsc aperfmperf eagerfpu cpuid_faulting pni pclmulqdq dtes64 monitor ds_cpl vmx smx est tm2 ssse3 sdbg fma cx16 xtpr pdcm pcid dca ss
                         e4_1 sse4_2 x2apic movbe popcnt tsc_deadline_timer aes xsave avx f16c rdrand lahf_lm abm 3dnowprefetch epb cat_l3 cdp_l3 invpcid_single ssbd rsb_ctxsw ibrs ibpb stibp tpr_sha
                         dow vnmi flexpriority ept vpid fsgsbase tsc_adjust bmi1 hle avx2 smep bmi2 erms invpcid rtm cqm rdt_a rdseed adx smap intel_pt xsaveopt cqm_llc cqm_occup_llc cqm_mbm_total cq
                         m_mbm_local dtherm ida arat pln pts md_clear spec_ctrl intel_stibp flush_l1d
Virtualization features:
  Virtualization:        VT-x
  Hypervisor vendor:     Parallels
  Virtualization type:   container
Caches (sum of all):
  L1d:                   32 KiB (1 instance)
  L1i:                   32 KiB (1 instance)
  L2:                    256 KiB (1 instance)
  L3:                    20 MiB (1 instance)
```

## YABS Benchmark

```bash
root@ryzumi-proxy:~# curl -sL https://yabs.sh | bash
# ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## #
#              Yet-Another-Bench-Script              #
#                     v2026-04-29                    #
# https://github.com/masonr/yet-another-bench-script #
# ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## #

Sat May  2 10:44:12 AM WIB 2026

Basic System Information:
---------------------------------
Uptime     : 0 days, 12 hours, 2 minutes
Processor  : Intel(R) Xeon(R) CPU E5-2620 v4 @ 2.10GHz
CPU cores  : 1 @ 1724.963 MHz
AES-NI     : ✔ Enabled
VM-x/AMD-V : ✔ Enabled
RAM        : 1.9 GiB
Swap       : 0.0 KiB
Disk       : 98.3 GiB
Distro     : Debian GNU/Linux 13 (trixie)
Kernel     : 3.10.0-1160.90.1.vz7.200.7
VM Type    : OPENVZ
IPv4/IPv6  : ✔ Online / ✔ Online

IPv6 Network Information:
---------------------------------
ISP        : Scaleway SAS
ASN        : AS12876 Scaleway SAS
Host       : Scaleway
Location   : Paris, Île-de-France (IDF)
Country    : France

fio Disk Speed Tests (Mixed R/W 50/50) (Partition /dev/ploop18565p1):
---------------------------------
Block Size | 4k            (IOPS) | 64k           (IOPS)
  ------   | ---            ----  | ----           ----
Read       | 1.25 MB/s      (313) | 23.27 MB/s     (363)
Write      | 1.28 MB/s      (321) | 23.66 MB/s     (369)
Total      | 2.54 MB/s      (634) | 46.93 MB/s     (732)
           |                      |
Block Size | 512k          (IOPS) | 1m            (IOPS)
  ------   | ---            ----  | ----           ----
Read       | 70.76 MB/s     (138) | 107.28 MB/s    (104)
Write      | 74.52 MB/s     (145) | 114.43 MB/s    (111)
Total      | 145.29 MB/s    (283) | 221.72 MB/s    (215)

iperf3 Network Speed Tests (IPv4):
---------------------------------
Provider        | Location (Link)           | Send Speed      | Recv Speed      | Ping
-----           | -----                     | ----            | ----            | ----
Clouvider       | London, UK (10G)          | 917 Mbits/sec   | 415 Mbits/sec   | 8.56 ms
Eranium         | Amsterdam, NL (100G)      | 918 Mbits/sec   | 414 Mbits/sec   | 11.0 ms
Uztelecom       | Tashkent, UZ (10G)        | 720 Mbits/sec   | 239 Mbits/sec   | 181 ms
Leaseweb        | Singapore, SG (10G)       | 824 Mbits/sec   | 313 Mbits/sec   | 156 ms
Clouvider       | Los Angeles, CA, US (10G) | 826 Mbits/sec   | 248 Mbits/sec   | 144 ms
Leaseweb        | NYC, NY, US (10G)         | 892 Mbits/sec   | 290 Mbits/sec   | 75.4 ms
Edgoo           | Sao Paulo, BR (1G)        | 724 Mbits/sec   | 69.8 Mbits/sec  | 185 ms

iperf3 Network Speed Tests (IPv6):
---------------------------------
Provider        | Location (Link)           | Send Speed      | Recv Speed      | Ping
-----           | -----                     | ----            | ----            | ----
Clouvider       | London, UK (10G)          | 397 Mbits/sec   | 409 Mbits/sec   | 8.39 ms
Eranium         | Amsterdam, NL (100G)      | 394 Mbits/sec   | 408 Mbits/sec   | 11.0 ms
Uztelecom       | Tashkent, UZ (10G)        | 117 Mbits/sec   | 207 Mbits/sec   | 181 ms
Leaseweb        | Singapore, SG (10G)       | 82.3 Mbits/sec  | 310 Mbits/sec   | 156 ms
Clouvider       | Los Angeles, CA, US (10G) | 131 Mbits/sec   | 186 Mbits/sec   | 143 ms
Leaseweb        | NYC, NY, US (10G)         | 230 Mbits/sec   | 336 Mbits/sec   | 75.3 ms
Edgoo           | Sao Paulo, BR (1G)        | 75.6 Mbits/sec  | 87.4 Mbits/sec  | 185 ms

Geekbench 6 Benchmark Test:
---------------------------------
Test            | Value
                |
Single Core     | 561
Multi Core      | 563
Full Test       | https://browser.geekbench.com/v6/cpu/17847182
```

## Bench.Monster Benchmark

```bash
root@ryzumi-proxy:~# curl -sL bench.monster | bash
---------------------------------------------------------------------------
 Region: Global  https://bench.laset.com v1.8.7 2026-02-02
 Usage : curl -sL bench.laset.com | bash -s -- -Global
---------------------------------------------------------------------------
 OS           : Debian GNU/Linux 13 (64 Bit)
 Virt/Kernel  : Openvz / 3.10.0-1160.90.1.vz7.200.7
 CPU Model    : Intel(R) Xeon(R) CPU E5-2620 v4 @ 2.10GHz
 CPU Cores    : 1 @ 1724.963 MHz x86_64 20480 KB Cache
 CPU Flags    : AES-NI Enabled & VM-x/AMD-V Enabled
 Load Average : 0.28, 0.08, 0.07
 Total Space  : 99G (3.3G ~4% used)
 Total RAM    : 2000 MB (338 MB + 632 MB Buff in use)
 Total SWAP   : 0 MB (0 MB in use)
 IPv4/IPv6    : ✔ Online / ✔ Online
 Uptime       : 0 days 13:16
---------------------------------------------------------------------------
 Location     : France, Paris (Île-de-France)
 ASN & ISP    : AS12876, Scaleway SAS / ONLINE
---------------------------------------------------------------------------

 Performing Geekbench v6 CPU Benchmark test. Please wait...
curl: option : blank argument where content is expected
 ## Geekbench v6 CPU Benchmark:

  Single Core :   (POOR)
   Multi Core :
    CPU Steal : 0%

 ## IO Test

 CPU Speed:
    bzip2     : 64.8 MB/s
   sha256     : 186 MB/s
   md5sum     : 277 MB/s
    Steal     : 0%

 RAM Speed:
   Avg. write : 1365.3 MB/s
   Avg. read  : 2730.7 MB/s

 Disk Speed:
   1st run    : 244 MB/s
   2nd run    : 311 MB/s
   3rd run    : 569 MB/s
   -----------------------
   Average    : 374.7 MB/s

 ## Global Speedtest.net

 Location                             Upload      Download       Ping    Loss
-------------------------------------------------------------------------------
 Nearby                           400.26 Mbps   406.97 Mbps    0.95 ms      0%
-------------------------------------------------------------------------------
 USA, New York (Optimum)          102.42 Mbps   408.11 Mbps   80.51 ms      0%
 USA, Chicago (Uniti)             140.55 Mbps   400.99 Mbps   97.51 ms     N/A
 USA, Los Angeles (Uniti)          87.96 Mbps   399.61 Mbps  149.51 ms     N/A
 UK, London (Hyperoptic)          176.24 Mbps   404.02 Mbps   77.01 ms     N/A
 Germany, Frankfurt (Plusnet)     389.61 Mbps   409.25 Mbps   13.31 ms      0%
 India, Mumbai (Tata Play)         91.02 Mbps   403.43 Mbps  120.36 ms      0%
 Singapore (MyRepublic)           507.04 Mbps   422.20 Mbps  178.98 ms      0%
 Japan, Tokyo (Nearoute)           22.76 Mbps   423.47 Mbps  221.82 ms  11.71%
 Australia, Sydney (Neptune)       58.92 Mbps   426.98 Mbps  256.87 ms      0%
 Brazil, Sao Paulo (TIM)           59.03 Mbps   364.55 Mbps  249.98 ms      0%

 ## Statistics

 Total Traffic    : 8.11 GB
 Total Downloaded : 5.61 GB
 Total Uploaded   : 2.50 GB

 Average Loss     : 1.46 %

---------------------------------------------------------------------------
 Finished in : 25 min 14 sec

 Timestamp   : 2026-05-02 05:23:11 GMT
 Saved in    : /root/speedtest.log

 Share results:
 - https://www.speedtest.net/result/c/3d1ddd30-c17c-4df4-bc62-034468d33a9e
 -

root@ryzumi-proxy:~#
```

## Bench.sh Benchmark

```bash
-------------------- A Bench.sh Script By Teddysun -------------------
 Version            : v2026-01-31
 Usage              : wget -qO- bench.sh | bash
----------------------------------------------------------------------
 CPU Model          : Intel(R) Xeon(R) CPU E5-2620 v4 @ 2.10GHz
 CPU Cores          : 1 @ 1724.963 MHz
 CPU Cache          : 20480 KB
 AES-NI             : ✓ Enabled
 VM-x/AMD-V         : ✓ Enabled
 Total Disk         : 98.3 GB (3.2 GB Used)
 Total RAM          : 2.0 GB (300.9 MB Used)
 System Uptime      : 0 days, 11 hour 53 min
 Load Average       : 0.03, 0.35, 0.27
 OS                 : Debian GNU/Linux 13 (trixie)
 Arch               : x86_64 (64 Bit)
 Kernel             : 3.10.0-1160.90.1.vz7.200.7
 TCP Congestion Ctrl:
 Virtualization     : OPENVZ
 IPv4/IPv6          : ✓ Online / ✓ Online
 Organization       : AS12876 Scaleway SAS
 Location           : Paris / FR
 Region             : Île-de-France
----------------------------------------------------------------------
 I/O Speed(1st run) : 592 MB/s
 I/O Speed(2nd run) : 594 MB/s
 I/O Speed(3rd run) : 615 MB/s
 I/O Speed(average) : 600.3 MB/s
----------------------------------------------------------------------
 Node Name        Upload Speed      Download Speed      Latency
 Speedtest.net    403.09 Mbps       411.00 Mbps         1.05 ms
 Los Angeles, US  656.95 Mbps       436.21 Mbps         135.62 ms
 Dallas, US       107.61 Mbps       409.32 Mbps         105.60 ms
 Montreal, CA     119.67 Mbps       401.25 Mbps         90.39 ms
 Paris, FR        401.82 Mbps       410.55 Mbps         0.96 ms
 Amsterdam, NL    385.79 Mbps       409.48 Mbps         9.91 ms
 Suzhou, CN       54.80 Mbps        413.45 Mbps         211.07 ms
 Ningbo, CN       0.87 Mbps         358.05 Mbps         204.47 ms
 Hong Kong, CN    521.81 Mbps       415.54 Mbps         166.90 ms
 Singapore, SG    573.68 Mbps       445.42 Mbps         153.76 ms
 Taipei, CN       67.03 Mbps        434.30 Mbps         207.04 ms
 Tokyo, JP        65.09 Mbps        443.99 Mbps         229.86 ms
----------------------------------------------------------------------
 Finished in        : 5 min 34 sec
 Timestamp          : 2026-05-02 10:41:17 WIB
----------------------------------------------------------------------
```

## CPU Steal

```bash
root@ryzumi-proxy:~# mpstat 30 5
Linux 3.10.0-1160.90.1.vz7.200.7 (ryzumi-proxy)         05/02/2026      _x86_64_        (1 CPU)

10:25:16 AM  CPU    %usr   %nice    %sys %iowait    %irq   %soft  %steal  %guest  %gnice   %idle
10:25:46 AM  all    1.64    0.00    0.98    0.00    0.00    0.00    0.00    0.00    0.00   97.38
10:26:16 AM  all    1.16    0.00    0.93    0.00    0.00    0.00    0.00    0.00    0.00   97.91
10:26:46 AM  all    1.73    0.00    0.98    0.00    0.00    0.00    0.00    0.00    0.00   97.29
10:27:16 AM  all    0.80    0.00    0.89    0.00    0.00    0.00    0.00    0.00    0.00   98.31
10:27:46 AM  all    0.76    0.00    0.84    0.00    0.00    0.00    0.00    0.00    0.00   98.40
Average:     all    1.22    0.00    0.92    0.00    0.00    0.00    0.00    0.00    0.00   97.86
root@ryzumi-proxy:~#
```