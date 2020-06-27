# Home Server

Notes, tips, tricks, cheat sheets, designs, layouts, tools, plans, etc. for my home server. Currently, this is `whiplash`.

## ZFS



- Need to have regular scrubs... Weekly for consumer-grade disks
- Snapshots are like file system versions
  - http://www.openoid.net/why-sanoids-zfs-replication-matters/

### Cheat Sheets

- https://www.thegeekdiary.com/solaris-zfs-command-line-reference-cheat-sheet/
- https://blog.programster.org/zfs-cheatsheet
- http://www.datadisk.co.uk/html_docs/sun/sun_zfs_cs.htm
- https://cheatography.com/the-iceman-blog/cheat-sheets/zfs-command-line-reference/
- http://unix-karri.com/zfs-cheat-sheet/
- https://hamwaves.com/zfs/en/zfs.a4.pdf

## General File System


## Screen


## RSync


## Plans

### Ideal

Stored off-site, but server is a local write-through cache which also updates as external systems update the off-site source. A pull + push cache. Cache is "smart", with more frequently accessed stuff, and _then_ recently accessed stuff, is cached with a higher priority than less-frequently and less-recently accesed stuff.

### Backup



### 




