# level 02

### ![#409EFF](https://via.placeholder.com/15/409EFF/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ Password`
```
f2av5il02puano7naaf6adaaf
```

### ![#E6A23C](https://via.placeholder.com/15/E6A23C/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ ‎‏‏‎Exploit`

On voit un level02.pcap, qui est un fichier qui contient des traces réseaux. On le DL
```js
scp -P 4242 level02@192.168.1.22:~/level02.pcap ./Developpement/42-snowcrash
```

On l’ouvre dans wireshark. On passe rapidement dans chaque paquet voir si y’a qqch d'intéressant.
Un des paquets contient `password`.
On l’ouvre, on trouve
```js
..wwwbugs login: l.le.ev.ve.el.lX.X
..
Password: ft_wandr...NDRel.L0L
```

Les . sont des characters que wireshark n’arrive pas à afficher, on regarde l’hexa, les . représente 7f soit DEL en ascii.
Ce qui donne ft_waNDReL0L



```cmd
su flag02 ft_waNDReL0L
getflag
```

### ![#67C23A](https://via.placeholder.com/15/67C23A/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ Flag`
```
kooda2puivaav1idi4f57q8iq
```