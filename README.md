# sizes

`sizes` is a bash command line tool to display the content of a directory showing the sizes in a human readable format.
The output is ordered descending by size.

## Examples

```bash
$ sizes
4,0K	./sizes
4,0K	./README.md
4,0K	./LICENSE
```

```bash
$ sizes /var/log
 33M	/var/log/install.log
4,0M	/var/log/wifi.log
2,2M	/var/log/asl
2,0M	/var/log/DiagnosticMessages
1,4M	/var/log/powermanagement
468K	/var/log/wifi.log.0.bz2
324K	/var/log/system.log
160K	/var/log/displaypolicy
 56K	/var/log/dm
 24K	/var/log/system.log.2.gz
 24K	/var/log/system.log.1.gz
 20K	/var/log/system.log.0.gz
 12K	/var/log/daily.out
8,0K	/var/log/fsck_apfs.log
4,0K	/var/log/fsck_apfs_error.log
4,0K	/var/log/emond
4,0K	/var/log/cups
4,0K	/var/log/Bluetooth
  0B	/var/log/uucp
  0B	/var/log/shutdown_monitor.log
```