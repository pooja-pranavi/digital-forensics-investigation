# Digital Forensics Investigation – Insider Attack Analysis

## Overview

This project presents a complete digital forensic investigation of a simulated insider-assisted attack on an administrative system. The analysis combines memory forensics and disk forensics to identify malicious activity, recover deleted artifacts, and reconstruct attacker behavior.

The investigation focuses on detecting unauthorized data manipulation, hidden processes, and anti-forensic techniques using industry-standard tools.


## Objectives

* Identify insider-based unauthorized activity
* Detect suspicious and hidden processes from memory
* Recover deleted files and artifacts
* Analyze anti-forensic behavior
* Reconstruct the attack timeline


## Tools Used

* **FTK Imager** – Disk image acquisition and evidence preservation
* **Volatility** – Memory analysis and process investigation
* **Autopsy** – File system analysis and recovery of deleted data

## Investigation Workflow

### 1. Evidence Acquisition

* Collected disk image in `.E01` format
* Maintained integrity of forensic evidence

### 2. Memory Analysis (Volatility)

* Used `pslist` and `psscan` to identify running and hidden processes
* Detected suspicious process activity indicating compromise
* Observed anomalies in process execution

### 3. Disk Analysis (Autopsy)

* Recovered multiple deleted files
* Identified suspicious file activity
* Analyzed metadata and file system structure

### 4. Behavioral Analysis

* Identified insider with legitimate access abusing privileges
* Detected data manipulation and unauthorized actions
* Observed anti-forensic attempts such as file deletion


## Key Findings

* Suspicious process detected through memory analysis
* Evidence of large-scale file deletion
* Indicators of unauthorized access and data tampering
* Signs of anti-forensic activity to hide traces


## Results Summary

* Identified a suspicious and potentially hidden process through memory analysis
* Recovered multiple deleted files indicating anti-forensic activity
* Detected unauthorized data manipulation within the system
* Correlated memory and disk artifacts to reconstruct attacker behavior


## Impact

This project demonstrates practical application of digital forensics techniques to detect, analyze, and reconstruct real-world insider attack scenarios.

## Conclusion

The investigation confirms an insider-assisted attack involving data manipulation and concealment. By combining memory and disk forensic techniques, the attack behavior was successfully analyzed and key indicators of compromise were identified.

## Repository Note

Large forensic evidence files (.E01, memory dumps) are excluded due to size limitations. Only analysis artifacts and the investigation report are included.
