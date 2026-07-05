---
date: 2026-06-30
tags: [note, linux, gentoo]
id: u3sj
aliases: []
---

# gentoo

## useful commands:

emerge -s/-S - search name/description
emerge --sync - update repos
emerge -auDN @world - update/apply new use
equery uses/meta <pkgname> - get uses and versions of package
qeuery files <pkgsname> - get files that provided by installed package
eclean-dist/eclean-kernel - cleanup
emerge --noreplace <pkgname> - move package from deps to @world
emerge --deselect <pkgname> - plan package for a remove in the next --depclean run
emerge --depclean - remove unneeded deps and deselected packages
emerge --oneshot <pkgname> - package will be removed with next --depclean
emerge --info - shitload of info about the system
emerge -C <pkgname> - remove package that isn't in @world (installed  non-explicitly)
emaint all - clean-up


## notes

- never install xdg-portal-gnome along with niri, creates open dialog bugs.
