<h1> monkey-installer</h1>

<h2>Tutorial</h2>
(Assuming Your on a Brand New Archiso)<br>
pacman -Sy git - Syncs Package Repos & Installs Git<br>
git clone https://github.com/avvon/monkey-installer - Clones The Repo<br>

sh install.sh - Starts The Installer In Bash<br>
sh install-2.sh - Start Second Part In Bash<br>

exit -Exits Arch Install<br>
umount -l /mnt - Unmount Drives<br>
reboot<br>

<h2>Partitioning</h2>
<h3>Home And Root On Same Partition</h3>
g - GPT<br>

n - New Partition<br>
enter<br>
enter<br>
+550M<br>

n - New Partition<br>
enter<br>
enter<br>
+2G<br>

n - New Partition<br>
enter<br>
enter<br>
enter<br>

t - Change Filesystem<br>
1<br>
1<br>

t - Change Filesystem<br>
2<br>
19<br>

w - Write Changes<br>

<h3>Home And Root On Different Partitions</h3>
g - GPT<br>

n - New Partition<br>
enter<br>
enter<br>
+550M<br>

n - New Partition<br>
enter<br>
enter<br>
+2G<br>

n - New Partition<br>
enter<br>
enter<br>
+30G - Size Depends On Use Case<br>

n - New Partition<br>
enter<br>
enter<br>
enter<br>

t - Change Filesystem<br>
1<br>
1<br>

t - Change Filysystem<br>
2<br>
19<br>

w - Write Changes<br>


