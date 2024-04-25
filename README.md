# DNS Management Exercises (in progress)

## Overview
This project focuses on hands-on DNS management exercises using a Windows Server 2022 environment to demonstrate critical handling of DNS configurations, including A and CNAME records. These exercises illustrate the importance of accurate DNS settings for network reliability and efficiency.

## Environments and Technologies Used
- **DNS Server**: Configured on Windows Server 2022
- **Operating Systems Used**:
  - Windows Server 2022 (Domain Controller DC-1)
  - Windows 10 (Client Machine Client-1)

## High-Level Configuration Steps
1. **Setup DNS Server on Windows Server**:
   - Install and configure the DNS role on Windows Server 2022.
2. **Perform DNS Record Configurations and Testing**:
   - Conduct exercises to add, modify, and test A and CNAME records.
3. **Validate DNS Resolutions and Cache Management**:
   - Test DNS resolutions and understand the behavior of DNS caching.

## Detailed Configuration and Testing Steps

### Step 1: Setup DNS Server
- **Install DNS Server Role**:
  - Use the Server Manager on DC-1 to add the DNS server role.

- **Initial DNS Configuration**:
  - Configure initial DNS settings to manage DNS zones and records effectively.

### Step 2: Perform DNS Record Configurations and Testing
- **A-Record Exercise**:
  - Log into DC-1, create an A record for "mainframe" pointing to DC-1's private IP address. Test pinging "mainframe" from Client-1 to verify resolution.

- **CNAME Record Exercise**:
  - Create a CNAME record on DC-1 that aliases "search" to "www.google.com". Use Client-1 to test the resolution of "search" via ping and `nslookup`.

### Step 3: Validate DNS Resolutions and Cache Management
- **Local DNS Cache Exercise**:
  - Change the "mainframe" A record to a different IP (e.g., 8.8.8.8), then observe and manage DNS cache behavior on Client-1 using `ipconfig /displaydns` and `ipconfig /flushdns`.
