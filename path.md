# Directory Paths and Their Purpose

| Directory/Path         | Contains                                                                                                                                                                                                                       |
|-----------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| /etc/centrifydc       | The agent configuration file and the Kerberos configuration file.                                                                                                                        |
| /usr/share/centrifydc | Kerberos-related files and service library files used by the Centrify Agent to enable group policy and authentication and authorization services.                                         |
| /usr/sbin/usr/bin     | Command line programs to perform Active Directory tasks, such as joining a domain and changing a user password.                                                                           |
| /var/centrify         | Directories for temporary and common files that can be used by the agent.                                                                                                                |
| /var/centrifydc       | The IP address of the DNS server, details about the software you have installed, the Active Directory domain the computer is joined to, the Active Directory site the computer is part of, and other details. |
| /var/log              | Error messages, warnings, and informational messages, along with other kernel and program messages.                                                                                       |

---

# Centrify & Delinea Command Reference

| Command      | Description |
|--------------|-------------|
| `adcheck`    | Check the operating system, network, and Active Directory connections to verify readiness to join a domain. <br>**Syntax:** `adcheck domain_name [options]` |
| `adfinddomain` | Display the domain controller associated with the specified AD domain. <br>**Syntax:** `adfinddomain [options] domain_name` |
| `adgpupdate` | Retrieve and apply group policies from the AD domain controller. <br>**Syntax:** `adgpupdate [options]` |
| `adid`       | Display real and effective UIDs and GIDs for the current or specified user. <br>**Syntax:** `adid [option] [username\|uid]` |
| `adinfo`     | Display detailed AD, network, and diagnostic info for the local computer. <br>**Syntax:** `adinfo [options] [--user username[@domain]] [--password password]` |
| `adlicense`  | Display the current status of agent features on the local computer. |
| `adpasswd`   | Change your Active Directory password. |
| `adquery`    | Query AD for user/group info (backward compatibility). <br>**Syntax:** `adquery user\|group [options] [username\|groupname]` |
| `adsetgroups`| View or change group membership. <br>**Syntax:** `adsetgroups [options] group` |
| `adsmb`      | Perform file operations using the Delinea SMB stack. <br>**Syntax:** `adsmb file_operation -s share [options]` |
| `dzdo`       | Execute a privileged command as root or another user. <br>**Syntax:** `dzdo [options]` |
| `dzinfo`     | Display rights/roles info for users. <br>**Syntax:** `dzinfo [options]` |
| `dzsh`       | Run commands in a restricted environment shell. |