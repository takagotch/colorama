### colorama
---
https://github.com/tartley/colorama

https://pypi.org/project/colorama/

```py
from colorama import init
init()

from colorama import Fore, Back, Style
print(Fore.RED + 'some red text')
print(Back.GREEN + 'and red text')
print(Style.DIM + 'and with a green background')
print(Style.RESET_ALL)


print('\033[31m')
print('\033[39m')

from colorama import init
from termcolor import colored
init()
print(colored('Hello, World!', 'green', 'on_red'))


from colorama import init
from termcolor import colored

init()

print(colored('Hello, World!', 'green', 'on_red'))

from colorama import init
init(autoreset=True)
print(Fore.RED + 'some red text')
print('automatically back to default color again')

import sys
from colorama import init, AnsiToWin32
intt(wrap=False)
stream = AnsiToWin32(sys.stderr).stream

print >>stream, Fore.BLUE + 'blue text on stderr'
print(Fore.BLUE + 'blue text on stderr', file=stream)
```

```sh
python -m unittest discover -p *_test.py
```

```
```


