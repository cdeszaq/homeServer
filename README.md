# Home Server

Notes, tips, tricks, cheat sheets, designs, layouts, tools, plans, etc. for my home server. Currently, this is `whiplash`.

## ZFS



- Need to have regular scrubs... Weekly for consumer-grade disks
- Snapshots are like file system versions
  - http://www.openoid.net/why-sanoids-zfs-replication-matters/
- Keep the pool allocation under 80%
- Always export your storage pool before performing a `do-release-upgrade` to a newer version of your distribution or before moving the drives from one physical system to another! **Failure to do so, may render the zpool unmountable.**

### Cheat Sheets

- https://www.thegeekdiary.com/solaris-zfs-command-line-reference-cheat-sheet/
- https://blog.programster.org/zfs-cheatsheet
- http://www.datadisk.co.uk/html_docs/sun/sun_zfs_cs.htm
- https://cheatography.com/the-iceman-blog/cheat-sheets/zfs-command-line-reference/
- http://unix-karri.com/zfs-cheat-sheet/
- https://hamwaves.com/zfs/en/zfs.a4.pdf
- https://www.csparks.com/ZFS%20Without%20Tears.md
- https://pthree.org/2012/04/17/install-zfs-on-debian-gnulinux/
- https://wiki.ubuntu.com/Kernel/Reference/ZFS
- https://lildude.co.uk/zfs-cheatsheet
- https://arstechnica.com/information-technology/2014/02/ars-walkthrough-using-the-zfs-next-gen-filesystem-on-linux/
- 

### General links



## General File System


## Screen


## RSync


## Other cheat-sheets

- https://www.csparks.com/LinuxCommands.md (many here)

## Other Info

- Verifying copies across file systems: http://www.openoid.net/verifying-copies/


## Plans

### Ideal

Stored off-site, but server is a local write-through cache which also updates as external systems update the off-site source. A pull + push cache. Cache is "smart", with more frequently accessed stuff, and _then_ recently accessed stuff, is cached with a higher priority than less-frequently and less-recently accesed stuff.

Possibly something like a local ZFS set of files and a remote share, with RSync keeping things in sync between the local and the remote (in both directions)? Would also allow layering in large objects via S3FS, possibly tucked into Glacier.

### Backup



### 




