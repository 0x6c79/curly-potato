---
title: "问题合集"
date: 2024-07-01
draft: false
description: "记录遇见的问题及解决方法。"
tags: ["problems"]
---

# archlinux 中PipeWire音频出现撕裂（电流声）
---
wireplumber是一个强大的pipewire会话和代理管理器
默认配置文件位置：`/usr/share/wireplumber/`
全局配置文件位置：`/etc/wireplumber/`
单一用户的配置文件位置：`~/.config/wireplumber/`
默认情况下，wireplumber只有默认配置文件，需要用户创建全局或单一用户配置文件
然后重启用户守护进程`systemctl --user daemon-reload`，然后重启计算机

# 如何删除Git submodule
---
1. Delete the relevant line from the `.gitmodules` file.
2. Delete the relevant section from `.git/config`.
3. Run `git rm --cached path_to_submodule` (no trailing slash).
4. Commit and delete the now untracked submodule files.

# Mount a local Hard Disk
---
获取硬盘UUID
```bash
lsblk --fs # to check disk's UUID
sudo vim /etc/fstab
```
编辑 /etc/fstab
```vim
# Static information about the filesystems.
# See fstab(5) for details.

# <file system> <dir> <type> <options> <dump> <pass>
# /dev/nvme0n1p2
UUID=7c4f1907-3834-4722-b2b4-ed71163ac45f	/         	btrfs     	rw,relatime,ssd,discard=async,space_cache=v2,subvolid=256,subvol=/@	0 0

# /dev/nvme0n1p2
UUID=7c4f1907-3834-4722-b2b4-ed71163ac45f	/home     	btrfs     	rw,relatime,ssd,discard=async,space_cache=v2,subvolid=257,subvol=/@home	0 0

# /dev/nvme0n1p2
UUID=7c4f1907-3834-4722-b2b4-ed71163ac45f	/var/log  	btrfs     	rw,relatime,ssd,discard=async,space_cache=v2,subvolid=258,subvol=/@log	0 0

# /dev/nvme0n1p2
UUID=7c4f1907-3834-4722-b2b4-ed71163ac45f	/var/cache/pacman/pkg	btrfs     	rw,relatime,ssd,discard=async,space_cache=v2,subvolid=259,subvol=/@pkg	0 0

# /dev/nvme0n1p2
UUID=7c4f1907-3834-4722-b2b4-ed71163ac45f	/.snapshots	btrfs     	rw,relatime,ssd,discard=async,space_cache=v2,subvolid=260,subvol=/@.snapshots	0 0

# /dev/nvme0n1p1
UUID=94ED-F31F      	/boot     	vfat      	rw,relatime,fmask=0022,dmask=0022,codepage=437,iocharset=ascii,shortname=mixed,utf8,errors=remount-ro	0 2

# /dev/sda1  Games
UUID=4bd7c80d-ffa4-4bdb-a7db-34bf11e8127d	/mnt/Games	ext4	defaults	0 0

# /dev/sdb1 Data
UUID=88f60110-693d-430a-bdee-97d5169ee661	/mnt/Data	ext4	defaults	0 0
```


# SpeedTest
---
网络速度测试通常通过发送和接收数据包来测量网络的性能。工作原理通常包括以下步骤：

1. **选择测试服务器**：用户选择一个测试服务器，可以是一个远程服务器或者是提供速度测试服务的专用服务器。
2. **发送数据**：客户端向测试服务器发送一个已知大小的数据包。
3. **测量时间**：客户端记录发送数据包的时间戳。
4. **接收数据**：测试服务器接收数据包，并立即将其回传给客户端。
5. **测量时间**：客户端记录接收数据包的时间戳。
6. **计算速度**：客户端使用发送和接收数据包所花费的时间，结合已知的数据包大小，计算出网络的速度，通常以 Mbps（兆位每秒）为单位。

这是一个简化的网络速度测试工作原理的描述。实际的速度测试可能会考虑更多因素，例如网络延迟、数据包丢失率等。
