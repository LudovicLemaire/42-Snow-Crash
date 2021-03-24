# level 00

### ![#E6A23C](https://via.placeholder.com/15/E6A23C/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ ‎‏‏‎Exploit`

Utiliser la commande find pour trouver tous les fichiers auxquels le user level00 a accès
```cmd
find / -group flag00 2>/tmp/wow
```
On trouve deux fichiers
```
/usr/sbin/john
/rofs/usr/sbin/john
```

En faisant un cat des fichiers, on trouve le code `cdiiddwpgswtgt`

En faisant un décrypt [with decode](https://www.dcode.fr/caesar-cipher) on trouve que c'est encrypté avec un rot15.

En faisant un reverse, on trouve le code `nottoohardhere`

```cmd
su flag00 nottoohardhere
getflag
```

### ![#67C23A](https://via.placeholder.com/15/67C23A/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ Flag`
```
x24ti5gi3x0ol2eh4esiuxias
```