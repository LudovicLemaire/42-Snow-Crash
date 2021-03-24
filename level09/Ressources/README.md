# level 09

### ![#409EFF](https://via.placeholder.com/15/409EFF/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ Password`
```
25749xKZ8L7DkSCwJkT9dyv6f
```

### ![#E6A23C](https://via.placeholder.com/15/E6A23C/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ ‎‏‏‎Exploit`

On remarque que le binaire root chaque char différemment (+1 à chaque fois).

En faisant un ltrace on voit
```c
puts("You should not reverse this")
```

Il faut donc reverse +1 et l’appliquer au token.

Petit script en C

```c
#include <string.h>
#include <stdio.h>

int	main(int ac, char **av) {
	int i = 0;
	while (i < strlen(av[1])) {
		av[1][i]-= i;
		i++;
	}
	puts(av[1]);
	return (0);
}
```

On compile `gcc wow.c -o wow`

Puis dans `/tmp`
```js
./wow `cat ~/token`
```

Ce qui récupère le flag `f3iji1ju5yuevaus41q1afiuq`



```cmd
su flag09 f3iji1ju5yuevaus41q1afiuq
getflag
```

### ![#67C23A](https://via.placeholder.com/15/67C23A/000000?text=+) `‎‎‎‎‎‎‎‏‏‎ Flag`
```
s5cAJpM8ev6XHw998pRWG728z
```