Windows Brute‑Force Detection (EventCode 4625)
This project demonstrates a Splunk detection for Windows failed authentication attempts (EventCode 4625).
The goal is to identify potential brute‑force attacks by correlating failed logons within a short time window.

Detection Logic
A brute‑force attempt is defined as:

≥5 failed logons

from the same SourceIP

within 30 seconds
