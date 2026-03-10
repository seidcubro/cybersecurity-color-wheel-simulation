# Incident Timeline Diagram

```mermaid
timeline
    title 2:13 AM VPN Login Incident Timeline

    01:07:13 : Phishing email delivered to jordan.rivera@wvrus.org
    02:12:41 : High-risk IdP sign-in attempt from Eastern Europe
    02:12:44 : MFA push 1 sent
    02:12:58 : MFA push 2 sent
    02:13:11 : MFA push 3 sent
    02:13:22 : MFA push 4 sent
    02:13:35 : MFA push 5 sent
    02:13:47 : MFA push 6 approved
    02:13:52 : VPN authentication successful
    02:22 - 02:29 : svc-backup-reports authenticates across multiple hosts
    02:27:14 : READ on \\FS-RES-02\Research_Contracts\Q1\
    02:28:01 : READ on deliverables directory
    02:31:20 : contracts_Q1.zip created
    02:33:09 : Scheduled task created on FS-RES-02 via PowerShell
    02:35:44 : ZIP moved to ProgramData temp path
    02:36:12 : DNS query to sync-storage-cloud[.]com from FS-RES-02
    02:37 - 02:41 : Proxy shows ~420 MB outbound to suspicious cloud domain
    02:35 - 02:45 : VPN stats show 510 MB outbound
```

