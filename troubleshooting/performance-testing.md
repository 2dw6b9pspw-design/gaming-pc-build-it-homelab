# Performance Testing and Validation

This document outlines the performance and stability testing performed after system assembly and operating system installation to validate thermals, stability, and component functionality.

---

## 1. Test Objectives

- Verify CPU thermal performance under sustained load
- Confirm overall system stability
- Validate storage performance and health
- Establish baseline performance metrics for future comparison

---

## 2. Test Environment

- Operating System: Windows
- CPU: AMD Ryzen 5 7600X3D
- Cooling Solution: Thermalright Peerless Assassin 120 SE ARGB
- Graphics: Integrated graphics
- Monitoring and Test Tools:
  - HWiNFO
  - Prime95
  - Cinebench R23
  - Samsung Magician

---

## 3. Idle Performance Validation

After completing OS installation and driver setup, the system was allowed to idle at the desktop to establish baseline thermal and voltage behavior.

Using HWiNFO for monitoring, the following observations were recorded:

- CPU package, CCD, and hotspot temperatures remained within expected idle ranges
- Memory clock and timings confirmed DDR5-6000 operation
- CPU voltages remained stable at idle
- Core C-state residency confirmed proper power management behavior

![HWiNFO Idle Baseline](../images/hwinfo-idle-baseline.png)

This baseline validation confirmed correct cooler installation, proper memory configuration, and normal idle system behavior prior to stress testing.

---

## 4. CPU Stress Testing

Prime95 was used to apply sustained CPU load to evaluate thermal limits and system stability.

- Test was allowed to run for an extended duration
- CPU temperatures were monitored continuously using HWiNFO
- No thermal throttling, crashes, or system instability were observed

![Prime95 Stress Test](../images/prime95-stress-test.png)

---

## 5. CPU Performance Benchmarking

Cinebench R23 was used to measure CPU performance under both single-core and multi-core workloads.

- Multi-core benchmark confirmed expected performance for the installed CPU
- Single-core benchmark validated boost behavior and clock scaling

![Cinebench Multi-Core](../images/cinebench-multicore.png)  
![Cinebench Single-Core](../images/cinebench-singlecore.png)

---

## 6. Storage Performance and Health Validation

Samsung Magician was used to validate NVMe SSD health and performance.

- Drive health reported as normal
- Sequential and random performance metrics were within expected ranges
- Firmware version was verified

![Samsung 990 Pro Benchmark](../images/samsung-990pro-benchmark.png)

---

## 7. Stability Verification

- Performed multiple system reboots following stress and benchmark testing
- Verified consistent POST behavior
- Confirmed no system crashes, freezes, or unexpected reboots occurred during testing

---

## 8. Results Summary

The system demonstrated stable operation under idle and sustained load conditions. CPU temperatures remained within safe operating limits, storage performance met expectations, and no hardware or driver-related issues were identified during testing.

---

## 9. Next Steps

- Monitor thermals during extended gaming sessions
- Re-evaluate performance after future hardware upgrades
- Maintain baseline metrics for long-term comparison

