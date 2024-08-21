# BASTION
Blue Team Assessment and Security Threat Investigation and Oversight Network
---

### **Problem Statement**

- **Observation**: Most individuals are hasty when upgrading or updating their Windows systems to address potential adversarial actions.
- **Need**: A system vulnerability detector and scanner is required to:
  - Audit and verify system and network vulnerabilities.
  - Rectify misconfigurations.
  - Mitigate prominent threats to individuals or organizations.
- **Approach**: Implement a blue team strategy to identify and map potential vulnerabilities in a Windows OS subsystem for enhanced security.

### **Expected Solution**

- **General Requirements**:
  - **Agent-less Mechanism**: The solution must be AV/EDR friendly and operate without requiring agents.
  - **Vulnerability and Exploit Searching**: Ability to search for and crawl open-source exploits and their patches.
  - **Supported Platforms**: Must work with the latest Windows 10/11 builds.
  - **Report Generation**: Consolidate findings into report files (PDF and/or HTML format).

- **System-Level Information**:
  - **Basic OS Information**:
    - OS version details.
    - Installed .NET versions.
  - **Security Configurations**:
    - Providers registered for AMSI.
    - Registered antivirus information (via WMI).
    - Classic and advanced audit policy settings (registry keys).
  - **Auto-Run Items**:
    - Executables/scripts/programs set to auto-run.
  - **Firewall and Defender Settings**:
    - Standard and non-standard firewall rules.
    - Windows Defender settings, including exclusion locations.
  - **User and System Information**:
    - User and machine personal certificate files.
    - Current environment PATH folders and environment variables.
    - Lists of files/folders, including downloads, documents, and desktop folders.
    - File version information and AMSI providers registered for AMSI.
  - **Hotfixes and Installed Products**:
    - Installed hotfixes (via WMI).
    - Installed products (registry).
  - **Group Policies and Users**:
    - Local Group Policy settings.
    - Non-empty local groups.
    - Local users (active/disabled).
  - **Microsoft Updates**:
    - All updates (via COM, WMI).
  - **Authentication and Remote Connections**:
    - NTLM authentication settings.
    - Saved RDP connections (registry).
    - Current incoming RDP sessions.
    - Remote Desktop Server/Client settings.
  - **System Security Configurations**:
    - Secure Boot configuration.
    - Sysmon configuration (registry).
    - UAC system policies (registry).
  - **PowerShell History**:
    - Searches for sensitive regex matches in PowerShell console history files.

- **Network-Level Information**:
  - **Network Configuration**:
    - Lists the current ARP table and adapter information.
    - DNS cache entries (via WMI).
    - Windows network profiles.
  - **Network Shares and Connections**:
    - Exposed network shares.
    - Current TCP and UDP connections with associated processes and services.
    - Current RPC endpoints.
    - Open ports status.
  - **Network Discovery**:
    - System interface connectors.
    - LLDP/CDP connections to infrastructure devices.
    - Attached network vectors (systems within the VLAN).
  - **Network Diagram**:
    - Capability to formulate a network diagram using the gathered information.

---
