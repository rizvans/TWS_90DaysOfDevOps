## Environment Basics - 
* Command: `uname -a`
  
  output : `Linux ip-172-31-17-40 6.14.0-1018-aws #18~24.04.1-Ubuntu SMP Mon Nov 24 19:46:27 UTC 2025 x86_64 x86_64 x86_64 GNU/Linux`
  
  Observation : Kernel version and architecture confirmed.

* Command: `cat /etc/os-release`
  
  output: `PRETTY_NAME="Ubuntu 24.04.3 LTS"
          NAME="Ubuntu"
          VERSION_ID="24.04"
          VERSION="24.04.3 LTS (Noble Numbat)"
          VERSION_CODENAME=noble
          ID=ubuntu
          ID_LIKE=debian
          HOME_URL="https://www.ubuntu.com/"
          SUPPORT_URL="https://help.ubuntu.com/"
          BUG_REPORT_URL="https://bugs.launchpad.net/ubuntu/"
          PRIVACY_POLICY_URL="https://www.ubuntu.com/legal/terms-and-policies/privacy-policy"
          UBUNTU_CODENAME=noble
          LOGO=ubuntu-logo`
  
   Observation : Confirms distribution and release version.

## Filesystem sanity -
* Command: `mkdir /tmp/runbook-demo`
  
  Observation: Directory created successfully in tmp.

* Command: `cp /etc/hosts /tmp/runbook-demo/hosts-copy && ls -l /tmp/runbook-demo`
  
  Observation: It copies the source file to runbook demo && means if copy works then shows the copies file with full list details.

## CPU Memory -
* Command: `top`
  
  Observation: It will show running processes with CPU usage, memory, PID, who started the server etc.

* Command: `ps -p pid -o pid,cmd,%cpu,%mem (after -p pid, pass the pid number of service)`
  
  Observation: It will give output details of the service in these 4 columns pid, cmd, pcpu,pmem

* Command: `free -h`
  
  Observation: Gives you free available memory details

## Disk/IO - 
* Command: `df -h`
  
  Observation: disk free, Gives you the disk available and mounted details

* Command: `du -h`
  
  Observation: Disk usage, Files and folders usage details

## Network -
* Command: `sudo ss -tulpn | grep sshd`
  
  Output: tcp   LISTEN 0      4096             0.0.0.0:22        0.0.0.0:*    users:(("sshd",pid=4229,fd=3),("systemd",pid=1,fd=205))
  
  Observation: ssh is listening to port 22

## Logs-
* Command: `journalctl -u ssh -n 50`
  
  Observation: Last 50 lines shows no error.

*Command: `tail -n 50 /var/log/auth.log `

Observation: Login attempts record

## If things worsen-
- Check logs
- restart service
- check cpu/storage
- check port

  
  

