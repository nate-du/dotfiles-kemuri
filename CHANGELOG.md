### 26/08/08
> Remove steps 6 and 7 from install steps. No longer using KDE Plasma and CachyOS automatically configures limine snapper service when using btrfs. 

6. Import KDE Plasma settings with konsave

> konsave -i konsave/gruvbox-dark-mesh.knsv

> konsave -a gruvbox-dark-mesh

7. Enable limine-snapper-sync service
```
systemctl enable --now limine-snapper-sync.service
```