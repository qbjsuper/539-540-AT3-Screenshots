# ICTNWK539/540 AT3 Screenshot Index

This index matches the **ICTNWK539/540 AT3 Screenshot Checklist** and the current screenshot evidence repository for the Anzac Airport integrated server implementation.

Repository:

```text
https://github.com/qbjsuper/539-540-AT3-Screenshots
```

## Link structure used in this index

The index uses relative links so it works inside the GitHub repository.

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
| BAA-DC1 | BAA-BIG-DC1 |
| BAA-DC2 | BAA-SML-DC1 |
| BAA-WS1 / Workstation | BAA-BIG-WS |
| BAA-FILE1 | BAA-BIG-FILE1 |
| BAA-MAIL1 | BAA-SML-MAIL1 |
| BAA-LNX1 | BAA-BIG-LX1 |
| Linux web server | BAA-SML-WEB1 |
| Linux Samba server | BAA-BIG-LX2 |
| Shared storage / HA evidence | BAA-STOR1, BAA-BIG-Nest1, BAA-SML-Nest1 |
| Firewalls | BAA-BIG-PFS1, BAA-SML-PFS1 |

## Important notes

- Azure Update Manager is used as the approved replacement for WSUS.
- BAA-FILE1 is implemented as BAA-BIG-FILE1.
- BAA-DC1 is implemented as BAA-BIG-DC1.
- BAA-DC2 is implemented as BAA-SML-DC1.
- High availability evidence uses BAA-STOR1, BAA-BIG-Nest1, BAA-SML-Nest1, and the BAA-NEST-CL1 failover cluster.
- Combined screenshots are used where one screenshot covers more than one checklist item.

## 1. VM and Host Foundation

| No. | Checklist requirement | Screenshot file / link | Notes |
|---|---|---|---|
| 1.1 | Hyper-V Manager showing required VMs | [SS_1-1_HyperV_Manager_Required_VMs.jpg](SS_1-1_HyperV_Manager_Required_VMs.jpg) | Upload if not already visible in the repository. |
| 1.2 | PowerShell VM list showing VM state, CPU, RAM, and uptime | [SS_1-2_PowerShell_VM_State_CPU_RAM_Uptime.jpg](SS_1-2_PowerShell_VM_State_CPU_RAM_Uptime.jpg) | Upload if not already visible in the repository. |
| 1.3 | VM settings for key servers | [SS_1-3_VM_Settings_Key_Servers.jpg](SS_1-3_VM_Settings_Key_Servers.jpg) | Upload if not already visible in the repository. |
| 1.4 | VM network adapter list showing virtual switch connections | [SS_1-4_VM_Network_Adapter_VSwitch_Connections.jpg](SS_1-4_VM_Network_Adapter_VSwitch_Connections.jpg) | Upload if not already visible in the repository. |
| 1.5 | VM disk list or VM hard drive settings | [SS_1-5_VM_Disk_Inventory_Hard_Drive_Settings.jpg](SS_1-5_VM_Disk_Inventory_Hard_Drive_Settings.jpg) | Shows disk inventory / hard drive settings. |

## 2. Windows Server and Domain Foundation

| No. | Checklist requirement | Screenshot file / link | Notes |
|---|---|---|---|
| 2.1 | Server Manager dashboard on BAA-BIG-DC1 | [SS_2-1_BAA_BIG_DC1_Server_Manager_Dashboard.jpg](SS_2-1_BAA_BIG_DC1_Server_Manager_Dashboard.jpg) | Upload if not already visible in the repository. |
| 2.2 | Server Manager dashboard on BAA-SML-DC1 | [SS_2-2_BAA_SML_DC1_Server_Manager_Dashboard.jpg](SS_2-2_BAA_SML_DC1_Server_Manager_Dashboard.jpg) | Upload if not already visible in the repository. |
| 2.3 | Active Directory Domain Controllers list | [SS_2-3_AD_Domain_Controllers_List.jpg](SS_2-3_AD_Domain_Controllers_List.jpg) | Shows both domain controllers in bojieanzac.com. |
| 2.4 | Ping from BAA-BIG-DC1 to BAA-SML-DC1 | [SS_2-4_BIG_DC1_to_SML_DC1_Ping.jpg](SS_2-4_BIG_DC1_to_SML_DC1_Ping.jpg) | Cross-site DC connectivity. |
| 2.5 | Ping from BAA-SML-DC1 to BAA-BIG-DC1 | [SS_2-5_SML_DC1_to_BIG_DC1_Ping.jpg](SS_2-5_SML_DC1_to_BIG_DC1_Ping.jpg) | Reverse cross-site DC connectivity. |
| 2.6 | DNS Manager showing bojieanzac.com zone | [SS_2-6_DNS_Manager_bojieanzac_Zone.jpg](SS_2-6_DNS_Manager_bojieanzac_Zone.jpg) | AD-integrated DNS evidence. |
| 2.7 | DHCP console showing active scope | [SS_2-7_DHCP_Console_Active_Scope.jpg](SS_2-7_DHCP_Console_Active_Scope.jpg) | DHCP scope evidence. |
| 2.8 | DHCP lease for workstation | [SS_2-8_DHCP_Lease_for_Workstation.jpg](SS_2-8_DHCP_Lease_for_Workstation.jpg) | Workstation lease evidence. |

## 3. Workstation Evidence

| No. | Checklist requirement | Screenshot file / link | Notes |
|---|---|---|---|
| 3.1 | Windows 11 Pro workstation running | [SS_3-1_Windows_11_Workstation_Running.jpg](SS_3-1_Windows_11_Workstation_Running.jpg) | Upload if not already visible in the repository. |
| 3.2 | Workstation IP configuration | [SS_3-2_Workstation_IP_Configuration.jpg](SS_3-2_Workstation_IP_Configuration.jpg) | Upload if not already visible in the repository. |
| 3.3 | Workstation domain membership showing bojieanzac.com | [SS_3-3_Workstation_Domain_Membership.jpg](SS_3-3_Workstation_Domain_Membership.jpg) | Shows BAA-BIG-WS joined to bojieanzac.com. |
| 3.4 | Domain user login on workstation | [SS_3-4_Workstation_Domain_User_Login.jpg](SS_3-4_Workstation_Domain_User_Login.jpg) | Shows successful domain user login. |
| 3.5A | Workstation ping to BAA-BIG-DC1 | [SS_3-5A_Workstation_Ping_to_BIG_DC1.jpg](SS_3-5A_Workstation_Ping_to_BIG_DC1.jpg) | Ping to 172.16.60.10. |
| 3.5B | Workstation ping to BAA-SML-DC1 | [SS_3-5B_Workstation_Ping_to_SML_DC1.jpg](SS_3-5B_Workstation_Ping_to_SML_DC1.jpg) | Ping to 172.16.50.10. |
| 3.6 | Workstation DNS lookup for bojieanzac.com | [SS_3-6_Workstation_DNS_Lookup_bojieanzac.jpg](SS_3-6_Workstation_DNS_Lookup_bojieanzac.jpg) | DNS resolves the domain controller addresses. |

## 4. Active Directory Objects

| No. | Checklist requirement | Screenshot file / link | Notes |
|---|---|---|---|
| 4.1 | Active Directory Users and Computers showing OUs | [SS_4-1_ADUC_Organisational_Units.jpg](SS_4-1_ADUC_Organisational_Units.jpg) | Shows OUs created for the design. |
| 4.2 | At least two created users | [SS_4-2_ADUC_Created_Users.jpg](SS_4-2_ADUC_Created_Users.jpg) | Shows the created test users. |
| 4.3 | Security groups for departments | [SS_4-3_ADUC_Department_Security_Groups.jpg](SS_4-3_ADUC_Department_Security_Groups.jpg) | Shows department security groups. |
| 4.4 | User group membership | [SS_4-4_AD_User_Group_Membership.jpg](SS_4-4_AD_User_Group_Membership.jpg) | Shows users assigned to correct access groups. |

## 5. File Server, Folder Structure, and Permissions

| No. | Checklist requirement | Screenshot file / link | Notes |
|---|---|---|---|
| 5.1 | BAA-FILE1 running | [SS_5-1_BAA_BIG_FILE1_Running.jpg](SS_5-1_BAA_BIG_FILE1_Running.jpg) | BAA-FILE1 is implemented as BAA-BIG-FILE1. |
| 5.2 | Shared folder structure | [SS_5-2_BAA_BIG_FILE1_Shared_Folder_Structure.jpg](SS_5-2_BAA_BIG_FILE1_Shared_Folder_Structure.jpg) | Shows the department folder structure. |
| 5.3 | NTFS permissions on a department folder | [SS_5-3_BAA_BIG_FILE1_NTFS_Permissions.jpg](SS_5-3_BAA_BIG_FILE1_NTFS_Permissions.jpg) | Shows NTFS permissions using AD groups. |
| 5.4 | Authorised user accessing correct folder | [SS_5-4_Authorised_User_Folder_Access.jpg](SS_5-4_Authorised_User_Folder_Access.jpg) | Authorised user access test. |
| 5.5 | Unauthorised user denied access | [SS_5-5_Unauthorised_User_Access_Denied.jpg](SS_5-5_Unauthorised_User_Access_Denied.jpg) | Restricted access test. |
| 5.6 | File creation/edit/save test | [SS_5-6_File_Create_Edit_Save_Test.jpg](SS_5-6_File_Create_Edit_Save_Test.jpg) | Data availability for authorised user. |
| Extra | BAA-BIG-FILE1 domain join verification | [SS_BAA_BIG_FILE1_Domain_Join_Verification.jpg](SS_BAA_BIG_FILE1_Domain_Join_Verification.jpg) | Extra support evidence proving the file server is domain joined. |

## 6. Windows and Linux Integration

| No. | Checklist requirement | Screenshot file / link | Notes |
|---|---|---|---|
| 6.1 | Ubuntu Server version | [SS_6-1_Ubuntu_Server_Version.jpg](SS_6-1_Ubuntu_Server_Version.jpg) | Non-Windows OS evidence. |
| 6.2 | Ubuntu IP configuration | [SS_6-2_Ubuntu_IP_Configuration.jpg](SS_6-2_Ubuntu_IP_Configuration.jpg) | Linux IP, gateway, and DNS evidence. |
| 6.3 | Ubuntu joined to or authenticating with AD | [SS_6-3_Ubuntu_AD_Domain_Integration.jpg](SS_6-3_Ubuntu_AD_Domain_Integration.jpg) | Linux / AD integration evidence. |
| 6.4 | AD user authentication from Ubuntu | [SS_6-4_AD_User_Authentication_From_Ubuntu.jpg](SS_6-4_AD_User_Authentication_From_Ubuntu.jpg) | AD user authentication from Linux. |
| 6.5 | Windows to Linux sharing evidence | [SS_6-5_SFTP_or_Samba_Access_From_Windows.jpg](SS_6-5_SFTP_or_Samba_Access_From_Windows.jpg) | Original cross-platform sharing evidence. |
| 6.5A | BAA-BIG-LX2 pre-domain join check | [SS_6-5A_BAA_BIG_LX2_Pre_Domain_Join_Check.jpg](SS_6-5A_BAA_BIG_LX2_Pre_Domain_Join_Check.jpg) | Samba server baseline. |
| 6.5B | BAA-BIG-LX2 domain join verification | [SS_6-5B_BAA_BIG_LX2_Domain_Join_Verification.jpg](SS_6-5B_BAA_BIG_LX2_Domain_Join_Verification.jpg) | Samba / Winbind domain join. |
| 6.5C | BAA-BIG-LX2 AD computer object | [SS_6-5C_BAA_BIG_LX2_AD_Computer_Object.jpg](SS_6-5C_BAA_BIG_LX2_AD_Computer_Object.jpg) | Linux server visible in AD. |
| 6.5D | Samba and Winbind services running | [SS_6-5D_Samba_Winbind_Service_Running_On_BAA_BIG_LX2.jpg](SS_6-5D_Samba_Winbind_Service_Running_On_BAA_BIG_LX2.jpg) | Samba service evidence. |
| 6.5E | Samba share configured with AD group | [SS_6-5E_Samba_Share_Configured_With_AD_Group.jpg](SS_6-5E_Samba_Share_Configured_With_AD_Group.jpg) | AD group-based access control. |
| 6.5F | Samba port 445 reachable from workstation | [SS_6-5F_Samba_Port_445_Reachable_From_BAA_BIG_WS.jpg](SS_6-5F_Samba_Port_445_Reachable_From_BAA_BIG_WS.jpg) | SMB service connectivity. |
| 6.5G | Samba share access from Windows domain user | [SS_6-5G_Samba_Share_Access_From_Windows_Domain_User.jpg](SS_6-5G_Samba_Share_Access_From_Windows_Domain_User.jpg) | Authorised domain user access. |
| 6.5H | Samba file create/read test from Windows | [SS_6-5H_Samba_File_Create_Read_Test_Domain_User.jpg](SS_6-5H_Samba_File_Create_Read_Test_Domain_User.jpg) | Cross-platform data test. |
| 6.5I | Samba access control negative test | [SS_6-5I_Samba_Share_Access_Control_Negative_Test.jpg](SS_6-5I_Samba_Share_Access_Control_Negative_Test.jpg) | Non-member access denied. |
| 6.6 | Linux firewall allowing required application traffic | [SS_6-6_Linux_Firewall_Application_Traffic_Allowed.jpg](SS_6-6_Linux_Firewall_Application_Traffic_Allowed.jpg) | Linux firewall evidence. |
| Extra | BAA-SML-WEB1 AD domain join verification | [SS_EXTRA_WEB1_AD_Domain_Join_Verification.jpg](SS_EXTRA_WEB1_AD_Domain_Join_Verification.jpg) | Extra Linux domain integration evidence. |

## 7. Web, Mail, and FTP/SFTP Services

| No. | Checklist requirement | Screenshot file / link | Notes |
|---|---|---|---|
| 7.1 | Web service running on Linux | [SS_7-1_Web_Service_Running_On_Linux.jpg](SS_7-1_Web_Service_Running_On_Linux.jpg) | Web service status. |
| 7.2 | Web page opened from workstation | [SS_7-2_Web_Page_Opened_From_Workstation.jpg](SS_7-2_Web_Page_Opened_From_Workstation.jpg) | Web connectivity from BAA-BIG-WS. |
| 7.3A | Mail service running evidence 1 | [SS_7-3_Mail_Service_Running_On_BAA-SML-MAIL1(1).jpg](SS_7-3_Mail_Service_Running_On_BAA-SML-MAIL1(1).jpg) | Mail service support evidence. |
| 7.3B | Mail service running evidence 2 | [SS_7-3_Mail_Service_Running_On_BAA-SML-MAIL1(2).jpg](SS_7-3_Mail_Service_Running_On_BAA-SML-MAIL1(2).jpg) | Mail service support evidence. |
| 7.3C | Mail service running evidence 3 | [SS_7-3_Mail_Service_Running_On_BAA-SML-MAIL1(3).jpg](SS_7-3_Mail_Service_Running_On_BAA-SML-MAIL1(3).jpg) | Mail service support evidence. |
| 7.4 | Email sent from one user mailbox | [SS_7-4_Email_Sent_From_Finance_User_Mailbox.jpg](SS_7-4_Email_Sent_From_Finance_User_Mailbox.jpg) | Mail sending test. |
| 7.5 | Email received by another user mailbox | [SS_7-5_Email_Received_By_Admin_User_Mailbox.jpg](SS_7-5_Email_Received_By_Admin_User_Mailbox.jpg) | Mail receiving test. |
| 7.6 | FTP/SFTP service running | [SS_7-6_SFTP_Service_Running_On_BAA-BIG-LX1.jpg](SS_7-6_SFTP_Service_Running_On_BAA-BIG-LX1.jpg) | OpenSSH SFTP service evidence. |
| 7.7 | FTP/SFTP login from workstation | [SS_7-7_SFTP_Login_From_Workstation.jpg](SS_7-7_SFTP_Login_From_Workstation.jpg) | Authorised SFTP login. |
| 7.8 | FTP/SFTP upload and download test | [SS_7-8_SFTP_Upload_And_Download_Test.jpg](SS_7-8_SFTP_Upload_And_Download_Test.jpg) | Upload and download test. |
| 7.9 | Large file FTP/SFTP transfer | [SS_7-9_Large_File_SFTP_Transfer.jpg](SS_7-9_Large_File_SFTP_Transfer.jpg) | Large transfer evidence. |
| 7.10 | Concurrent FTP/SFTP user/session test | [SS_7-10_Concurrent_SFTP_Session_Test.jpg](SS_7-10_Concurrent_SFTP_Session_Test.jpg) | Concurrent session evidence. |

## 8. Update Management, Printer GPO, Proxy, and NTP

| No. | Checklist requirement | Screenshot file / link | Notes |
|---|---|---|---|
| 8.1 | Update management configured | [SS_8-1_Azure_Update_Manager_Machines_Onboarded.jpg](SS_8-1_Azure_Update_Manager_Machines_Onboarded.jpg) | Azure Update Manager used as approved WSUS replacement. |
| 8.1B | Periodic update assessment enabled | [SS_8-1B_Azure_Update_Manager_Periodic_Assessment_Enabled.jpg](SS_8-1B_Azure_Update_Manager_Periodic_Assessment_Enabled.jpg) | Azure Update Manager assessment setting. |
| 8.2 | Update compliance status | [SS_8-2_Azure_Update_Manager_Update_Compliance_Status.jpg](SS_8-2_Azure_Update_Manager_Update_Compliance_Status.jpg) | Update compliance evidence. |
| 8.2B | Update assessment result | [SS_8-2B_Azure_Update_Manager_Assessment_Result.jpg](SS_8-2B_Azure_Update_Manager_Assessment_Result.jpg) | Detailed update assessment evidence. |
| 8.2C | Update schedule configured | [SS_8-2C_Azure_Update_Manager_Update_Schedule_Configured.jpg](SS_8-2C_Azure_Update_Manager_Update_Schedule_Configured.jpg) | Maintenance schedule evidence. |
| 8.2D | Associated update schedule | [SS_8-2D_Azure_Update_Manager_Associated_Update_Schedule.jpg](SS_8-2D_Azure_Update_Manager_Associated_Update_Schedule.jpg) | Shows machines associated with schedule. |
| 8.3 | Shared printer added on server | [SS_8-3_Shared_Printer_Added_On_BAA_BIG_FILE1.jpg](SS_8-3_Shared_Printer_Added_On_BAA_BIG_FILE1.jpg) | Printer hosted on BAA-BIG-FILE1. |
| 8.3 Extra | Printer test page printed from server | [SS_EXTRA_8-3_Printer_Test_Page_Printed_From_BAA_BIG_FILE1.jpg](SS_EXTRA_8-3_Printer_Test_Page_Printed_From_BAA_BIG_FILE1.jpg) | Upload if this evidence is used in the Test Plan. |
| 8.4 | Printer deployment Group Policy | [SS_8-4_Printer_Deployment_Group_Policy.jpg](SS_8-4_Printer_Deployment_Group_Policy.jpg) | GPO printer deployment evidence. |
| 8.5 | Printer visible on workstation | [SS_8-5_Printer_Visible_On_BAA_BIG_WS.jpg](SS_8-5_Printer_Visible_On_BAA_BIG_WS.jpg) | Workstation printer deployment test. |
| 8.5 Extra | Finance user printed page output | [SS_EXTRA_8-5_Finance_User_Printed_Page_Output.jpg](SS_EXTRA_8-5_Finance_User_Printed_Page_Output.jpg) | Upload if this evidence is used in the Test Plan. |
| 8.6 | Squid proxy service running | [SS_8-6_Squid_Proxy_Service_Running_On_BAA_BIG_LX1.jpg](SS_8-6_Squid_Proxy_Service_Running_On_BAA_BIG_LX1.jpg) | Linux proxy service evidence. |
| 8.7 | Workstation proxy access log | [SS_8-7_Workstation_Proxy_Access_Log_From_BAA_BIG_WS.jpg](SS_8-7_Workstation_Proxy_Access_Log_From_BAA_BIG_WS.jpg) | Proxy access log evidence. |
| 8.8 | NTP/time sync status on Windows domain controller | [SS_8-8_NTP_DC_Status.jpg](SS_8-8_NTP_DC_Status.jpg) | Windows time synchronisation evidence. |
| 8.9 | NTP/time sync status on Ubuntu Linux VM | [SS_8-9_NTP_Time_Sync_Status_On_BAA_BIG_LX2.jpg](SS_8-9_NTP_Time_Sync_Status_On_BAA_BIG_LX2.jpg) | Linux time synchronisation evidence. |

## 9. Backup and Restore

| No. | Checklist requirement | Screenshot file / link | Notes |
|---|---|---|---|
| 9.1 | Backup tool or Windows Server Backup installed | [SS_9-1_Windows_Server_Backup_Installed_On_BAA_BIG_FILE1.jpg](SS_9-1_Windows_Server_Backup_Installed_On_BAA_BIG_FILE1.jpg) | Windows Server Backup installed. |
| 9.2 / 9.3 | Backup job configured and completed successfully | [SS_9-2_9-3_Backup_Job_Configured_And_Completed_Successfully.jpg](SS_9-2_9-3_Backup_Job_Configured_And_Completed_Successfully.jpg) | Combined evidence for backup configuration and successful completion. |
| 9.4 / 9.5 | Test file deleted and restored to recovery location | [SS_9-4_9-5_Test_File_Deleted_And_Restored_To_Recovery_Location.jpg](SS_9-4_9-5_Test_File_Deleted_And_Restored_To_Recovery_Location.jpg) | Combined evidence for delete and restore scenario. |
| 9.6 | Restored file opened successfully | [SS_9-6_Restored_File_Opened_Successfully.jpg](SS_9-6_Restored_File_Opened_Successfully.jpg) | Restored data is readable. |

## 10. Firewall Testing

| No. | Checklist requirement | Screenshot file / link | Notes |
|---|---|---|---|
| 10.1 | Ping works before Windows Firewall change | [SS_10-1_Ping_Works_Before_Windows_Firewall_Change.jpg](SS_10-1_Ping_Works_Before_Windows_Firewall_Change.jpg) | Baseline ping before block rule. |
| 10.2 | Windows Firewall rule blocking ping | [SS_10-2_Windows_Firewall_Rule_Blocking_Ping_On_BAA_BIG_FILE1.jpg](SS_10-2_Windows_Firewall_Rule_Blocking_Ping_On_BAA_BIG_FILE1.jpg) | Windows firewall rule configuration. |
| 10.3 | Ping blocked after firewall change | [SS_10-3_Ping_Blocked_After_Windows_Firewall_Change.jpg](SS_10-3_Ping_Blocked_After_Windows_Firewall_Change.jpg) | Proves ICMP is blocked. |
| 10.4 | Required services still accessible after ping block | [SS_10-4_SMB_Service_Still_Accessible_After_Ping_Block.jpg](SS_10-4_SMB_Service_Still_Accessible_After_Ping_Block.jpg) | Confirms SMB still works. |
| 10.5 | Linux firewall status | [SS_10-5_Linux_UFW_Firewall_Status_On_BAA_BIG_LX1.jpg](SS_10-5_Linux_UFW_Firewall_Status_On_BAA_BIG_LX1.jpg) | UFW firewall status. |
| 10.6 | Linux application access allowed | [SS_10-6_Linux_Application_Access_Allowed_From_Workstation.jpg](SS_10-6_Linux_Application_Access_Allowed_From_Workstation.jpg) | Application access through Linux firewall. |

## 11. Performance and Diagnostic Evidence

| No. | Checklist requirement | Screenshot file / link | Notes |
|---|---|---|---|
| 11.1 | Windows Task Manager or Performance Monitor | [SS_11-1_Windows_Task_Manager_Performance_On_BAA_BIG_FILE1.jpg](SS_11-1_Windows_Task_Manager_Performance_On_BAA_BIG_FILE1.jpg) | Windows server performance monitoring. |
| 11.2 | Windows Event Viewer with no critical service errors | [SS_11-2_Windows_Event_Viewer_No_Critical_Service_Errors_On_BAA_BIG_FILE1.jpg](SS_11-2_Windows_Event_Viewer_No_Critical_Service_Errors_On_BAA_BIG_FILE1.jpg) | Windows diagnostic review. |
| 11.3 | Server Manager showing roles/services running | [SS_11-3_Server_Manager_Roles_And_Services_Running_On_BAA_BIG_FILE1.jpg](SS_11-3_Server_Manager_Roles_And_Services_Running_On_BAA_BIG_FILE1.jpg) | Windows service status. |
| 11.4 | Ubuntu CPU, memory, disk, and network status | [SS_11-4_Ubuntu_CPU_Memory_Disk_Network_Status_On_BAA_BIG_LX1.jpg](SS_11-4_Ubuntu_CPU_Memory_Disk_Network_Status_On_BAA_BIG_LX1.jpg) | Linux performance monitoring. |
| 11.5 | Ubuntu service status for web/FTP/proxy/NTP/mail | [SS_11-5_Ubuntu_Service_Status_For_SFTP_Proxy_NTP_On_BAA_BIG_LX1.jpg](SS_11-5_Ubuntu_Service_Status_For_SFTP_Proxy_NTP_On_BAA_BIG_LX1.jpg) | Linux service diagnostics. |
| 11.6 | Hyper-V Manager showing VM health | [SS_11-6_Hyper-V_Manager_Showing_VM_Health.jpg](SS_11-6_Hyper-V_Manager_Showing_VM_Health.jpg) | VM health evidence. |
| 11.7 | Diagnostic report or command output | [SS_11-7_Diagnostic_Report_Command_Output_On_BAA_BIG_FILE1.jpg](SS_11-7_Diagnostic_Report_Command_Output_On_BAA_BIG_FILE1.jpg) | Diagnostic command output. |

## 12. High Availability / Cluster Evidence

| No. | Checklist requirement | Screenshot file / link | Notes |
|---|---|---|---|
| 12.1 | Failover Cluster Manager showing cluster nodes | [SS_12-1_Failover_Cluster_Manager_Showing_BAA_NEST_CL1_Nodes.jpg](SS_12-1_Failover_Cluster_Manager_Showing_BAA_NEST_CL1_Nodes.jpg) | Shows BAA-NEST-CL1 nodes. |
| 12.2 | Cluster Shared Volume or shared storage | [SS_12-2_Cluster_Shared_Volume_And_BAA_STOR1_Shared_Storage.jpg](SS_12-2_Cluster_Shared_Volume_And_BAA_STOR1_Shared_Storage.jpg) | CSV and shared storage evidence. |
| 12.3 | Test VM running as clustered role | [SS_12-3_BAA_TEST_VM01_Running_As_Clustered_Role.jpg](SS_12-3_BAA_TEST_VM01_Running_As_Clustered_Role.jpg) | Cluster-protected test VM. |
| 12.4 | Controlled VM move from one node to another | [SS_12-4_Controlled_VM_Move_From_BAA_BIG_Nest1_To_BAA_SML_Nest1.jpg](SS_12-4_Controlled_VM_Move_From_BAA_BIG_Nest1_To_BAA_SML_Nest1.jpg) | Planned migration evidence. |
| 12.5 | VM running after move/failover | [SS_12-5_BAA_TEST_VM01_Running_After_Move_On_Target_Node.jpg](SS_12-5_BAA_TEST_VM01_Running_After_Move_On_Target_Node.jpg) | VM running after movement. |
| 12.6 | Ping or service access before and after VM move | [SS_12-6_SSH_Service_Access_Before_And_After_VM_Move.jpg](SS_12-6_SSH_Service_Access_Before_And_After_VM_Move.jpg) | Service continuity after VM movement. |

## 13. Troubleshooting Evidence

| No. | Troubleshooting item | Screenshot file / link | Notes |
|---|---|---|---|
| TS-01 Before | AD user creation password policy failed | [SS_13-1_AD_User_Create_Failed_Password_Policy.jpg](SS_13-1_AD_User_Create_Failed_Password_Policy.jpg) | Before evidence. |
| TS-01 After | AD test users created | [SS_13-4_AD_Test_Users_Created.jpg](SS_13-4_AD_Test_Users_Created.jpg) | After evidence for user creation. |
| TS-02 Before | Enhanced Session / RDS logon denied | [SS_13-6_Workstation_Test_User_RDS_Logon_Denied.png](SS_13-6_Workstation_Test_User_RDS_Logon_Denied.png) | Before evidence. This file is PNG. |
| TS-02 After | Basic Session login succeeded | [SS_13-7_Workstation_Test_User_Basic_Session_Login.jpg](SS_13-7_Workstation_Test_User_Basic_Session_Login.jpg) | After evidence. |
| TS-03 Before | SFTP upload failed due to incorrect local path | [SS_13-5_SFTP_Upload_Failed_Local_Path.jpg](SS_13-5_SFTP_Upload_Failed_Local_Path.jpg) | Before evidence. |
| TS-03 After | SFTP upload successful | [SS_13-6_SFTP_Upload_Successful.jpg](SS_13-6_SFTP_Upload_Successful.jpg) | After evidence. |
| TS-04 Before | WordPress redirected to old Daydream Travel domain | [SS_13-8_WordPress_Redirected_To_Old_Daydream_Domain.jpg](SS_13-8_WordPress_Redirected_To_Old_Daydream_Domain.jpg) | Before evidence. |
| TS-04 After | WordPress URLs updated to Anzac Airport HTTPS | [SS_13-9_WordPress_URLs_Updated_To_Anzac_Airport_HTTPS.jpg](SS_13-9_WordPress_URLs_Updated_To_Anzac_Airport_HTTPS.jpg) | After evidence. |
| TS-05 Before | WordPress invalid JSON response | [SS_13-8A_WordPress_Update_Failed_Invalid_JSON_Response.jpg](SS_13-8A_WordPress_Update_Failed_Invalid_JSON_Response.jpg) | Before evidence. |
| TS-05 After A | WordPress page save issue resolved | [SS_13-9A_WordPress_JSON_Issue_Resolved_Page_Saved.jpg](SS_13-9A_WordPress_JSON_Issue_Resolved_Page_Saved.jpg) | After evidence. |
| TS-05 After B | WordPress REST API returns HTTP 200 JSON | [SS_13-9B_WordPress_REST_API_Returns_200_OK_JSON.jpg](SS_13-9B_WordPress_REST_API_Returns_200_OK_JSON.jpg) | After evidence. |
| TS-06 Before | Domain controller availability failed during BAA-BIG-DC1 shutdown | [SS_13-12_Domain_Controller_Availability_Failed_During_BIG_DC1_Shutdown.jpg](SS_13-12_Domain_Controller_Availability_Failed_During_BIG_DC1_Shutdown.jpg) | Main before evidence. |
| TS-06 Diagnostic | BAA-SML-DC1 DNS, LDAP, Kerberos working; SYSVOL issue observed | [SS_13-13_BAA_SML_DC1_DNS_LDAP_Kerberos_Working_SYSVOL_Missing.jpg](SS_13-13_BAA_SML_DC1_DNS_LDAP_Kerberos_Working_SYSVOL_Missing.jpg) | Supporting diagnostic evidence. |
| TS-06 Diagnostic | BAA-SML-DC1 SYSVOL and NETLOGON share check | [SS_13-14_BAA_SML_DC1_SYSVOL_NETLOGON_Share_Check.jpg](SS_13-14_BAA_SML_DC1_SYSVOL_NETLOGON_Share_Check.jpg) | Supporting diagnostic evidence. |
| TS-06 Before fix | DHCP DNS option missing BAA-SML-DC1 | [SS_13-15_DHCP_DNS_Option_Before_Fix_Missing_SML_DC1.jpg](SS_13-15_DHCP_DNS_Option_Before_Fix_Missing_SML_DC1.jpg) | Root cause evidence. |
| TS-06 Fix | DHCP DNS option updated with both domain controllers | [SS_13-16_DHCP_DNS_Option_Updated_With_Both_Domain_Controllers.jpg](SS_13-16_DHCP_DNS_Option_Updated_With_Both_Domain_Controllers.jpg) | Configuration correction evidence. |
| TS-06 Fix verification | Workstation DHCP renewed with both DNS servers | [SS_13-17_BAA_BIG_WS_DHCP_Renewed_With_Both_DNS_Servers.jpg](SS_13-17_BAA_BIG_WS_DHCP_Renewed_With_Both_DNS_Servers.jpg) | Client-side correction evidence. |
| TS-06 After | Domain controller availability retest using BAA-SML-DC1 | [SS_13-18_Domain_Controller_Availability_Retest_Using_BAA_SML_DC1.jpg](SS_13-18_Domain_Controller_Availability_Retest_Using_BAA_SML_DC1.jpg) | Main after evidence. |

## 14. Final Document Evidence

| No. | Checklist requirement | Screenshot file / link | Notes |
|---|---|---|---|
| 14.1 | Final VM list after implementation | [SS_14-1_Final_VM_List_After_Implementation.jpg](SS_14-1_Final_VM_List_After_Implementation.jpg) | Upload after final review if used. |
| 14.2 | Final service status summary | [SS_14-2_Final_Service_Status_Summary.jpg](SS_14-2_Final_Service_Status_Summary.jpg) | Upload after final review if used. |
| 14.3 | Final test plan with results completed | [SS_14-3_Final_Test_Plan_With_Results_Completed.jpg](SS_14-3_Final_Test_Plan_With_Results_Completed.jpg) | Completed Test Plan screenshot. |
| 14.4 | Final troubleshooting document completed | [SS_14-4_Final_Troubleshooting_Document_Completed.jpg](SS_14-4_Final_Troubleshooting_Document_Completed.jpg) | Completed Troubleshooting Log screenshot. |
| 14.5 | Final report sign-off page | [SS_14-5_Final_Report_Sign_Off_Page.jpg](SS_14-5_Final_Report_Sign_Off_Page.jpg) | Final Report sign-off screenshot. |

## Quick final upload check

Before submission, confirm the following links open correctly in GitHub:

- SS_8-1 to SS_8-2D for Azure Update Manager
- SS_8-3 to SS_8-5 for printer evidence
- SS_8-6 and SS_8-7 for Squid proxy evidence
- SS_9-1 to SS_9-6 for backup and restore
- SS_10-1 to SS_10-6 for firewall testing
- SS_11-1 to SS_11-7 for performance and diagnostics
- SS_12-1 to SS_12-6 for high availability
- SS_13-12 to SS_13-18 for domain controller availability troubleshooting
- SS_14-3 to SS_14-5 for final document evidence
