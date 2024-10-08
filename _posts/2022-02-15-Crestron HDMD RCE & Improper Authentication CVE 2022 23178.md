![](https://reciprocity.com/wp-content/uploads/2021/09/blog_most-common-types-cybersecurity-vulnerabilities_featured-img_730x270.jpg)

## Crestron HD-MD-XX -RCE & Improper Authentication-  CVE-2022-23178
As an AV Technician I take an interest in securing AV devices that I interact with. In this process I discovered a vulnerability with the Crestron HD-MD series of “DM-LITE” devices that allows for remote code execution as well as inproper handling of plaintext credentials.

[Here is the official vulnerability report that I submitted to Crestron](https://github.com/AnthonyTippy/Vulnerabilities/blob/main/Crestron_HD-MD_Series_Vulnerability_Report_-_Anthony_Tippy_-_08-10-21.pdf)

Discovered : 07/01/2021
Reported : 08/10/2021
Crestron Response: 10/07/2021
Publicly Disclosed : 02/15/2022

I submitted a request to MITRE for an official CVE but received no response. 

Vulnerability was discovered in the summer of 2021.  I contacted and reported this vulnerability to Crestron.  They are aware of the issue after my reporting, but have chosen to accept this risk/vulnerability.

## CVE-2022-23178 -Red Team PenTesting
Red Team Pentesting appears to have also [discovered the vulnerability](redteam-pentesting.de/en/advisories/rt-sa-2021-009/-credential-disclosure-in-web-interface-of-crestron-device) regarding credentials being stored in cleartext and have submitted [CVE-2022-23178](https://nvd.nist.gov/vuln/detail/CVE-2022-23178) however this makes no mention of the RCE capabilities that these devices are vulnerable to as well.  

### CVE-2022-23178  Detail

### Current Description

An issue was discovered on Crestron HD-MD4X2-4K-E 1.0.0.2159 devices. When the administrative web interface of the HDMI switcher is accessed unauthenticated, user credentials are disclosed that are valid to authenticate to the web interface. Specifically, aj.html sends a JSON document with uname and upassword fields.
### Severity
**Base Score:** [9.8 CRITICAL](https://nvd.nist.gov/vuln-metrics/cvss/v3-calculator?name=CVE-2022-23178&vector=AV:N/AC:L/PR:N/UI:N/S:U/C:H/I:H/A:H&version=3.1&source=NIST)

