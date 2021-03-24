# level 13

### ![#409EFF](https://via.placeholder.com/15/409EFF/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ Password`
```
2A31L79asukciNyi8uppkEuSx
```

### ![#E6A23C](https://via.placeholder.com/15/E6A23C/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ ‎‏‏‎Exploit`

Aucun fichier rien

Il ne reste plus que le getflag

Exactement comme avant
```sh
gdb getflag
disass main
```
Y’a bcp de bordel cette fois, on va break au premier test
```c
break *0x0804898e
run
```
Et là on essaie sur toutes les adresse juste après un jump
```c
jump *0x08048de5
```
On récupère le code `7QiHafiNa3HVozsaXkawuYrTstxbpABHD8CPnHJ`

Si on continue avec les post jump, on peut également récupérer tous les flags des levels précédents.


```cmd
su flag14
```

### ![#67C23A](https://via.placeholder.com/15/67C23A/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ Flag`
```
7QiHafiNa3HVozsaXkawuYrTstxbpABHD8CPnHJ
```