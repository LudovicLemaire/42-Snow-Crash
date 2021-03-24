# level 13

### ![#409EFF](https://via.placeholder.com/15/409EFF/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ Password`
```
g1qKMiRpXf53AWhDaU7FEkczr
```

### ![#E6A23C](https://via.placeholder.com/15/E6A23C/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ ‎‏‏‎Exploit`

Il y a un binaire, il attend un UID 4242.

En analysant le binaire on voit qu’il fait un compare. Y’a qu’à le skip en faisant un disass.
```cmd
gdb ./level13
disass main
```
On met un breakpoint au niveau du cmp
```c
break *0x0804859a
```
On reprend
```js
run
```
Il s’arrête au breakpoint, on jump dans le programme là où le compare serait valide.
```c
jump *0x080485cb
```
Le token s’affiche `2A31L79asukciNyi8uppkEuSx`


```cmd
su level14
```

### ![#67C23A](https://via.placeholder.com/15/67C23A/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ Flag`
```
2A31L79asukciNyi8uppkEuSx
```