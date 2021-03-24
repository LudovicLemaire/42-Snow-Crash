# level ??

### ![#409EFF](https://via.placeholder.com/15/409EFF/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ Password`
```
wiok45aaoguiboiki2tuin6ub
```

### ![#E6A23C](https://via.placeholder.com/15/E6A23C/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ ‎‏‏‎Exploit`

On trouve un binaire, on analyse via ltrace

Il fait appelle à getenv de LOGNAME

En faisant un export de logname en wow, le programme print wow

Avec le bon formatage unix, on peut remplacer wow par un print de la commande getflag
```js
export LOGNAME=\`getflag\`
```

```cmd
su level08
```

### ![#67C23A](https://via.placeholder.com/15/67C23A/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ Flag`
```
fiumuikeil55xe9cu4dood66h
```