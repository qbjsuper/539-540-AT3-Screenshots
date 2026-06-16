# ICTNWK539/540 AT3 Screenshot Index

This index matches the **ICTNWK539/540 AT3 Screenshot Checklist** and uses the current GitHub repository structure.

Repository:

```text
https://github.com/qbjsuper/539-540-AT3-Screenshots
```

## Link structure used in this index

Link format:

```text
[filename](filename)
```

Example:

```text
[SS_5-3_BAA_BIG_FILE1_NTFS_Permissions.jpg](SS_5-3_BAA_BIG_FILE1_NTFS_Permissions.jpg)
```

## Lab name mapping

| Checklist name | Practical lab name |
|---|---|
| BAA-FILE1 | BAA-BIG-FILE1 |
| BAA-WS1 / Workstation | BAA-BIG-WS |
| BAA-DC1 | BAA-BIG-DC1 |
| BAA-DC2 | BAA-SML-DC1 |
| Linux VM | BAA-BIG-LX1 or selected Ubuntu Linux VM |
| Mail server | BAA-SML-MAIL1 |
| HA / cluster evidence | BAA-BIG-Nest1, BAA-SML-Nest1, BAA-STOR1 |

## 1. VM and Host Foundation

| No. | Checklist requirement | Screenshot file / link | Notes |
| --- | --- | --- | --- |
| 1.1 | Hyper-V Manager showing required VMs | [SS_1-1_HyperV_Manager_Required_VMs.jpg](SS_1-1_HyperV_Manager_Required_VMs.jpg) | Show required AT3 VMs on physical Hyper-V host. |
| 1.2 | PowerShell VM list showing VM state, CPU, RAM, and uptime | [SS_1-2_PowerShell_VM_State_CPU_RAM_Uptime.jpg](SS_1-2_PowerShell_VM_State_CPU_RAM_Uptime.jpg) | Use `Get-VM` output from Hyper-V host. |
| 1.3 | VM settings for key servers | [SS_1-3_VM_Settings_Key_Servers.jpg](SS_1-3_VM_Settings_Key_Servers.jpg) | Show CPU, memory, firmware, disk and switch settings. |
| 1.4 | VM network adapter list showing virtual switch connections | [SS_1-4_VM_Network_Adapter_VSwitch_Connections.jpg](SS_1-4_VM_Network_Adapter_VSwitch_Connections.jpg) | Show VMs connected to the correct Hyper-V virtual switch. |
| 1.5 | VM disk list or VM hard drive settings | [SS_1-5_VM_Disk_Inventory_Hard_Drive_Settings.jpg](SS_1-5_VM_Disk_Inventory_Hard_Drive_Settings.jpg) | Shows guest volume layout for BAA-BIG-FILE1. |
| 1.5B | Additional VM hard disk evidence | [SS_1-5B_BAA_BIG_FILE1_Attached_VHDX_Disks.jpg](SS_1-5B_BAA_BIG_FILE1_Attached_VHDX_Disks.jpg) | Extra evidence from Hyper-V host showing attached VHDX disks. |

## 2. Windows Server and Domain Foundation

| No. | Checklist requirement | Screenshot file / link | Notes |
| --- | --- | --- | --- |
| 2.1 | Server Manager dashboard on BAA-BIG-DC1 | [SS_2-1_BAA_BIG_DC1_Server_Manager_Dashboard.jpg](SS_2-1_BAA_BIG_DC1_Server_Manager_Dashboard.jpg) | Proves BAA-BIG-DC1 is installed and running. |
| 2.2 | Server Manager dashboard on BAA-SML-DC1 | [SS_2-2_BAA_SML_DC1_Server_Manager_Dashboard.jpg](SS_2-2_BAA_SML_DC1_Server_Manager_Dashboard.jpg) | Proves BAA-SML-DC1 is installed and running. |
| 2.3 | Active Directory Domain Controllers list | [SS_2-3_AD_Domain_Controllers_List.jpg](SS_2-3_AD_Domain_Controllers_List.jpg) | Show both DCs in `bojieanzac.com`. |
| 2.4 | Ping from BAA-BIG-DC1 to BAA-SML-DC1 | [SS_2-4_BIG_DC1_to_SML_DC1_Ping.jpg](SS_2-4_BIG_DC1_to_SML_DC1_Ping.jpg) | Cross-site DC connectivity. |
| 2.5 | Ping from BAA-SML-DC1 to BAA-BIG-DC1 | [SS_2-5_SML_DC1_to_BIG_DC1_Ping.jpg](SS_2-5_SML_DC1_to_BIG_DC1_Ping.jpg) | Reverse cross-site DC connectivity. |
| 2.6 | DNS Manager showing bojieanzac.com zone | [SS_2-6_DNS_Manager_bojieanzac_Zone.jpg](SS_2-6_DNS_Manager_bojieanzac_Zone.jpg) | AD-integrated DNS evidence. |
| 2.7 | DHCP console showing active scope | [SS_2-7_DHCP_Console_Active_Scope.jpg](SS_2-7_DHCP_Console_Active_Scope.jpg) | DHCP scope evidence. |
| 2.8 | DHCP lease for workstation | [SS_2-8_DHCP_Lease_for_Workstation.jpg](SS_2-8_DHCP_Lease_for_Workstation.jpg) | Show BAA-BIG-WS lease. |

## 3. Workstation Evidence

| No. | Checklist requirement | Screenshot file / link | Notes |
| --- | --- | --- | --- |
| 3.1 | Windows 11 Pro workstation running | [SS_3-1_Windows_11_Workstation_Running.jpg](SS_3-1_Windows_11_Workstation_Running.jpg) | Lab uses Windows 11 Enterprise Evaluation; acceptable for domain-capable workstation evidence. |
| 3.2 | Workstation IP configuration | [SS_3-2_Workstation_IP_Configuration.jpg](SS_3-2_Workstation_IP_Configuration.jpg) | Show IP, gateway, DNS and DHCP settings. |
| 3.3 | Workstation domain membership showing bojieanzac.com | [SS_3-3_Workstation_Domain_Membership.jpg](SS_3-3_Workstation_Domain_Membership.jpg) | Shows BAA-BIG-WS joined to `bojieanzac.com`. |
| 3.4 | Domain user login on workstation | [SS_3-4_Workstation_Domain_User_Login.jpg](SS_3-4_Workstation_Domain_User_Login.jpg) | Shows domain account login on workstation. |
| 3.5A | Workstation ping to BAA-BIG-DC1 | [SS_3-5A_Workstation_Ping_to_BIG_DC1.jpg](SS_3-5A_Workstation_Ping_to_BIG_DC1.jpg) | Ping to `172.16.60.10`. |
| 3.5B | Workstation ping to BAA-SML-DC1 | [SS_3-5B_Workstation_Ping_to_SML_DC1.jpg](SS_3-5B_Workstation_Ping_to_SML_DC1.jpg) | Ping to `172.16.50.10`. |
| 3.6 | Workstation DNS lookup for bojieanzac.com | [SS_3-6_Workstation_DNS_Lookup_bojieanzac.jpg](SS_3-6_Workstation_DNS_Lookup_bojieanzac.jpg) | DNS resolves both DCs. |

## 4. Active Directory Objects

| No. | Checklist requirement | Screenshot file / link | Notes |
| --- | --- | --- | --- |
| 4.1 | Active Directory Users and Computers showing OUs | [SS_4-1_ADUC_Organisational_Units.jpg](SS_4-1_ADUC_Organisational_Units.jpg) | Shows Anzac Airport OU and sub-OUs. |
| 4.2 | At least two created users | [SS_4-2_ADUC_Created_Users.jpg](SS_4-2_ADUC_Created_Users.jpg) | Shows Finance, Administration, IT and Ground Operations test users. |
| 4.3 | Security groups for departments | [SS_4-3_ADUC_Department_Security_Groups.jpg](SS_4-3_ADUC_Department_Security_Groups.jpg) | Shows `BAA-GRP-*` department security groups. |
| 4.4 | User group membership | [SS_4-4_AD_User_Group_Membership.jpg](SS_4-4_AD_User_Group_Membership.jpg) | Shows users mapped to correct access groups. |

## 5. File Server, Folder Structure, and Permissions

| No. | Checklist requirement | Screenshot file / link | Notes |
| --- | --- | --- | --- |
| 5.1 | BAA-FILE1 running | [SS_5-1_BAA_BIG_FILE1_Running.jpg](SS_5-1_BAA_BIG_FILE1_Running.jpg) | BAA-FILE1 is implemented as BAA-BIG-FILE1. |
| 5.2 | Shared folder structure | [SS_5-2_BAA_BIG_FILE1_Shared_Folder_Structure.jpg](SS_5-2_BAA_BIG_FILE1_Shared_Folder_Structure.jpg) | Shows `D:\Shares` department folder structure. |
| 5.2B | SMB shares created | [SS_5-2B_BAA_BIG_FILE1_SMB_Shares_Created.jpg](SS_5-2B_BAA_BIG_FILE1_SMB_Shares_Created.jpg) | Extra evidence showing SMB share names and paths. Upload this if not already uploaded. |
| 5.3 | NTFS permissions on a department folder | [SS_5-3_BAA_BIG_FILE1_NTFS_Permissions.jpg](SS_5-3_BAA_BIG_FILE1_NTFS_Permissions.jpg) | Shows NTFS permissions using AD security groups. |
| 5.4 | Authorised user accessing correct folder | [SS_5-4_Authorised_User_Folder_Access.jpg](SS_5-4_Authorised_User_Folder_Access.jpg) | Finance user accesses Finance share. |
| 5.5 | Unauthorised user denied access | [SS_5-5_Unauthorised_User_Access_Denied.jpg](SS_5-5_Unauthorised_User_Access_Denied.jpg) | Administration user denied access to Finance share. |
| 5.6 | File creation/edit/save test | [SS_5-6_File_Create_Edit_Save_Test.jpg](SS_5-6_File_Create_Edit_Save_Test.jpg) | Finance user creates and saves test file. |
| 5.X | BAA-BIG-FILE1 domain join verification | [SS_BAA_BIG_FILE1_Domain_Join_Verification.jpg](SS_BAA_BIG_FILE1_Domain_Join_Verification.jpg) | Extra support evidence proving the file server is joined to `bojieanzac.com`. |

## 6. Windows and Linux Integration

| No. | Checklist requirement | Screenshot file / link | Notes |
| --- | --- | --- | --- |
| 6.1 | Ubuntu Server version | [SS_6-1_Ubuntu_Server_Version.jpg](SS_6-1_Ubuntu_Server_Version.jpg) | Proves non-Windows OS is installed. |
| 6.2 | Ubuntu IP configuration | [SS_6-2_Ubuntu_IP_Configuration.jpg](SS_6-2_Ubuntu_IP_Configuration.jpg) | Shows Linux IP, gateway and DNS settings. |
| 6.3 | Ubuntu joined to or authenticating with AD | [SS_6-3_Ubuntu_AD_Domain_Integration.jpg](SS_6-3_Ubuntu_AD_Domain_Integration.jpg) | Linux/AD integration evidence. |
| 6.4 | AD user authentication from Ubuntu | [SS_6-4_AD_User_Authentication_From_Ubuntu.jpg](SS_6-4_AD_User_Authentication_From_Ubuntu.jpg) | Proves AD user authentication from Linux. |
| 6.5 | Samba/SMB or SFTP share access from Windows | [SS_6-5_Windows_to_Linux_Share_Access.jpg](SS_6-5_Windows_to_Linux_Share_Access.jpg) | Cross-platform sharing evidence. |
| 6.6 | Linux firewall allowing required application traffic | [SS_6-6_Linux_Firewall_Application_Traffic.jpg](SS_6-6_Linux_Firewall_Application_Traffic.jpg) | Linux firewall evidence. |

## 7. Web, Mail, and FTP Services

| No. | Checklist requirement | Screenshot file / link | Notes |
| --- | --- | --- | --- |
| 7.1 | Web service running on Linux | [SS_7-1_Linux_Web_Service_Running.jpg](SS_7-1_Linux_Web_Service_Running.jpg) | Linux web service status. |
| 7.2 | Web page opened from workstation | [SS_7-2_Web_Page_Access_From_Workstation.jpg](SS_7-2_Web_Page_Access_From_Workstation.jpg) | Web connectivity from BAA-BIG-WS. |
| 7.3 | Mail service running | [SS_7-3_Mail_Service_Running.jpg](SS_7-3_Mail_Service_Running.jpg) | Mail server service status. |
| 7.4 | Email sent from one user mailbox | [SS_7-4_Email_Sent_From_User_Mailbox.jpg](SS_7-4_Email_Sent_From_User_Mailbox.jpg) | Mail sending test. |
| 7.5 | Email received by another user mailbox | [SS_7-5_Email_Received_By_User_Mailbox.jpg](SS_7-5_Email_Received_By_User_Mailbox.jpg) | Mail receiving test. |
| 7.6 | FTP/SFTP service running | [SS_7-6_FTP_SFTP_Service_Running.jpg](SS_7-6_FTP_SFTP_Service_Running.jpg) | FTP/SFTP service status. |
| 7.7 | FTP/SFTP login from workstation | [SS_7-7_FTP_SFTP_Login_From_Workstation.jpg](SS_7-7_FTP_SFTP_Login_From_Workstation.jpg) | Authorised transfer login. |
| 7.8 | FTP/SFTP upload and download test | [SS_7-8_FTP_SFTP_Upload_Download_Test.jpg](SS_7-8_FTP_SFTP_Upload_Download_Test.jpg) | File transfer test. |
| 7.9 | Large file FTP/SFTP transfer | [SS_7-9_Large_File_FTP_SFTP_Transfer.jpg](SS_7-9_Large_File_FTP_SFTP_Transfer.jpg) | Large transfer evidence. |
| 7.10 | Concurrent FTP/SFTP user/session test | [SS_7-10_Concurrent_FTP_SFTP_Sessions.jpg](SS_7-10_Concurrent_FTP_SFTP_Sessions.jpg) | Concurrent session evidence. |

## 8. WSUS, Printer GPO, Proxy, and NTP

| No. | Checklist requirement | Screenshot file / link | Notes |
| --- | --- | --- | --- |
| 8.1 | WSUS installed or configured | [SS_8-1_BAA_BIG_FILE1_WSUS_Installed_Configured.jpg](SS_8-1_BAA_BIG_FILE1_WSUS_Installed_Configured.jpg) | WSUS on BAA-BIG-FILE1 or selected Windows server. |
| 8.2 | WSUS computer group or update status | [SS_8-2_WSUS_Computer_Group_Update_Status.jpg](SS_8-2_WSUS_Computer_Group_Update_Status.jpg) | WSUS update management evidence. |
| 8.3 | Shared printer added on server | [SS_8-3_BAA_BIG_FILE1_Shared_Printer_Added.jpg](SS_8-3_BAA_BIG_FILE1_Shared_Printer_Added.jpg) | Printer hosted on BAA-BIG-FILE1. |
| 8.4 | Printer deployment Group Policy | [SS_8-4_Printer_Deployment_Group_Policy.jpg](SS_8-4_Printer_Deployment_Group_Policy.jpg) | GPO printer deployment evidence. |
| 8.5 | Printer visible on workstation | [SS_8-5_Printer_Visible_on_Workstation.jpg](SS_8-5_Printer_Visible_on_Workstation.jpg) | GPO printer deployment test. |
| 8.6 | Squid proxy service running | [SS_8-6_Squid_Proxy_Service_Running.jpg](SS_8-6_Squid_Proxy_Service_Running.jpg) | Linux proxy service evidence. |
| 8.7 | Workstation/browser using proxy or proxy access log | [SS_8-7_Proxy_Browser_Test_or_Access_Log.jpg](SS_8-7_Proxy_Browser_Test_or_Access_Log.jpg) | Proxy test evidence. |
| 8.8 | NTP/time sync status on Windows | [SS_8-8_Windows_NTP_Time_Sync_Status.jpg](SS_8-8_Windows_NTP_Time_Sync_Status.jpg) | Windows domain time synchronisation. |
| 8.9 | NTP/time sync status on Ubuntu | [SS_8-9_Ubuntu_NTP_Time_Sync_Status.jpg](SS_8-9_Ubuntu_NTP_Time_Sync_Status.jpg) | Linux time synchronisation. |

## 9. Backup and Restore

| No. | Checklist requirement | Screenshot file / link | Notes |
| --- | --- | --- | --- |
| 9.1 | Backup tool or Windows Server Backup installed | [SS_9-1_BAA_BIG_FILE1_Backup_Tool_Installed.jpg](SS_9-1_BAA_BIG_FILE1_Backup_Tool_Installed.jpg) | Windows Server Backup capability. |
| 9.2 | Backup job configured | [SS_9-2_Backup_Job_Configured.jpg](SS_9-2_Backup_Job_Configured.jpg) | Backup settings evidence. |
| 9.3 | Backup completed successfully | [SS_9-3_Backup_Completed_Successfully.jpg](SS_9-3_Backup_Completed_Successfully.jpg) | Backup test passed. |
| 9.4 | Test file deleted or changed | [SS_9-4_Test_File_Deleted_or_Changed.jpg](SS_9-4_Test_File_Deleted_or_Changed.jpg) | Restore scenario evidence. |
| 9.5 | File restored to another server or recovery location | [SS_9-5_File_Restored_to_Recovery_Location.jpg](SS_9-5_File_Restored_to_Recovery_Location.jpg) | Restore requirement. |
| 9.6 | Restored file opened successfully | [SS_9-6_Restored_File_Opened_Successfully.jpg](SS_9-6_Restored_File_Opened_Successfully.jpg) | Restored data is usable. |

## 10. Firewall Testing

| No. | Checklist requirement | Screenshot file / link | Notes |
| --- | --- | --- | --- |
| 10.1 | Ping works before Windows Firewall change | [SS_10-1_Ping_Works_Before_Windows_Firewall_Change.jpg](SS_10-1_Ping_Works_Before_Windows_Firewall_Change.jpg) | Baseline ping before block rule. |
| 10.2 | Windows Firewall rule blocking ping | [SS_10-2_Windows_Firewall_Rule_Blocking_Ping.jpg](SS_10-2_Windows_Firewall_Rule_Blocking_Ping.jpg) | Windows firewall rule configuration. |
| 10.3 | Ping blocked after firewall change | [SS_10-3_Ping_Blocked_After_Firewall_Change.jpg](SS_10-3_Ping_Blocked_After_Firewall_Change.jpg) | Proves ICMP is blocked. |
| 10.4 | Required services still accessible after ping block | [SS_10-4_Required_Services_Accessible_After_Ping_Block.jpg](SS_10-4_Required_Services_Accessible_After_Ping_Block.jpg) | Proves SMB/web/etc. still works. |
| 10.5 | Linux firewall status | [SS_10-5_Linux_Firewall_Status.jpg](SS_10-5_Linux_Firewall_Status.jpg) | Linux firewall configuration. |
| 10.6 | Linux application access allowed | [SS_10-6_Linux_Application_Access_Allowed.jpg](SS_10-6_Linux_Application_Access_Allowed.jpg) | Linux application allowed through firewall. |

## 11. Performance and Diagnostic Evidence

| No. | Checklist requirement | Screenshot file / link | Notes |
| --- | --- | --- | --- |
| 11.1 | Windows Task Manager or Performance Monitor | [SS_11-1_Windows_Performance_Monitoring.jpg](SS_11-1_Windows_Performance_Monitoring.jpg) | Windows performance monitoring. |
| 11.2 | Windows Event Viewer with no critical service errors | [SS_11-2_Windows_Event_Viewer_No_Critical_Errors.jpg](SS_11-2_Windows_Event_Viewer_No_Critical_Errors.jpg) | Diagnostic review. |
| 11.3 | Server Manager showing roles/services running | [SS_11-3_Server_Manager_Roles_Services_Running.jpg](SS_11-3_Server_Manager_Roles_Services_Running.jpg) | Service status evidence. |
| 11.4 | Ubuntu CPU, memory, disk, and network status | [SS_11-4_Ubuntu_CPU_Memory_Disk_Network_Status.jpg](SS_11-4_Ubuntu_CPU_Memory_Disk_Network_Status.jpg) | Linux performance monitoring. |
| 11.5 | Ubuntu service status for web/FTP/proxy/NTP/mail | [SS_11-5_Ubuntu_Service_Status.jpg](SS_11-5_Ubuntu_Service_Status.jpg) | Linux service diagnostics. |
| 11.6 | Hyper-V Manager showing VM health | [SS_11-6_HyperV_Manager_VM_Health.jpg](SS_11-6_HyperV_Manager_VM_Health.jpg) | Virtualisation host status. |
| 11.7 | Diagnostic report or command output | [SS_11-7_Diagnostic_Report_or_Command_Output.jpg](SS_11-7_Diagnostic_Report_or_Command_Output.jpg) | Diagnostic command/report evidence. |

## 12. High Availability / Cluster Evidence

| No. | Checklist requirement | Screenshot file / link | Notes |
| --- | --- | --- | --- |
| 12.1 | Failover Cluster Manager showing cluster nodes | [SS_12-1_Failover_Cluster_Manager_Nodes.jpg](SS_12-1_Failover_Cluster_Manager_Nodes.jpg) | Shows BAA-BIG-Nest1 and BAA-SML-Nest1. |
| 12.2 | Cluster Shared Volume or shared storage | [SS_12-2_Cluster_Shared_Volume_or_Shared_Storage.jpg](SS_12-2_Cluster_Shared_Volume_or_Shared_Storage.jpg) | CSV or BAA-STOR1 shared storage. |
| 12.3 | Test VM running as clustered role | [SS_12-3_Test_VM_Running_as_Clustered_Role.jpg](SS_12-3_Test_VM_Running_as_Clustered_Role.jpg) | Cluster-protected test VM. |
| 12.4 | Controlled VM move from one node to another | [SS_12-4_Controlled_VM_Move_Between_Nodes.jpg](SS_12-4_Controlled_VM_Move_Between_Nodes.jpg) | Planned migration evidence. |
| 12.5 | VM running after move/failover | [SS_12-5_VM_Running_After_Move_or_Failover.jpg](SS_12-5_VM_Running_After_Move_or_Failover.jpg) | Availability after movement. |
| 12.6 | Ping or service access before and after VM move | [SS_12-6_Ping_Service_Access_Before_After_VM_Move.jpg](SS_12-6_Ping_Service_Access_Before_After_VM_Move.jpg) | Service continuity evidence. |

## 13. Troubleshooting Evidence

| No. | Checklist requirement | Screenshot file / link | Notes |
| --- | --- | --- | --- |
| 13.1 | Failed test result before fix | [SS_13-1_AD_User_Create_Failed_Password_Policy.jpg](SS_13-1_AD_User_Create_Failed_Password_Policy.jpg) | AD user creation failed due to password policy. |
| 13.2 | Diagnostic command/tool used | [SS_13-2_AD_User_Create_Error_Message.jpg](SS_13-2_AD_User_Create_Error_Message.jpg) | Optional diagnostic screenshot for AD user creation issue. |
| 13.3 | Configuration correction | [SS_13-3_AD_User_Create_Strong_Password_Retry.jpg](SS_13-3_AD_User_Create_Strong_Password_Retry.jpg) | Optional screenshot showing retry with strong password, without exposing password. |
| 13.4 | Successful retest after fix | [SS_13-4_AD_Test_Users_Created.jpg](SS_13-4_AD_Test_Users_Created.jpg) | Users enabled after password reset. |
| 13.5 | Completed troubleshooting table | [SS_13-5_Completed_Troubleshooting_Table.jpg](SS_13-5_Completed_Troubleshooting_Table.jpg) | Screenshot of completed troubleshooting document. |
| 13.6 | Extra failed login evidence | [SS_13-6_Workstation_Test_User_RDS_Logon_Denied.png](SS_13-6_Workstation_Test_User_RDS_Logon_Denied.png) | Enhanced Session / RDS login denied. This file is `.png` in the repo. |
| 13.7 | Extra successful login evidence | [SS_13-7_Workstation_Test_User_Basic_Session_Login.jpg](SS_13-7_Workstation_Test_User_Basic_Session_Login.jpg) | Basic Session login succeeded. |

## 14. Final Report Evidence

| No. | Checklist requirement | Screenshot file / link | Notes |
| --- | --- | --- | --- |
| 14.1 | Final VM list after implementation | [SS_14-1_Final_VM_List_After_Implementation.jpg](SS_14-1_Final_VM_List_After_Implementation.jpg) | Final Hyper-V VM list. |
| 14.2 | Final service status summary | [SS_14-2_Final_Service_Status_Summary.jpg](SS_14-2_Final_Service_Status_Summary.jpg) | Summary of service status across servers. |
| 14.3 | Final test plan with results completed | [SS_14-3_Final_Test_Plan_With_Results.jpg](SS_14-3_Final_Test_Plan_With_Results.jpg) | Completed Test Plan document. |
| 14.4 | Final troubleshooting document completed | [SS_14-4_Final_Troubleshooting_Document.jpg](SS_14-4_Final_Troubleshooting_Document.jpg) | Completed Troubleshooting document. |
| 14.5 | Final report sign-off page | [SS_14-5_Final_Report_Sign_Off_Page.jpg](SS_14-5_Final_Report_Sign_Off_Page.jpg) | Final Report sign-off evidence. |
