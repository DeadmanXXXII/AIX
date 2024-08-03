# AIX

Here’s a comprehensive list of commands specific to AIX (Advanced Interactive eXecutive), IBM's Unix operating system.

# AIX Commands

## System Information

- **Check AIX version:**
  ```bash
  oslevel
  ```

- **Get detailed system information:**
  ```bash
  uname -a
  ```

- **List installed software:**
  ```bash
  lslpp -l
  ```

- **Display system configuration:**
  ```bash
  lsattr -El sys0
  ```

- **Check hardware details:**
  ```bash
  lshw
  ```

- **List all devices:**
  ```bash
  lsdev -C
  ```

## Package Management

- **Install a package:**
  ```bash
  installp -a -d /path/to/package.pkg
  ```

- **Update installed packages:**
  ```bash
  update_all -d /path/to/package.pkg
  ```

- **Remove a package:**
  ```bash
  installp -u packagename
  ```

- **Check package status:**
  ```bash
  lslpp -l packagename
  ```

## File and Directory Management

- **List files and directories:**
  ```bash
  ls
  ```

- **Change directory:**
  ```bash
  cd directoryname
  ```

- **Create a directory:**
  ```bash
  mkdir directoryname
  ```

- **Remove a directory:**
  ```bash
  rmdir directoryname
  ```

- **Copy files:**
  ```bash
  cp sourcefile destinationfile
  ```

- **Move files:**
  ```bash
  mv sourcefile destinationfile
  ```

- **Delete files:**
  ```bash
  rm filename
  ```

- **Find files:**
  ```bash
  find /path/to/search -name "filename"
  ```

- **Search for text within files:**
  ```bash
  grep "searchtext" filename
  ```

## System Monitoring and Management

- **Check disk usage:**
  ```bash
  df -g
  ```

- **Check disk space usage by directory:**
  ```bash
  du -g /path/to/directory
  ```

- **List all running processes:**
  ```bash
  ps -ef
  ```

- **Monitor system performance:**
  ```bash
  topas
  ```

- **View system logs:**
  ```bash
  errpt
  ```

- **Check network configuration:**
  ```bash
  ifconfig -a
  ```

- **List all network interfaces:**
  ```bash
  lsdev -Cc adapter
  ```

## User and Permissions Management

- **List all users:**
  ```bash
  lsuser all
  ```

- **Add a new user:**
  ```bash
  mkuser username
  ```

- **Delete a user:**
  ```bash
  rmuser username
  ```

- **Change file permissions:**
  ```bash
  chmod permissions filename
  ```

- **Change file ownership:**
  ```bash
  chown owner:group filename
  ```

## System Maintenance

- **Run disk repair:**
  ```bash
  fsck -y /dev/hdisk0
  ```

- **Verify disk structure:**
  ```bash
  lspv
  ```

- **Update the AIX operating system:**
  ```bash
  smit update_all
  ```

- **Check system status and health:**
  ```bash
  vmstat
  ```

## Networking

- **Ping a host:**
  ```bash
  ping hostname
  ```

- **Trace route to a host:**
  ```bash
  traceroute hostname
  ```

- **View network routing table:**
  ```bash
  netstat -rn
  ```

- **Manage network interfaces:**
  ```bash
  ifconfig interface
  ```

- **Configure network interfaces:**
  ```bash
  mkdev -c adapter -s network -t interface
  ```

## Security

- **Check for open ports:**
  ```bash
  netstat -an
  ```

- **Manage firewall settings (if applicable):**
  ```bash
  no -a
  ```

- **View security logs:**
  ```bash
  /usr/bin/errpt
  ```

## Miscellaneous

- **Generate a system report:**
  ```bash
  sysreport
  ```

- **Reboot the system:**
  ```bash
  shutdown -r now
  ```

This list covers a range of AIX commands for system management, file operations, and network configuration. Use these commands to administer and troubleshoot AIX systems effectively.
