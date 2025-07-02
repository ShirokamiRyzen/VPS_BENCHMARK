# VPS Benchmark Collection

🚀 **Comprehensive VPS benc## 📈 Performance Standards

| Category | CPU (Geekbench) | Disk I/O | Network | CPU Steal |
|----------|-----------------|----------|---------|-----------|
| **🟢 Excellent** | Single: >1000, Multi: >5000 | Sequential: >1GB/s, 4K: >100MB/s | Local: >500Mbps, Global: >100Mbps | 0.00% |
| **🟡 Good** | Single: >800, Multi: >3000 | Sequential: >500MB/s, 4K: >50MB/s | Local: >200Mbps, Global: >50Mbps | <0.10% |
| **🔴 Poor** | Single: <600, Multi: <2000 | Sequential: <200MB/s, 4K: <20MB/s | Local: <100Mbps, Global: <20Mbps | >1.00% |

## 🏆 Latest Benchmarksults from various providers to help you choose the best hosting!**

## 📊 What's in This Repository?

This repository contains complete benchmark results from VPS providers across different locations, including:
- **CPU & RAM Performance** - Geekbench scores and performance metrics
- **Disk I/O Speed** - Random and sequential read/write speeds  
- **Network Speed** - Upload/download from various global locations
- **CPU Steal** - Monitoring overselling from providers

## 🛠️ Benchmark Tools Used

| Tool | Command | Function |
|------|---------|----------|
| **YABS** | `curl -sL https://yabs.sh \| bash` | Complete benchmark (CPU, RAM, Disk, Network) |
| **Bench.Monster** | `curl -sL bench.monster \| bash` | Global network performance |
| **Bench.sh** | `wget -qO- bench.sh \| bash` | Quick I/O and network test |
| **mpstat** | `mpstat 30 5` | Monitor CPU steal time |

## 📁 Repository Structure

```
VPS_BENCHMARK/
├── README.md
├── template.md                        # Template for new benchmarks
└── [Provider] - [Location]/
    └── [Server Specifications].md
```

## 🎯 How to Use This Repository

### 👥 For VPS Buyers
1. **Browse benchmark results** by provider and location
2. **Compare performance** across CPU, I/O, and network speed
3. **Check CPU steal** - should be 0.00% (overselling indicator)
4. **Review Geekbench scores** for standardized comparison

### 🔧 Run Benchmarks Yourself
```bash
# Install tools (usually pre-installed)
apt update && apt install sysstat curl wget -y

# Run complete benchmark suite
curl -sL https://yabs.sh | bash -s -- -r
curl -sL bench.monster | bash  
wget -qO- bench.sh | bash
mpstat 1  # Monitor for several minutes
```

### 🤝 For Contributors
1. Fork this repository
2. Create new folder: `[Provider] - [Location]/`
3. Use `template.md` for consistency
4. Submit pull request with benchmark results

## � Standar Performa

| Kategori | CPU (Geekbench) | I/O Disk | Network | CPU Steal |
|----------|-----------------|----------|---------|-----------|
| **🟢 Excellent** | Single: >1000, Multi: >5000 | Sequential: >1GB/s, 4K: >100MB/s | Local: >500Mbps, Global: >100Mbps | 0.00% |
| **🟡 Good** | Single: >800, Multi: >3000 | Sequential: >500MB/s, 4K: >50MB/s | Local: >200Mbps, Global: >50Mbps | <0.10% |
| **🔴 Poor** | Single: <600, Multi: <2000 | Sequential: <200MB/s, 4K: <20MB/s | Local: <100Mbps, Global: <20Mbps | >1.00% |

## 🏆 Benchmark Terbaru

### OrangeVPS - Singapore
**[Xeon E5-2699 V4 8 vCPU 16GB DDR4 ECC 200GB NVMe](./OrangeVPS%20-%20Singapore/Xeon%20E5-2699%20V4%208%20vCPU%2016GB%20DDR4%20ECC%20200GB%20NVMe.md)**
- 💰 **Price**: $12/month (SM25-5 package)
- 🖥️ **CPU**: Intel Xeon E5-2699 v4 @ 2.20GHz (8 cores)
- 🧠 **RAM**: 16GB DDR4 ECC
- 💾 **Storage**: 200GB NVMe SSD
- 🌐 **Bandwidth**: 10TB @ 1Gbps
- 📊 **Geekbench**: Single: 918, Multi: 4700
- 🎯 **Rating**: 🟡 Good Performance
- 🖥️ **CPU**: Intel Xeon E5-2699 v4 @ 2.20GHz (8 cores)
- 🧠 **RAM**: 16GB DDR4 ECC
- 💾 **Storage**: 200GB NVMe SSD
- 🌐 **Bandwidth**: 10TB @ 1Gbps
- 📊 **Geekbench**: Single: 918, Multi: 4700
- 🎯 **Rating**: 🟡 Good Performance

## 🤝 Contributing

Contributions are welcome! Please ensure:
- ✅ Use `template.md` for consistency
- ✅ Report honest results (both good and bad)
- ✅ Include all benchmark tools
- ✅ Verify server specifications accurately

## 🔗 Useful Links

- [YABS Script](https://github.com/masonr/yet-another-bench-script) - Primary benchmark tool
- [Bench.Monster](https://bench.monster) - Global network testing
- [Geekbench Browser](https://browser.geekbench.com/) - Compare CPU scores

---
**📝 Disclaimer**: Benchmark results may vary depending on server load and network conditions. Use as a comparison reference, not the sole factor in VPS selection.
