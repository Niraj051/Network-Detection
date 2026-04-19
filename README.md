# Network-Activity-Detection (Sysmon Event ID 3)

## Summary

Detected network connections initiated from command-line activity.Two ports observered: 4444 and 8000.

## Tools Used
-Sysmon
-Splunk

## Evidence 
-Event ID: 1 (Process Creation)
-Event ID: 3 (Network Connection)
-Ports observed: 4444 , 8000
-Source Process: Resume.pdf.exe

## Analysis
 Port 4444 is commonly associated with penetration testing tools and reverse shells in lab environment. Port 8000 is commonly used for local web servers and   development service
  The risk depends on the process initiating the connection and the destination IP.

  ## Conclusion
  Activity may be begin in a lab environment but demonstrates how network connection are generated from system processes.

  ## Key Learning 
  Network ports alone are not indicators of attack. Context (process + behavior) is required for detection.
