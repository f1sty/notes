---
date: 2026-06-30
tags: [note]
id: zhv3
aliases: []
---

# linux

## purge caches

sync
echo 3 > /proc/sys/vm/drop_caches

## control volume using wireplumber

wpctl get-volume @DEFAULT_AUDIO_SINK@
wpctl set-volume @DEFAULT_AUDIO_SINK@ 5%+

## useful commands

cat /proc/net/tcp
echo > /dev/tcp/127.0.0.1/<port>
sudo dpkg-reconfigure tzdata
dnf repoquery -l <pkgname>
udevadm info /dev/input/mice
evtest /dev/input/event2
netstat -ano | findstr [Port Number]
xdg-mime default org.pwmt.zathura.desktop application/pdf
xdg-mime query default application/pdf
mutool convert -F text -o - <file.pdf> | less - convert pdf to text on fly
