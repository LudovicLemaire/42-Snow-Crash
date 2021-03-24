# level 01

### ![#409EFF](https://via.placeholder.com/15/409EFF/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ Password`
```
x24ti5gi3x0ol2eh4esiuxias
```

### ![#E6A23C](https://via.placeholder.com/15/E6A23C/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ ‎‏‏‎Exploit`

Même technique qu'avant, on affiche le fichier auxquel on a accès
```console
cat /etc/passwd
```

On voit que flag01 est encrypté différemment
```js
flag01:42hDRfypTqqnw:3001:3001::/home/flag/flag01:/bin/bash
```

On récupère le fichier pour le mettre dans l’outil John The Ripper
```js
scp -P 4242 level00@192.168.1.22:/etc/passwd ./Developpement/42-snowcrash
```

D’abord clean le fichier pour garder uniquement le flag01 `flag01:42hDRfypTqqnw`

Puis lancer le logiciel
```
john ./passwd
Loaded 1 password hash (descrypt, traditional crypt(3) [DES 128/128 AVX-16])
abcdefg		(flag01)
```

```cmd
su flag01 abcdefg
getflag
```

### ![#67C23A](https://via.placeholder.com/15/67C23A/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ Flag`
```
f2av5il02puano7naaf6adaaf
```