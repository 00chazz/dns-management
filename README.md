<h1>DNS Management Exercises</h1>

<h2>Overview</h2>
This project involved managing DNS settings, including A and CNAME records, in order to critically handle network services that ensure proper network operations and connectivity.

## Environments and Technologies Used
- **DNS Server**: Configuration on a Windows Server environment
- **Operating Systems Used**:
  - Windows Server 2022

## High-Level Configuration Steps
1. **Setup a DNS Server on Windows Server**:
   - Install and configure the DNS role on a Windows Server.
2. **Configure A and CNAME Records**:
   - Add and modify A and CNAME records to reflect changes in the network.
3. **Test DNS Resolutions**:
   - Verify that the DNS records are correctly resolving to their respective IP addresses.

## Detailed Configuration and Testing Steps

### Step 1: Setup DNS Server
- **Install DNS Server Role**:
  - On your Windows Server 2022, use the Server Manager to add the DNS server role.
  - **Screenshot**: Capture the completion screen of the DNS role installation to show it has been successfully added.

- **Initial DNS Configuration**:
  - Set up basic DNS settings to prepare for managing DNS records.
  - **Screenshot**: Show the initial DNS dashboard or the main configuration page where DNS zones are visible.

### Step 2: Configure DNS Records
- **Add A Records**:
  - Create A records to map domain names to IP addresses. For instance, map `example.com` to `192.168.1.1`.
  - **Screenshot**: Display the DNS management console with the list of new A records added, highlighting the mappings.

- **Modify CNAME Records**:
  - Set up CNAME records to alias one domain name to another. For example, alias `www.example.com` to `example.com`.
  - **Screenshot**: Illustrate the DNS console showing the CNAME records configuration with the domain aliases properly set.

### Step 3: Test DNS Resolutions
- **DNS Lookup Tests**:
  - Use tools like `nslookup` or `dig` to test if the DNS records are resolving correctly. Perform this from different clients if possible.
  - **Screenshot**: Capture the command-line output of `nslookup www.example.com` showing the IP address it resolves to, matching the A record.

## Conclusion
Effective DNS management is crucial for ensuring network reliability and efficiency. This project provides a practical approach to managing DNS records, highlighting best practices for configuring A and CNAME records to support robust network operations.

## Connect with Me
- **LinkedIn:** [Chazz Conino](https://www.linkedin.com/in/chazz-c-382a75122/)
