<h1> monkey-installer</h1>

<h2>Tutorial</h2>
(Assuming Your on a Fresh Archiso)
pacman -Sy - Syncs Package Repos
pacman -S git - Installs Git
git clone https://github.com/avvon/monkey-installer - Clones The Repo

sh install.sh - Starts The Installer In Bash
sh install-2.sh - Start Second Part In Bash

exit -Exits Arch Install
umount -l /mnt - Unmount Drives
reboot

<h2>Partitioning</h2>
<h3>Home And Root On Same Partition</h3>
g - GPT

n - New Partition
enter
enter
+550M

n - New Partition
enter
enter
+2G

n - New Partition
enter
enter
enter

t - Change Filesystem
1
1

t - Change Filysystem
2
19

w - Write Changes

<h3>Home And Root On Different Partitions</h3>
g - GPT

n - New Partition
enter
enter
+550M

n - New Partition
enter
enter
+2G

n - New Partition
enter
enter
+30G - Size Depends On Use Case

n - New Partition
enter
enter
enter

t - Change Filesystem
1
1

t - Change Filysystem
2
19

w - Write Changes


