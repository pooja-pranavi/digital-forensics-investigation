# Digital Forensics Investigation – Insider Attack Analysis

## Overview

This project presents a full digital forensic investigation of a simulated insider-assisted compromise in an administrative system. The analysis combines memory forensics and disk forensics to identify malicious activity, reconstruct events, and uncover anti-forensic behavior.

The investigation focuses on detecting unauthorized data manipulation, hidden processes, and evidence of cleanup attempts using industry-standard forensic tools.

---

## Objectives

* Identify insider-based data tampering
* Detect malicious and hidden processes from memory
* Recover deleted artifacts from disk
* Analyze anti-forensic techniques
* Reconstruct attack timeline

---

## Tools Used

* **FTK Imager** – Evidence acquisition and disk imaging
* **Volatility** – Memory analysis and process inspection
* **Autopsy** – File system and deleted data analysis

---

## Investigation Workflow

### 1. Evidence Acquisition

* Collected disk image (.E01 format)
* Preserved integrity of evidence for analysis

### 2. Memory Analysis (Volatility)

* Used `pslist` and `psscan` to identify active and hidden processes
* Detected suspicious process indicating possible malicious activity
* Observed abnormal timestamps suggesting manipulation

### 3. Disk Analysis (Autopsy)

* Recovered thousands of deleted files
* Identified suspicious files and traces of unauthorized activity
* Analyzed file system metadata for anomalies

### 4. Behavioral Analysis

* Identified insider using valid system access
* Detected record manipulation and unauthorized changes
* Observed anti-forensic actions such as file deletion and cleanup

---

## Key Findings

* Suspicious process activity detected in memory
* Evidence of large-scale file deletion (anti-forensics)
* Indicators of data tampering and unauthorized access
* Attempt to conceal activity using cleanup techniques

---

## Conclusion

The investigation confirms an insider-assisted attack involving data manipulation and concealment. By combining memory and disk forensic techniques, it was possible to reconstruct the attack behavior and identify critical indicators of compromise.

---

## Repository Note

Large forensic evidence files (.E01, memory dumps) are not included due to size limitations. Only analysis artifacts and report files are provided.
