# VPS Benchmark Collection

A comprehensive collection of VPS (Virtual Private Server) benchmark results from various providers, helping users make informed decisions when choosing VPS hosting services.

## 📊 What This Repository Contains

This repository contains detailed benchmark results for VPS servers from different providers, including:

- **Performance Metrics**: CPU, RAM, and disk I/O performance
- **Network Speed Tests**: Upload/download speeds from various global locations
- **System Information**: Hardware specifications and virtualization details
- **Geekbench Scores**: Industry-standard CPU benchmarking results

## 🛠️ Benchmark Tools Used

All VPS benchmarks in this repository are performed using these popular and reliable tools:

### 1. YABS (Yet-Another-Bench-Script)
```bash
curl -sL https://yabs.sh | bash -s -- -r
```
- **Purpose**: Comprehensive system benchmarking
- **Tests**: CPU, RAM, disk I/O, network speed, and Geekbench
- **Output**: Detailed system information and performance metrics

### 2. Bench.Monster
```bash
curl -sL bench.monster | bash
```
- **Purpose**: Global network performance testing
- **Tests**: CPU benchmarks, I/O tests, and worldwide speed tests
- **Output**: Performance scores and global connectivity results

### 3. Bench.sh (by Teddysun)
```bash
wget -qO- bench.sh | bash
```
- **Purpose**: Simple and fast benchmarking
- **Tests**: I/O speed and network performance
- **Output**: Quick performance overview

### 4. CPU Steal Monitoring
```bash
mpstat 1
```
- **Purpose**: Monitor CPU steal time (important for VPS)
- **Tests**: Real-time CPU usage statistics
- **Output**: CPU utilization breakdown including steal percentage

## 📁 Repository Structure

```
VPS_BENCHMARK/
├── README.md                          # This file
├── template.md                        # Template for new benchmark reports
└── [Provider] - [Location]/           # Provider-specific folders
    └── [Server Specs].md              # Individual benchmark reports
```

## 🎯 How to Use This Repository

### For VPS Shoppers
1. Browse the benchmark results by provider and location
2. Compare CPU, I/O, and network performance across different options
3. Check CPU steal percentages to assess overselling
4. Review Geekbench scores for standardized CPU performance comparison

### For VPS Providers
1. Use the `template.md` to create standardized benchmark reports
2. Follow the established folder structure: `[Provider] - [Location]/`
3. Include all benchmark tools for comprehensive testing
4. Ensure transparency in reporting both good and poor results

### For Contributors
1. Fork this repository
2. Create a new folder following the naming convention
3. Use the provided template for consistency
4. Submit a pull request with your benchmark results

## 📋 Benchmark Report Template

Each benchmark report should include:

- **Package Information**: Pricing, specifications, and provider details
- **Table of Contents**: Quick navigation to different benchmark sections
- **YABS Benchmark**: Complete system performance overview
- **Bench.Monster Benchmark**: Global network performance
- **Bench.sh Benchmark**: Additional I/O and network tests
- **CPU Steal**: Monitor for resource overselling

## 🔍 Key Metrics to Look For

### CPU Performance
- **Single-core vs Multi-core**: Different workloads benefit from different CPU characteristics
- **Geekbench Scores**: Industry-standard comparison metric
- **CPU Steal**: Should be consistently 0.00% for dedicated resources

### Storage Performance
- **4K Random I/O**: Important for databases and general system responsiveness
- **Sequential I/O**: Important for large file operations
- **Consistency**: Look for stable performance across multiple test runs

### Network Performance
- **Local Network**: Tests within the same region/datacenter
- **Global Connectivity**: Tests to major global locations
- **Upload vs Download**: Asymmetric performance may indicate bandwidth limitations

## 🚀 Running Your Own Benchmarks

To replicate these benchmarks on your own VPS:

1. **Install required tools** (usually pre-installed on most Linux distributions):
   ```bash
   # Update system packages
   apt update && apt upgrade -y
   
   # Install monitoring tools if needed
   apt install sysstat curl wget -y
   ```

2. **Run the benchmark suite**:
   ```bash
   # YABS (comprehensive)
   curl -sL https://yabs.sh | bash -s -- -r
   
   # Bench.Monster (global network)
   curl -sL bench.monster | bash
   
   # Bench.sh (quick overview)
   wget -qO- bench.sh | bash
   
   # Monitor CPU steal (run for several minutes)
   mpstat 1
   ```

3. **Document the results** using the provided template

## 📊 Performance Categories

### Excellent Performance
- **CPU**: Geekbench single-core > 1000, multi-core > 5000
- **I/O**: Sequential > 1GB/s, Random 4K > 100MB/s
- **Network**: > 500 Mbps to local region, > 100 Mbps globally
- **CPU Steal**: Consistently 0.00%

### Good Performance
- **CPU**: Geekbench single-core > 800, multi-core > 3000
- **I/O**: Sequential > 500MB/s, Random 4K > 50MB/s
- **Network**: > 200 Mbps to local region, > 50 Mbps globally
- **CPU Steal**: Occasionally 0.01-0.10%

### Poor Performance
- **CPU**: Geekbench single-core < 600, multi-core < 2000
- **I/O**: Sequential < 200MB/s, Random 4K < 20MB/s
- **Network**: < 100 Mbps to local region, < 20 Mbps globally
- **CPU Steal**: Consistently > 1.00%

## 🤝 Contributing

We welcome contributions! Please:

1. **Follow the template**: Use `template.md` for consistency
2. **Be honest**: Report both good and bad results
3. **Be complete**: Include all benchmark tools
4. **Be accurate**: Double-check server specifications
5. **Be respectful**: Maintain professional tone in reports

## 📝 License

This repository is provided for educational and comparison purposes. All benchmark results are provided as-is without warranty. Individual VPS providers retain ownership of their respective trademarks and service marks.

## 🔗 Useful Links

- [YABS GitHub Repository](https://github.com/masonr/yet-another-bench-script)
- [Bench.Monster Website](https://bench.monster)
- [Bench.sh Script](https://bench.sh)
- [Geekbench Browser](https://browser.geekbench.com/)

---

**Disclaimer**: Benchmark results may vary based on server load, network conditions, and other factors. These results are provided for comparative purposes only and should not be the sole factor in VPS selection decisions.
