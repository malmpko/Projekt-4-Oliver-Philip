## Kvoter

Projektet använder gruppkvoter på NFS-servern. Katalogen `/shares` ligger på ett separat ext4-filsystem som monteras med stöd för `usrquota` och `grpquota`.

Kvoterna är satta per grupp:

| Grupp | Soft limit | Hard limit |
|---|---:|---:|
| avd_a | 20 MB | 25 MB |
| avd_b | 20 MB | 25 MB |

Kvoten verifierades genom att användaren `anna`, som tillhör gruppen `avd_a`, försökte skapa en fil på 100 MB i `/mnt/avdelning-a`. Testet stoppades med meddelandet `Disk quota exceeded`, vilket visar att gruppkvoten fungerar.