# rclone-systemd-timer

Easy systemd backup service using rclone and cloud drive

### How to install

```
cp backup.service backup.timer /etc/systemd/system/
systemctl enable backup.timer
systemctl daemon-reload && systemctl daemon-reexec
```

### Defaults

- zstd archive format with max compression level
- remove old backups after 70 days
